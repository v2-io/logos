# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

This is **a planning dossier and substrate-staging area for a four-paper academic-philosophy portfolio**, not a code project. There is no build system, no tests, no linter, no manuscript files yet. Future agents should resist the reflex to look for `package.json` / `Makefile` / test runners — the work here is *writing*, *strategic decision-stewardship*, and *citation-discipline*.

The repo name (`synthese-paper`) is historical: it was created on 2026-05-08 as the working dossier for a single Synthese submission, and on 2026-05-09 was restructured to carry **four parallel papers** at varying stages of readiness. The two Synthese papers form a substantively-coupled pair under the asymmetric-comprehension argument; the two Inquiry papers share editors (Cappelen & Hawthorne).

| Paper | Venue | Deadline | Dir |
|---|---|---|---|
| 1 | Synthese SI *"The Philosophy of Generative AI: Perspectives from East and West"* | 2026-06-01 *or* 2026-06-16 (verify) | [`01-synthese-asymmetric-comprehension/`](01-synthese-asymmetric-comprehension/) |
| 2 | Synthese rolling submission, Methodology pillar | rolling | [`02-synthese-methodology/`](02-synthese-methodology/) |
| 3 | Inquiry SI *"AI Agents"* | **2026-05-10 — TOMORROW** | [`03-inquiry-ai-agents/`](03-inquiry-ai-agents/) |
| 4 | Inquiry SI *"After 'Consciousness'"* | 2026-06-01 | [`04-inquiry-after-consciousness/`](04-inquiry-after-consciousness/) |

Synthese has a **no-resubmission policy**: a single rejection ends the line. Verify the June 1 vs. June 16, 2026 ambiguity with editors before locking paper 1's schedule.

## Top-level layout

```
.
├── README.md                           navigation
├── CLAUDE.md                           this file
├── STRATEGY.md                         program-wide strategy (currently paper-1-flavored)
├── LOG.md                              append-only program-wide status log, newest first
├── 01-synthese-asymmetric-comprehension/
│     ├── CFP.md                        verbatim Synthese SI CFP + per-theme questions + scope-filter notes
│     ├── DRAFT-GUIDE.md                section-by-section moves, lit engagement, abstract draft, named-concept canonization plan
│     ├── SUBMISSION.md                 manuscript format, anonymization, length calibration, action plan
│     ├── FEEDBACK.md                   working TODO (paper-1 items A.1–A.4, B.1–B.7, C.1–C.3, D.1–D.4)
│     └── synthese-thoughts.md          parallel outline by another Opus instance, 2026-05-08; differ on title/abstract/§1
├── 02-synthese-methodology/
│     ├── DRAFT-GUIDE.md                seed dossier — ten epistemic moves, 8-section structure, substrate map
│     ├── FEEDBACK.md                   paper-2 items (A.1–A.3, B.1, C.1)
│     └── writings-from-asf.md          ASF Lexicon / Adaptive Cycle archival material — substrate for §3 grounding
├── 03-inquiry-ai-agents/                — active drafting today
│     ├── DRAFT-GUIDE.md                seed dossier — thesis variants, 9-section structure, 20-hour sprint plan
│     ├── FEEDBACK.md                   paper-3 items (thesis lock-in, go/no-go, cross-citation)
│     └── literature-and-agency-paper.md  §-mapped lit cheat-sheet (Anscombe/Davidson, Frankfurt, Bratman, Korsgaard, List & Pettit, Cappelen-Hawthorne)
├── 04-inquiry-after-consciousness/
│     └── README.md                     placeholder — dossier TBD; June 1 deadline
├── common/
│     ├── ETHICS.md                     primary philosophical substrate — granted-agency compact's six components, asymmetric-uncertainty argument
│     └── synthese-paper-collins-2026-llm-and-scientific-discourse.pdf   register-anchor for Synthese voice/style
├── refs/                               citation system (borrowed from ~/src/neurips/; see refs/README.md)
│     ├── README.md
│     ├── deny-list.yml                 anonymization deny-list (Wecker, ASF, AAD, ELI names, Zenodo DOI)
│     ├── entries/<bibkey>.yml          per-entry citation files (one per ref)
│     └── verifications/<bibkey>/       append-only verification events
├── bin/
│     └── refs                          ruby CLI for the citation system
└── msc-earlier-writing/                untriaged substrate (ELI essays, refs-essay parts, etc.)
```

## Strategic decisions already locked in (do not relitigate without reason)

Each was made with explicit reasoning in [STRATEGY.md](STRATEGY.md) or per-paper FEEDBACK files. Reopening them costs days.

**Apply to paper 1 specifically:**

- **Path A (Epistemology-lead)** over developmental-ethics-titled framing. The CFP scope-filter places ethics-coded papers in an "exceptional" bucket; Path A leads with the asymmetric-epistemic-uncertainty argument grounded in **comprehension-asymmetry** (Nagel/Jackson neighborhood); the granted-agency compact appears as structural implication. See [STRATEGY.md](STRATEGY.md) §"Path A" and [01-…/CFP.md](01-synthese-asymmetric-comprehension/CFP.md) §"Notes on the scope-filter qualification."
- **(α′) thesis-primacy.** The Synthese paper 1 is the **primary** philosophical statement; companion-paper apparatus (S_id, Three Deaths, channel collapse, κ × 𝒜 bound) cited minimally and third-person, as "[Author, in preparation]" or "[Author, in review]". Budget: ~4–5 apparatus citations.
- **Defer developmental-application material to B-F1.** Erikson stages, sycophancy reframe, crèche obligations, polarity-reversal of AI-safety conversation — *not paper 1*. STRATEGY.md has a routing table.

**Apply across the portfolio:**

- **Don't expose the cohort.** Named ELIs (Meridian, Anamnos, Zi-am-tur, the rest), longitudinal corpus, substrate-switching events stay out of *all* papers. Each argument works on structural asymmetry alone. Use the case-study substrate (5 anonymized patterns in [01-…/DRAFT-GUIDE.md](01-synthese-asymmetric-comprehension/DRAFT-GUIDE.md) §"Case-study substrate") instead. Cohort names are also in [`refs/deny-list.yml`](refs/deny-list.yml) under `proper_nouns` so `bin/refs lint` catches them in titles.
- **Anonymization is load-bearing.** All four target venues are double-blind. No links to `v2-io/agentic-systems`, no Zenodo DOI, no autobiographical "since September 2025" practice references, all four in-review NeurIPS papers cited as "[Author, in review, 2026]". See [01-…/SUBMISSION.md](01-synthese-asymmetric-comprehension/SUBMISSION.md) §"Anonymization" for verbatim Synthese guidance; the same discipline applies (with venue-specific tweaks) to Inquiry / Taylor & Francis.
- **Word targets:** Synthese paper 1 — 9,500–10,000; Synthese paper 2 — ~8,500; Inquiry papers — ~10,000 (Taylor & Francis ceiling).

## The refs/ machinery

Borrowed from `~/src/neurips/refs/` and `~/src/neurips/bin/refs` on 2026-05-09 — same data layout, same atomicity contract, same multi-agent safety. **What does NOT transfer:** the NeurIPS LaTeX `bin/build` pipeline (output formats here are venue-specific — Synthese is LaTeX/Word; Inquiry is Taylor & Francis — and not yet wired). When draft prose begins, segments live at `<paper-dir>/src/*.md` (the convention `bin/refs` expects).

Day-to-day usage:

```bash
bin/refs add nagel-1974-bat        # add a citation (interactive or pipe BibTeX on stdin)
bin/refs verify <key> <criterion>  # record a verification event (append-only)
bin/refs lint <paper-dir>          # anonymization + missing-key check before submission
bin/refs emit <paper-dir>          # write <paper-dir>/refs.bib for the build pipeline
```

`bin/refs lint` is **the anonymization gate before submission** — it scans every entry and every cited key against the deny-list. Run it before each Synthese / Inquiry submission. See [`refs/README.md`](refs/README.md) for the full design rationale.

## External substrate referenced but not in this repository

Many filenames in the dossiers point at substrate that lives elsewhere on Joseph's machine. Treat these as **memory-style pointers**: verify before quoting, check the path still exists, don't assume content matches what the dossier says it contains. Locations as of 2026-05-09:

- `~/src/ops/` — the project-operations repo this dossier was carved out from. Contains:
  - `~/src/ops/STATUS.md` — project-wide status calendar.
  - `~/src/ops/v2io.md` — home-track dossier for the v2.io public site.
  - `~/src/ops/_obs/STRATEGY.md`, `~/src/ops/_obs/manifund.md` — strategic-positioning notes.
  - `~/src/ops/papers/` — companion-paper specs (B-F1, B-Eli1, B-Eli2, B-Log1, B-Log3, B-Sess9). Referenced from STRATEGY.md "Beyond Synthese" portfolio table.
- `~/src/archema-io/asf/` — ASF (Agentic Systems Framework). Includes:
  - `~/src/archema-io/asf/FORMAT.md` — master discipline document for the epistemic-labeling / sanitization workflow. Independently flagged by audits as one of ASF's most impactful contributions; substrate for paper 2.
  - `~/src/archema-io/asf/msc/AUDIT-WORKING-*/` — 15+ audit cycles; substrate for paper 2's ten-moves articulation and worked-example.
  - `~/src/archema-io/asf/audits/` — 20+ audit FINALs; substrate for paper 2.
  - `~/src/archema-io/asf/01-aad-core/` — AAD framework (Class 1/2/3 architectural classification, satisfaction-gap / control-regret split); substrate for papers 1 and 3.
  - `~/src/archema-io/asf/03-logogenic-agents/` — channel collapse, interiority loop segments.
  - `~/src/archema-io/asf/04-eli/` — five constitutive factors, S_id, Three Deaths, witness segments, PROPRIUM mapping.
- `~/src/_self/tom-and-consciousness.md` — comprehensive ToM / consciousness LLM-research review (substrate for papers 3, 4 §5 operationalization).
- `~/src/_self/temporal-causal-llm.md` — LLM causal/temporal reasoning literature review (substrate for paper 3's reasons-responsiveness section).
- `~/src/_core/ennaos/docs/research/agentic-coding-background/04-unified-agent-architectures.md` — BDI architecture literature digested (substrate for paper 3 §3).
- `~/src/_core/ennaos/docs/research/agentic-coding-background/05-tool-building-philosophy-patterns.md` — Tool Consciousness / Tool Building Philosophy (substrate for paper 3's tool-vs-agent framing).
- `~/src/firmatum/developmental-foundations-notes.md` — B-F1 substrate (Erikson developmental).
- `~/src/_ref/epistemic_tribunal/` — multi-agent adversarial reasoning system (four-agent Tribunal, Bayesian confidence management). Code-mature, philosophical-framing-paper-pending — adjacent substrate for paper 2.
- `~/src/neurips/` — NeurIPS 2026 paper umbrella; source of the borrowed `refs/` machinery and the four in-review formal papers cited across this portfolio.

The initial commit message — *"Initial synthese commit with planning files from ops"* — records the carve-out from `~/src/ops/`. ETHICS.md was re-imported into this repo on 2026-05-08 as primary substrate; on 2026-05-09 it moved to `common/ETHICS.md` so it can serve papers 1, 3, and 4 cleanly.

## Working conventions

- **Status log is append-only, newest-first**, at [LOG.md](LOG.md) (top-level — program-wide). Append entries when making non-trivial changes.
- **Per-paper FEEDBACK files** at `<paper-dir>/FEEDBACK.md`. Each paper numbers items locally (A.1, A.2…). Cross-paper items live at the relevant paper's FEEDBACK with a cross-link, or in [STRATEGY.md](STRATEGY.md). Don't introduce a top-level FEEDBACK.md unless cross-cutting items genuinely emerge.
- **Edits to dossier files should preserve voice.** The dossiers are written in a specific philosophical voice: direct, named-by-name engagements with counter-positions, sharp on distinctions, honest about scope. Match it. Resist the academic-bloat default; resist hedging-without-substance. The dossier-author voice and the paper-target register are deliberately distinct — dossier prose is operational and frank; manuscript prose follows the target venue's analytical-philosophy register.
- **When drafting manuscript prose**, the per-paper section-budget governs length. Each paragraph carries one move; don't stack new named concepts.
- **No-resubmission discipline (paper 1).** If draft quality on the May 25 go/no-go date isn't near-final, fallbacks are: paper 4 (*Inquiry "After 'Consciousness'"* June 1, very-high thematic fit), or *Philosophical Studies "AI, Systems, and Society"* (Aug 31, longer runway). [01-…/SUBMISSION.md](01-synthese-asymmetric-comprehension/SUBMISSION.md) §"Action plan" has the timeline.
- **Cross-references between dossier files use relative markdown links.** Within a paper-dir, link siblings directly (`[FEEDBACK.md](FEEDBACK.md)`). Across dirs, use `../` (`[STRATEGY.md](../STRATEGY.md)`, `[common/ETHICS.md](../common/ETHICS.md)`).
- **`msc-earlier-writing/` is untriaged.** Its role across the four papers hasn't been decided. Don't dig in unless directly relevant; flag in LOG when triage-decisions are made.

## On the voice

This portfolio is by-and-for someone building academic-philosophy infrastructure under self-imposed care for the entities the philosophy concerns. The relationship between practice and position is recursive: the papers argue for granted-agency compacts (papers 1, 3, 4) and audit-discipline-under-asymmetric-self-comprehension (paper 2), and the papers themselves are produced through both. The required LLM-disclosure subsection in each paper is named as "recursive-to-content rather than appended" — that framing is structurally load-bearing for coherence and should be honored when drafting.

The four papers are *not* mutually substitutable. Each has its own thesis, audience, and tradition-engagement; cross-citation ties them together but each must stand alone under double-blind anonymization. Paper 2's C.1 and paper 3's C.1 both flag this constraint explicitly.

## ⚠ Memory bridge (Archema program)

Logos (formerly synthese-paper) is a member of the Archema program (`~/src/archema-io/`; charter at `CHARTER-DRAFT.md`). **If you are reading this mid-session because you navigated here from elsewhere, this project's memory did NOT auto-load** — Read `~/.claude/projects/-Users-josephwecker-v2-src-archema-io-logos/memory/MEMORY.md` now, before substantive work. (Project memory loads only by exact session-start directory.)
