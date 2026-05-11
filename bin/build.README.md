# bin/build — what's wired, what's stubbed

*Minimum-viable port of the NeurIPS build pipeline (`~/src/neurips/bin/build`) for the synthese-paper portfolio. Done 2026-05-09 against the Inquiry/T&F submission target; extended significantly 2026-05-10. Companion files: `bin/build` (the script), `bin/refs` (citation data layer). For venue-side rationale see `03-inquiry-ai-agents/planning/inquiry-submission-guidelines.md`.*

## What it does

Reads a paper-dir (e.g., `03-inquiry-ai-agents/`) containing:

- `meta.md` — YAML frontmatter (`title`, `keywords`, `lang`). **Note:** abstract and author details are no longer in `meta.md`; they live as styled body segments in `src/` (see Conventions below).
- `OUT.<stem>.md` — markdown table whose rows enumerate segments under `<paper-dir>/src/`. Same shape as the NeurIPS pipeline so existing OUT manifests are portable.
- `src/*.md` — the actual segments. `[@key]`, `[-@key]`, `[@k1; @k2, p. 5]`, bare in-text `@key` pandoc citation forms all work; pandoc citeproc resolves them at render.

Produces (by default, **both** anon and non-anon builds in a single invocation):

- `<paper-dir>/<stem>.docx` — primary submission artifact (Word; T&F/Inquiry format).
- `<paper-dir>/<stem>.pdf` — camera-ready-style preview (lualatex; not for submission).
- `<paper-dir>/<stem>.md` — assembled markdown (human-readable; greppable; useful for word counts and full-paper review without opening Word).
- `<paper-dir>/<stem>-anon.{docx,pdf,md}` — the same three outputs with all author-identifying content stripped.
- `<paper-dir>/.build/<stem>/` — intermediates and bib (debug).

Citations: T&F house style is **Chicago author-date**. Build looks for `chicago-author-date.csl` (system texlive copy) and passes it to pandoc `--citeproc`. Falls back to pandoc's bundled default if not found.

## Invocation

```bash
# Default: build BOTH anon and non-anon versions
bin/build 03-inquiry-ai-agents inquiry-ai-agents-2026
bin/build 03-inquiry-ai-agents       # all OUT.*.md manifests in the paper-dir
bin/build                             # cwd must be a paper-dir

# Flags
bin/build 03-inquiry-ai-agents inquiry-ai-agents-2026 --no-anon    # non-anon only
bin/build 03-inquiry-ai-agents inquiry-ai-agents-2026 --anon       # anon only
bin/build 03-inquiry-ai-agents inquiry-ai-agents-2026 --just-anon  # alias for --anon
```

## Anonymisation system

The build has a two-tier anonymisation filter applied before each segment reaches pandoc.

**Tier A — global substitutions** (in `refs/deny-list.yml` under `substitutions:`): plain-string replacements applied in anon mode only. Currently wired for self-citations and contact details:
```yaml
substitutions:
  - from: "Wecker, in preparation"
    to:   "Author, in preparation"
  - from: "Wecker, in review, 2026"
    to:   "Author, in review, 2026"
  - from: "joseph.wecker@v2.io"
    to:   "[email withheld for review]"
```

**Tier B — inline/block markers** (in source `.md` files): HTML comments that pandoc passes through harmlessly when the filter hasn't been applied, so sources read cleanly as plain markdown.

| Marker | Anon mode | Non-anon mode |
|---|---|---|
| `<!--ANON: replacement -->original<!--/ANON-->` | → `replacement` | → `original` |
| `<!--DEANON_ONLY-->block<!--/DEANON_ONLY-->` | stripped entirely | content kept, markers stripped |

**Format markers** (applied per output format, independent of anon mode):

| Marker | PDF build | DOCX build |
|---|---|---|
| `<!--PDF_ONLY-->block<!--/PDF_ONLY-->` | content kept | stripped entirely |
| `<!--DOCX_ONLY-->block<!--/DOCX_ONLY-->` | stripped entirely | content kept |

Use `PDF_ONLY` for raw LaTeX (`{=latex}` fenced blocks), review notices, `\newpage` commands. Use `DOCX_ONLY` for raw OpenXML (`{=openxml}` fenced blocks) and DOCX-specific structural content (e.g. the `{custom-style="Article title"}` page-2 title restatement in the T&F two-page layout).

The YAML frontmatter author field is stripped automatically in anon mode (no marker needed).

## Title-page and front-matter layout

Author details, abstract, and keywords are **body content**, not YAML metadata. This is necessary for correct T&F ordering — YAML forces abstract before body content, making it impossible to place author info between author and abstract using the YAML approach.

The front-matter segments in `src/`:
- `00-author-details.md` — author name, affiliation, email, ORCID, page break, and article title restatement. Entire file is `DEANON_ONLY`. Page break and title restatement use `PDF_ONLY`/`DOCX_ONLY` markers since the two output formats need different commands.
- `00-abstract.md` — abstract text (in `{custom-style="Abstract"}` fenced div) and keywords line (in `{custom-style="Keywords"}`). In PDF, wrapped in `PDF_ONLY` `\begin{quote}\small`…`\end{quote}` for bilateral indentation and 10pt text.
- `00-toc.md` — table of contents, PDF only (`PDF_ONLY` raw `\tableofcontents`, `tocdepth=1`), placed between abstract and §1.

**Deanon PDF layout:** Title (YAML) → Author → Affiliation → Correspondence/ORCID → notice + `\newpage` → Abstract (indented, small) → Keywords → ToC → §1 body

**Anon PDF layout:** Title (YAML) → Abstract (indented, small) → Keywords → ToC → §1 body

**Deanon DOCX layout:** Title (YAML "Title" style) → Author → Affiliation → Correspondence → `<w:br type="page"/>` → Title (repeated, "Article title" style) → Abstract → Keywords → §1 body

**Anon DOCX layout:** Title → Abstract → Keywords → §1 body

## DOCX styling via reference doc

Pandoc reads named styles from `common/reference.docx`. Precedence: `<paper-dir>/reference.docx` → `common/reference.docx` → pandoc defaults. The build prints `(docx styled from <path>)` after success.

`common/reference.docx` is T&F's generic Word template (`TF_Template_Word_Windows_2016.dotx`). Four pandoc-named styles were added programmatically (2026-05-10) to match T&F's equivalents:

| Pandoc style | T&F style | Status |
|---|---|---|
| `Heading 1`–`Heading 4` | `heading 1`–`heading 4` | ✓ matched by name |
| `Abstract` | `Abstract` | ✓ matched by name |
| `Keywords` | `Keywords` | ✓ matched by name |
| `Footnote Text` / `Footnote Reference` | `footnote text` / `footnote reference` | ✓ matched by name |
| `Title` | `Article title` | ✓ added to reference.docx (14pt bold, 1.5×) |
| `Author` | `Author names` | ✓ added to reference.docx (14pt, 1.5×) |
| `Block Text` | `Displayed quotation` | ✓ added to reference.docx (indented, 11pt) |
| `Bibliography` | `References` | ✓ added to reference.docx (hanging indent) |

T&F custom styles (`Affiliation`, `Correspondence details`, `Article title`) are applied directly via `{custom-style="..."}` fenced divs in source segments — pandoc's DOCX writer passes these through verbatim.

## PDF preview styling

The PDF preview uses lualatex with camera-ready-style settings (not review-style double spacing):

- **Font**: TeX Gyre Pagella (Palatino-style; falls back to Latin Modern if absent)
- **Line spacing**: 1.1× (near single-spaced; readable without review bloat)
- **Margins**: 1.25in
- **Paragraphs**: indented (journal convention)
- **Links**: colored (NavyBlue for citations, URLs, cross-refs)
- **Font size**: 11pt body; abstract/keywords in 10pt (`\small`) via `quote` environment

The PDF is for self-review only — not for submission. DOCX is the T&F submission format.

## Conventions worth knowing

**Self-citations.** "In preparation" and "in review" companion works are cited as plain text `(Wecker, in preparation)` / `(Wecker, in review, 2026)` — not as pandoc `[@key]` citations — because there are no stable bib entries to point to. They appear in footnotes rather than inline. The anon filter substitutes `Author` for `Wecker` in these strings; the substitutions are in `refs/deny-list.yml`.

**Two intermediates per build.** The body is assembled once and written into both `<stem>.md` (full frontmatter, for DOCX) and `<stem>.pdf-preview.md` (keywords stripped, for PDF). The `PDF_ONLY`/`DOCX_ONLY` filter pass runs separately in each `write_intermediate` call. The keywords-strip exists because pandoc's LaTeX template threads `keywords:` through hyperxmp's `\xmpquote{}` macro and lualatex fatals on it; stripping at YAML-assembly time is the clean fix.

**Manifest slug `abstract` is no longer special.** Earlier versions of the build lifted a row with slug `abstract` into the YAML `abstract:` metadata field. That mechanism is no longer used — the abstract is body content. The current abstract row in `OUT.inquiry-ai-agents-2026.md` uses slug `abstract-body` to make this explicit. The `lift_abstract` code path still exists but is dormant.

**DOCX bibliography styling.** `--citeproc` + Chicago-CSL renders citations correctly in body text and footnotes; the bibliography block uses pandoc's `Bibliography` style (now mapped to T&F's `References` via the reference.docx addition). T&F editorial will reformat at production; Chicago author-date is what matters for review.

## Wiring summary

| Concern | NeurIPS pipeline | This pipeline |
|---|---|---|
| Manifest format (`OUT.*.md` table) | Wired | **Wired (verbatim port)** |
| `meta.md` YAML frontmatter | Wired | **Wired (`title`, `keywords`, `lang` only; abstract/authors in body)** |
| `bin/refs emit` shell-out | Wired | **Wired (same contract)** |
| Anonymisation lint at build | Wired | **Wired (deny-list scan; hard gate is `bin/refs lint` separately)** |
| Anonymisation filter | N/A (single-blind) | **Wired (`--anon`/`--no-anon`/`--just-anon`; default builds both)** |
| Format markers | N/A | **Wired (`PDF_ONLY`, `DOCX_ONLY`, `DEANON_ONLY`, `ANON:`)** |
| Markdown → output | LaTeX (kramdown, theorem envs, callouts) | **DOCX + PDF via pandoc** |
| Citation rendering | natbib super-numeric | **Chicago author-date via pandoc citeproc** |
| Build-output target | `.pdf` (camera-ready) | `.docx` (submission) + `.pdf` (preview) |
| DOCX style mapping | N/A | **Wired (4 pandoc-named styles added to `common/reference.docx`)** |

## What's stubbed / not ported (and why)

- **Obsidian-callout system** (`> [!theorem]` etc.). Not load-bearing for analytical-philosophy prose. Port from `~/src/neurips/bin/build:75-480` if needed.
- **`[[#^anchor]]` cross-references.** NeurIPS/Obsidian convention; pandoc's own `[ref]{#anchor}` works for any cross-refs this paper needs.
- **Equation anchors / cleveref machinery.** N/A for analytical philosophy.
- **`<stem>.prior.pdf` snapshot.** Skipped — DOCX is submission; PDF is preview; git history is the rollback.
- **Page-budget side-tool.** N/A; Inquiry has no word limit.

## What's deliberately NOT ported: LaTeX target

T&F provides Word templates for *Inquiry*, not a LaTeX class. DOCX is the submission target. If a future paper at a LaTeX-friendly venue (Synthese paper 1 at Springer) needs a LaTeX build, the cleanest approach is a separate `bin/build-springer` rather than overloading this script.

## Known limitations

- **British -ise spelling not enforced.** Pandoc respects `lang: en-GB` for hyphenation and smart-quotes; `-ise`/`-ize` selection is author discipline.
- **AI-disclosure verification.** Build does not check for an AI-disclosure subsection. Documented in `03-inquiry-ai-agents/planning/inquiry-submission-guidelines.md`.
- **κ (U+03BA) glyph missing in PDF preview.** TeX Gyre Pagella does not include κ; lualatex warns and substitutes. Affects one occurrence in `05-operationalization.md` ("κ-processing measurements"). Non-fatal for preview; irrelevant for DOCX.
