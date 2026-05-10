# bin/build — what's wired, what's stubbed

*Minimum-viable port of the NeurIPS build pipeline (`~/src/neurips/bin/build`) for the synthese-paper portfolio. Done 2026-05-09 against the Inquiry/T&F submission target. Companion files: `bin/build` (the script), `bin/refs` (citation data layer, already wired). For the venue-side rationale see `03-inquiry-ai-agents/planning/inquiry-submission-guidelines.md`.*

## What it does

Reads a paper-dir (e.g., `03-inquiry-ai-agents/`) containing:

- `meta.md` — YAML frontmatter (title, authors, abstract body, keywords) + abstract body after the second `---`.
- `OUT.<stem>.md` — markdown table whose rows enumerate segments under `<paper-dir>/src/`. Same shape as the NeurIPS pipeline so existing OUT manifests are portable.
- `src/*.md` — the actual segments. `\cite{key}` / `\citet{key}` / pandoc-style `[@key]` all work; pandoc's citeproc resolves them at render.

Produces:

- `<paper-dir>/<stem>.docx` — **primary submission artifact** for Inquiry/T&F. Word format is what T&F prefers (no LaTeX class is provided for *Inquiry*).
- `<paper-dir>/<stem>.pdf` — preview only (lualatex via pandoc). Not for submission; for the drafter's self-review.
- `<paper-dir>/.build/<stem>/<stem>.md` — concatenated intermediate (debug).
- `<paper-dir>/.build/<stem>/<stem>.references.bib` — emitted via `bin/refs emit`.

Citations: T&F house style is **Chicago author-date**. The build looks for `chicago-author-date.csl` (system texlive copy on this machine) and passes it to pandoc's `--citeproc`. Falls back to pandoc's bundled default if not found. Both LaTeX-style (`\cite{key}`, `\citet{}`, …) and pandoc-native (`[@key]`, `[-@key]`, `[@k1; @k2, p. 5]`, bare in-text `@key`) citation forms are supported and pre-scanned by `bin/refs emit`; either may be used freely in segment source.

## Conventions worth knowing

**Abstract source-of-truth.** If a manifest row has slug `abstract` (any type), the build *lifts* that file's prose into the YAML `abstract:` metadata field instead of concatenating it into the body. Otherwise meta.md's body-after-second-`---` is used. The lifting routine strips a leading H1 and any italic-only paragraphs (drafter notes like `*Drafted last per protocol.*`) so the source file can carry structural and workflow markers without polluting the metadata. Citations inside the abstract (`[-@nagel-1974-bat]` etc.) are processed by pandoc citeproc when rendered from a metadata field, so the abstract's bibliography integrates with the rest of the paper. — This honours the "abstract drafted last as a separate file" workflow without double-rendering against meta.md's placeholder.

**Two intermediates per build.** The build writes `<stem>.md` (full frontmatter, for DOCX) *and* `<stem>.pdf-preview.md` (keywords stripped, for PDF) into `.build/<stem>/`. The body is identical; only the YAML differs. The split exists because pandoc's LaTeX template threads `keywords:` through hyperxmp's `\xmpquote{...}` macro and lualatex fatals on it (and a CLI `--metadata=keywords:` override does *not* suppress the template loop). Stripping the field at YAML-assembly time is the clean fix; keywords still flow into the DOCX through its own intermediate.

**DOCX styling via reference doc.** Pandoc reads named styles, page setup, margins, and fonts from a reference Word document; body content still comes from markdown. Precedence: `<paper-dir>/reference.docx` → `common/reference.docx` → none (pandoc defaults). The build prints `(docx styled from <path>)` after success so the styling source is never silent.

`common/reference.docx` is currently Taylor & Francis's generic Word template (`TF_Template_Word_Windows_2016.dotx`, archived untouched at `common/vendor/`; renamed to `.docx` because pandoc accepts the OOXML payload either way). With this template applied, the build's DOCX picks up T&F's page geometry (A4 portrait, 25mm top/bottom × 30mm left/right margins), Times New Roman as the default body font, and en-GB locale. Of pandoc's named styles, three map cleanly to T&F-defined styles by name:

| Pandoc style | T&F style | Maps? |
|---|---|---|
| `Heading 1` / `Heading 2` / `Heading 3` / `Heading 4` | `heading 1`–`heading 4` | ✓ |
| `Abstract` | `Abstract` | ✓ |
| `Keywords` | `Keywords` | ✓ |
| `Footnote Text` / `Footnote Reference` | `footnote text` / `footnote reference` | ✓ |
| `Title` | `Article title` | ✗ (falls back to Word default) |
| `Author` | `Author names` | ✗ |
| `Block Text` (blockquote ≥50 w) | `Displayed quotation` | ✗ |
| `Bibliography` | `References` | ✗ |
| `First Paragraph` | (absent) | ✗ |

The four mismatches still render — they just use Word's default styles rather than T&F's house styling. To wire them up, edit `common/reference.docx` in Word and add the pandoc-name as an alias on the corresponding T&F style (right-click style → Modify → check "Add to Style Gallery" / set alternate names). That's styling-decision territory and a Word-side edit, not a build change.

## Wiring summary

| Concern | NeurIPS pipeline | This pipeline |
|---|---|---|
| Manifest format (`OUT.*.md` table) | Wired | **Wired (verbatim port)** |
| `meta.md` YAML frontmatter | Wired | **Wired (extended with `keywords` + `lang`)** |
| `bin/refs emit` shell-out | Wired | **Wired (same contract)** |
| Anonymisation lint at build | Wired | **Wired (same deny-list scan)** |
| Markdown → output | LaTeX (kramdown extensions, theorem environments, callouts, [[#^anchor]] xrefs) | **DOCX + PDF via pandoc** |
| Citation rendering | natbib super-numeric (NeurIPS house) | **Chicago author-date via pandoc citeproc** (T&F house) |
| Build-output target | `.pdf` (camera-ready) | `.docx` (submission) + `.pdf` (preview) |
| Page-budget side-tool | Wired (`bin/page-budget`) | Not ported (Inquiry has no word limit; calibration is dossier-side discipline, not build-time) |

## What's stubbed / not ported (and why)

- **Obsidian-callout system** (`> [!theorem]`, `> [!definition]`, `> [!table]`, `> [!figure]`, `> [!todo]`/`[!note]`/etc.). Useful in formal-results papers (NeurIPS); not load-bearing for analytical-philosophy prose. If a future paper wants theorem environments or table callouts, lift the kramdown parser/converter from `~/src/neurips/bin/build:75-480` and route around pandoc — but the simpler path for analytical philosophy is to write tables in plain markdown and skip theorem envs entirely.
- **`[[#^anchor]]` cross-references.** NeurIPS-specific Obsidian convention; pandoc's `[ref]{#anchor}` and `\Cref` flow are different. Not needed for paper 3.
- **Equation anchors / cleveref machinery.** N/A for analytical philosophy.
- **`\appendix` / appendix-aware section numbering.** If paper 3 needs an appendix, prefix the segment heading with the desired label (`# Appendix A: …`); pandoc renders verbatim.
- **`bin/refs lint` integration in build.** The build does a soft lint at build-time (deny-list scan against included segments). The hard gate before submission is still `bin/refs lint <paper-dir>` run separately, same as NeurIPS.
- **`<stem>.prior.pdf` snapshot.** Skipped — DOCX is the submission artifact; the PDF is preview-only and the drafter doesn't need a "last-known-good" rollback for a 4.5-hour sprint. Trivial to add (`FileUtils.mv` before publish) if it becomes useful.
- **Page-budget side-tool.** N/A; Inquiry has no word limit (verbatim from the T&F page) and the paper-dir already has its own dossier-side word target.

## What's deliberately NOT ported: LaTeX target

T&F provides Word templates for *Inquiry*, not a LaTeX class. Submitting LaTeX to *Inquiry* is not contraindicated, but there's no class file to compile against and a custom-LaTeX submission risks production-side rework. **DOCX is the right submission target.** If a future paper at a LaTeX-friendly venue (Synthese paper 1 at Springer, e.g.) needs a LaTeX build, the cleanest approach is a *separate* `bin/build-springer` rather than overloading this script.

## Invocation

```bash
# All manifests in 03-inquiry-ai-agents (will pick up OUT.*.md after drafter creates one)
bin/build 03-inquiry-ai-agents

# Specific manifest
bin/build 03-inquiry-ai-agents inquiry-ai-agents-2026

# From inside the paper-dir
cd 03-inquiry-ai-agents && ../bin/build
```

## Drafter quickstart

The paper 3 dossier currently has *no* `meta.md`, *no* `OUT.*.md`, and *no* `src/` directory. For the build to produce anything the drafter needs to land:

1. **`03-inquiry-ai-agents/meta.md`** — YAML frontmatter (`title`, `keywords`, `lang: en-GB`) + abstract body after the second `---`. T&F wants a 200-word unstructured abstract. Author block can be a single anonymised entry for review (`Anonymous Author / Affiliation pending`); cover page goes to a separate file at acceptance.

2. **`03-inquiry-ai-agents/OUT.<stem>.md`** — manifest table. Stem suggestion: `inquiry-ai-agents-2026` (matches the paper-3 framing in CLAUDE.md). Example minimum:

   ```
   | § | Type     | Slug                                | Title                          | Stage |
   |---|----------|-------------------------------------|--------------------------------|-------|
   | 1 | Section  | [intro](src/01-introduction.md)     | Introduction                   | draft |
   | 2 | Section  | [structure](src/02-structure.md)    | Structural conditions          | draft |
   | 3 | Section  | [compact](src/03-compact.md)        | Six components of the compact  | draft |
   | – | Bibliography | [refs](src/refs.md)             | References                     | draft |
   ```

3. **`03-inquiry-ai-agents/src/*.md`** — actual draft prose.

Once those are in place: `bin/build 03-inquiry-ai-agents` produces `<stem>.docx` for submission and `<stem>.pdf` for preview.

## Sanity test

The build was sanity-tested with a one-section stub on 2026-05-09; produced `inquiry-ai-agents-2026.docx` (3.5 KB) and `.pdf` (~70 KB) cleanly. A second sanity-test pass that evening with the full 12-segment paper-3 stub surfaced three real issues fixed in the same session: pandoc-native `[@key]` citations weren't picked up by `bin/refs emit` (the `CITE_RE` regex only matched `\cite{}`); the lualatex `\xmpquote` keywords-fatal had not in fact been suppressed by `--metadata=keywords:`; and the abstract was rendering twice (once from meta.md's YAML, once from the lifted file). All three are addressed in the conventions described above. To re-run: drop a `meta.md`, an `OUT.test.md`, and a `src/01-stub.md` into a paper-dir and run `bin/build`.

## Known limitations

- **Pandoc's DOCX writer doesn't emit reference styles automatically.** The `--citeproc` + Chicago-CSL combination renders citations correctly, but the bibliography in DOCX uses pandoc's default style. T&F's editorial side will reformat at production; for review the rendered Chicago author-date form is what matters.
- **British -ise spelling is not enforced by the build.** Pandoc respects `lang: en-GB` for hyphenation and locale-sensitive smart-quotes, but `organise/organize` selection is author discipline. Add to the pre-submission checklist.
- **AI-disclosure verification.** The build does not check for the presence of an AI-disclosure subsection. Drafter discipline; documented in `03-inquiry-ai-agents/planning/inquiry-submission-guidelines.md`.
