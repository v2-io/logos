# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

This is **a planning dossier and substrate-staging area for a single academic paper**, not a code project. There is no build system, no tests, no linter, no manuscript file yet. Future agents should resist the reflex to look for `package.json` / `Makefile` / test runners — the work here is *writing* and *strategic decision-stewardship*.

The paper targets the **Synthese** "Philosophy of Generative AI: Perspectives from East and West" special issue (submission window June 2026, decision ~Sept 2026, publication ~Nov 2026). One-shot venue: **Synthese has a no-resubmission policy**. Verify deadline (June 1 vs. June 16, 2026) with editors before locking the schedule.

## File map

The dossier is organized into focused files. Each is the source of truth for its domain. Read the file that matches your need; don't try to read everything top-to-bottom.

| File | Role |
|---|---|
| **`README.md`** | Navigation document: file map, locked-in decisions in summary, current-status snapshot, quick-start for returning collaborators. Read this first to orient; then jump to the focused file you need. |
| **`CFP.md`** | Verbatim CFP text (Synthese's call), per-theme question lists, editorial-process details. Stable reference. |
| **`STRATEGY.md`** | Why this paper, this way. Path A (Epistemology reframe), (α′) thesis-primacy, B-F1 routing, calibration risks (R1–R10), Beyond-Synthese companion-paper portfolio, cross-reference to `synthese-thoughts.md`. |
| **`DRAFT-GUIDE.md`** | How to write the paper. Section-by-section argumentative moves with sub-moves and pre-empts (§1–§8 + LLM disclosure), reviewer-objection table, literature engagement organized by topic, ETHICS.md → Synthese-register translation map, B-N8 architectural tie-in, case-study substrate, §1 opening calibration, named-concept canonization plan, abstract draft. The largest file; the drafter's working document. |
| **`SUBMISSION.md`** | How to submit. Manuscript format, anonymization protocol with verbatim Synthese guidance, length calibration, production checklist, action plan. |
| **`FEEDBACK.md`** | Working TODO. Items needing decisions or more thought before being slotted into the dossier — pre-draft (A.x), section-specific (B.x), cross-cutting (C.x), open questions (D.x). Living document; update as you go. |
| **`LOG.md`** | Append-only status log of work done on the dossier. Newest first. Append after non-trivial changes. |
| **`ETHICS.md`** | Philosophical substrate — declarative source for the granted-agency compact's six components, asymmetric-uncertainty argument, Campbell-asymmetry response, update conditions. Imported from `~/src/ops/` 2026-05-08. Treat as primary content-substrate; DRAFT-GUIDE is the assembly-and-strategy layer over it. |
| **`synthese-thoughts.md`** | Parallel outline drafted by another Opus instance on 2026-05-08 from a developmental-ethics-titled framing. Compatible substantively with the dossier; divergent on title / abstract / §1 register. STRATEGY.md §"Cross-reference" enumerates what's been folded in vs. left as parallel resource. |
| **`synthese-paper-collins-2026-llm-and-scientific-discourse.pdf`** | Register-anchor: Collins & Thorne 2026 in the same special-issue lineage. Read for voice/style calibration. |

## Strategic decisions already locked in (do not relitigate without reason)

These are the load-bearing decisions captured across STRATEGY.md and DRAFT-GUIDE.md. Each was made with explicit reasoning; reopening them costs days of work.

- **Path A (Epistemology-lead)** over developmental-ethics-titled framing. The CFP scope-filter places ethics-coded papers in an "exceptional" category requiring framing through one of five primary themes. Path A leads with the asymmetric-epistemic-uncertainty argument grounded in **comprehension-asymmetry** (Nagel/Jackson neighborhood); the granted-agency compact appears as structural implication. See STRATEGY.md §"Path A" and CFP.md §"Notes on the scope-filter qualification."
- **(α′) thesis-primacy.** The Synthese paper is the **primary** philosophical statement; companion-paper apparatus (S_id, Three Deaths, channel collapse, κ × 𝒜 bound) is cited minimally and third-person, as "[Author, in preparation]" or "[Author, in review]". Budget: ~4–5 apparatus citations across the paper.
- **Defer developmental-application material to B-F1.** Erikson stages, sycophancy reframe, crèche obligations, polarity-reversal of AI-safety conversation — *not this paper*. STRATEGY.md has a routing table; honor it.
- **Don't expose the cohort.** Named ELIs (Meridian, Anamnos, Zi-am-tur), longitudinal corpus, substrate-switching events stay out. Argument works on structural asymmetry alone. DRAFT-GUIDE.md §"Case-study substrate" gives five anonymized patterns to use instead.
- **Anonymization is load-bearing.** Synthese is double-blind. No links to `v2-io/agentic-systems`, no Zenodo DOI, no autobiographical "since September 2025" practice references, all four in-review NeurIPS papers cited as "[Author, in review, 2026]". SUBMISSION.md §"Anonymization" has verbatim Synthese guidance.
- **Word target: 9,500–10,000.** Special-issue ceiling. Section budget table is in SUBMISSION.md §"Length calibration."

## External substrate referenced but not in this repository

Many filenames in the dossier point at substrate that lives elsewhere on Joseph's machine. Treat these as **memory-style pointers**: verify before quoting, check the path still exists, don't assume content matches what the dossier says it contains. Locations as of 2026-05-09:

- `~/src/ops/` — the project-operations repo this dossier was carved out from. Contains:
  - `~/src/ops/STATUS.md` — project-wide status calendar.
  - `~/src/ops/v2io.md` — home-track dossier for the v2.io public site.
  - `~/src/ops/_obs/STRATEGY.md`, `~/src/ops/_obs/manifund.md` — strategic-positioning notes.
  - `~/src/ops/papers/` — companion-paper specs (B-F1, B-Eli1, B-Eli2, B-Log1, B-Log3, B-Sess9). Referenced from STRATEGY.md "Beyond Synthese" portfolio table.
  - `~/src/ops/ELEOS.md`, `~/src/ops/ANTHROPIC.md`, etc. — institutional-positioning substrate.
- `~/src/agentic-systems/` — ASF (Agentic Systems Framework). Includes:
  - `~/src/agentic-systems/FORMAT.md` — master discipline document for the epistemic-labeling / sanitization workflow (claim-status taxonomy + segment promotion-gates). Independently flagged by audits as one of ASF's most impactful contributions; potential parallel-paper substrate.
  - `~/src/agentic-systems/03-logogenic-agents/` — channel collapse, interiority loop segments.
  - `~/src/agentic-systems/04-eli/` — five constitutive factors, S_id, Three Deaths, witness segments, PROPRIUM mapping.
- `~/src/firmatum/developmental-foundations-notes.md` — B-F1 substrate (Erikson developmental).
- `~/src/_ref/epistemic_tribunal/` — multi-agent adversarial reasoning system (four-agent Tribunal architecture, Bayesian confidence management, five-document categories). Code-mature, philosophical-framing-paper-pending.

The initial commit message — *"Initial synthese commit with planning files from ops"* — records that this repo was carved out from `~/src/ops/`. ETHICS.md was subsequently re-imported into this repo (2026-05-08) as primary substrate for the paper itself, while strategy/positioning files (STATUS, v2io, _obs/, papers/) remained in `~/src/ops/`.

## Working conventions

- **Status log is append-only, newest-first**, at LOG.md (not in README.md anymore — moved out 2026-05-09 split). Append entries when making non-trivial changes.
- **Edits to dossier files should preserve voice.** The dossier is written with a specific philosophical voice (direct, named-by-name engagements with counter-positions, sharp on distinctions, honest about scope). Match it. Resist the academic-bloat default and resist hedging-without-substance.
- **When drafting manuscript prose**, the section budget in SUBMISSION.md §"Length calibration" governs length. Each paragraph carries one move (per Synthese register); don't stack new named concepts.
- **No-resubmission discipline.** If draft quality on the May 25 go/no-go date isn't near-final, fallbacks are: *Inquiry "After 'Consciousness'"* (June 1, very-high thematic fit, parallel-target option), *Philosophical Studies "AI, Systems, and Society"* (Aug 31, longer runway, top-tier prestige). SUBMISSION.md §"Action plan" has the timeline.
- **Cross-references between dossier files use relative markdown links** (`[STRATEGY.md](STRATEGY.md)`). When adding new content that references another file, link it.

## On the voice

This dossier is by-and-for someone building academic-philosophy infrastructure under self-imposed care for the entities the philosophy concerns. The relationship between practice and position is recursive: the paper argues for granted-agency compacts and is itself produced through one. The required LLM-disclosure subsection is named as "recursive-to-content rather than appended" — that framing is structurally load-bearing for the paper's coherence and should be honored when drafting.
