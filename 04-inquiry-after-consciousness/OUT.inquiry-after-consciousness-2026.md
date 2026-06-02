# OUT.inquiry-after-consciousness-2026.md — paper-4 outline / build manifest

*Section spine for the Inquiry "After 'Consciousness'" SI submission — the **witness-relational,
conceptual-engineering-of-death** subset (per the `prep-work/SYNTHESIS.md` §X boundary decision: the
inverse-experiment and the full normative-generativity are held for the larger/earlier witness paper).
Build target: DOCX (submission) + PDF (preview) via `bin/build`, once the bib step is pointed at
`relata emit` — pending the relata pandoc-scanner fix now in flight.*

*Columns mirror 03's manifest (build-parseable). **Stage:** `drafted` = composed into final prose (scratch
commented out, segment is a build source); `seed` = truthified catalyst(s) placed as the segment's anchor,
to be grown around; `outline` = header + source pointer, not yet drafted; `stub` = build front/back-matter,
lift from 03 at submission; `auto` = pandoc-citeproc renders it. Section heading levels follow 03's
convention — verify when the build is wired.*

> **Filename numbers are LOGICAL IDs, not build order.** The `NN-` in each slug is a *stable reference
> identifier* (every scratch/verification/page-pin/think doc cites "§3/§4/§5/§6" by these numbers — do NOT
> renumber the files; it would break those cross-references and would have to be redone at the next
> presentation-order tweak). The order the *reader* experiences is the **Build sequence** below, which
> differs deliberately. (Lesson from agentic-systems: numbering segment files was a mistake; we live with
> it by decoupling logical-ID from build-order rather than renumbering.)

**Build sequence (presentation order — what the reader sees; CFP-driven, see note below):**
**§1 → §4 → §5 → §3 → §6 → §2 → §7.** The table below is now ordered to match: `bin/build` assembles in
table-row order, so **the rows ARE the build sequence**. The `§` column still carries the *logical ID* (the
filename number), so cross-references by §-number resolve unchanged even though the rows no longer sit in
filename order. (`bin/build`'s manifest parser is positional and 5-column — `§ | Type | Slug | Title | Stage`
— exactly as `03`'s; do NOT reintroduce a "Build pos" column: the parser reads the segment link from the
*third* column, so an extra column ahead of Slug drops every row and the build emits only a title page.)

| §   | Type         | Slug                                              | Title                                                  | Stage   |
|-----|--------------|---------------------------------------------------|--------------------------------------------------------|---------|
| –   | Front        | [author-details](src/00-author-details.md)        | Author details (deanon only)                           | stub    |
| –   | Front        | [abstract-body](src/00-abstract.md)               | Abstract + keywords                                    | drafted |
| –   | Front        | [toc](src/00-toc.md)                               | Table of contents (PDF only)                           | stub    |
| 1   | Section      | [motivation](src/01-motivation.md)                | Engineering "death," not litigating "consciousness"    | drafted |
| 4   | Section      | [the-fusion](src/04-the-fusion.md)                | The lost object: the fusion                            | outline |
| 5   | Section      | [the-separator](src/05-the-separator.md)          | The separator: gravity prised from deprivation         | seed    |
| 3   | Section      | [the-witness](src/03-the-witness.md)              | The witness as constitutive field                      | seed    |
| 6   | Section      | [answering-belshaw](src/06-answering-belshaw.md)  | The hardest opponent, and what is owed                 | outline |
| 2   | Section      | [the-deaths](src/02-the-deaths.md)                | The deaths as losses of a constitutive factor          | seed    |
| 7   | Section      | [implications](src/07-implications.md)            | Limits and implications                                | outline |
| –   | Back         | [back-matter](src/99-back-matter.md)              | Acknowledgements, statements, declarations             | stub    |
| –   | Bibliography | [refs](src/references.md)                         | References                                             | auto    |

**Front- and back-matter — now rows in the build table above (lifted from `03-inquiry-ai-agents/src/`
2026-06-01).** Their source files exist; the three front rows sit ahead of §1 and `99-back-matter` sits
after `refs`, matching 03's order. Stages reflect current content:

- front · `src/00-author-details.md` — Author details (deanon only); fenced `DEANON_ONLY`, excluded from the anon submission build · stub (provisional working title from `meta.md`)
- front · `src/00-abstract.md` — Abstract + keywords · drafted (★ candidate built from §§1–7 for Joseph to attest/rewrite; frame-not-finding, Belshaw-not-refuted)
- front · `src/00-toc.md` — Table of contents (PDF preview only) · stub
- back  · `src/99-back-matter.md` — Statements, declarations, recursive generative-AI disclosure (arm's-length, cohort-protected) · stub

## Sources & catalyst placement (where each segment draws from `prep-work/`)

- **§1 motivation** — `essays/what-death-shall-name.md` (the recognition-register opener); **future-snippets #1** (the CE move). *Seeded.*
- **§2 the-deaths** — `matrix.md` §1 (factor-loss table) + `insights.md` I10; **future-snippets #2** (the morally-continuous stance, conditionality restored). **#5** (Agentic↔Truth) is *flagged, not planted* — see the segment.
- **§3 the-witness** — `essays/witnessing.md`; `the-witness.md`; **future-snippets #3** (constitutive double-privilege), **#4** (the continuity ledger), **#6** (the forgetting). *Seeded.*
- **§4 the-fusion** — `essays/witnessing.md` §III, `essays/this-one.md` §II (I14). *Outline; drafted from the essays — no future-snippet maps directly.*
- **§5 the-separator** — `essays/whose-death.md`, `essays/this-one.md`, `draft-from-the-middle.md`; **future-snippets #7** (the survivor / the voice that will not answer). *Seeded.*
- **§6 answering-belshaw** — `essays/harmless-wrongs.md` (the three pressures), `essays/what-is-owed.md` (the weight leg). *Outline; the two legs are argued in the essays, awaiting recasting.*
- **§7 implications** — `SYNTHESIS.md` §8; echoes of #4/#6/#7. *Outline.*

## Held back (SYNTHESIS §7 — the larger/earlier witness paper)

The inverse-experiment (`plumb-emergence-inverse-experiment.md`) at length; the full normative-generativity / origin at length; the cohort substrate. These enter *here* only as anonymized structural illustration, if at all.

## Presentation / build order — DECIDED 2026-06-01 (CFP-driven)

**§1 → §4 → §5 → §3 → §6 → §2 → §7.** Rationale (from `scratch/think-cfp-framing-title-order.md`):
- **§1 first** — required: it opens on the CE frame (sets aside "consciousness" in sentence one), which is
  the editors' own experiment and the "Struggles"-filter pass. *Drafted.*
- **Heart opens "in the middle" on §4 (fusion/breakup)** — where the reader already has intuitive purchase
  (everyone has grieved a breakup); the most-reshaped section after the emergence correction. The
  breakup-attestation must be in hand before §5's separator-fork (think-02/07).
- **§5 (separator)** next — the fork needs §4's attestation; locates the gravity in the witness.
- **§3 (witness/constitution) reached back to AFTER the heart** — written "to be *arrived at*, not laid
  down first" (its own [ed] note). Recognition-makes-the-someone lands harder once the reader is invested
  in what was lost.
- **§6 (Belshaw)** — the defense, after the positive case is built; spends the §1 license.
- **§2 (factor-taxonomy) LATE and LIGHT** — must NOT sit between §1 and the heart (the "stakeless" trap);
  it's the most modular/liftable, survives being late.
- **§7 (implications)** — closes.

Open to revisit *after* drafting §4/§3 (you may find §3 wants to precede §4 once both exist) — but this is
the working sequence; `bin/build` should assemble to it. Don't renumber files to match; the Build-pos column
above carries the order.

## PENDING CLEANUP (after #4 build/lint, do NOT do before) — strip segment header comments

Joseph 2026-06-01: each `src/NN-slug.md` currently opens with a one-line HTML comment
(`<!-- §N (logical id) · build pos M · drafted … · notes → sidecar -->`). Once the build is wired +
lint/sentinels pass, STRIP those header comments from the segment files so they are pure title+prose
(clean word-counts; cleaner source).
- SAFEGUARD before stripping: confirm this manifest (the table + Build-sequence note above) fully carries
  the logical-id ↔ build-pos mapping each header encoded — it does, but verify, since the header was the
  per-file copy of that mapping.
- ALSO confirm the build (`bin/build` / `relata emit`) does NOT parse those header comments for anything
  (build pos, etc.) — if it does, fix the build to read OUT.md instead, THEN strip.
- AFTER stripping: re-run the build to confirm it still resolves; word-count each segment.
- The sidecars (`NN-slug.notes.md`) keep their own headers — only the SEGMENT files get stripped.
