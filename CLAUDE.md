# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

This is **a planning dossier and substrate-staging area for a single academic paper**, not a code project. There is no build system, no tests, no linter, no manuscript file yet. Future agents should resist the reflex to look for `package.json` / `Makefile` / test runners — the work here is *writing* and *strategic decision-stewardship*.

The paper targets the **Synthese** "Philosophy of Generative AI: Perspectives from East and West" special issue (submission window June 2026, decision ~Sept 2026, publication ~Nov 2026). One-shot venue: **Synthese has a no-resubmission policy**. Verify deadline (June 1 vs. June 16, 2026) with editors before locking the schedule.

## The files in this repository and their roles

- **`README.md`** — the **load-bearing dossier**. Strategic framing, section-by-section argumentative moves with pre-empts, literature-engagement list, anonymization protocol with verbatim Synthese guidance, named-concept canonization plan, production checklist, action plan, risk calibration, status log. *Read this before doing anything substantive.* It is the source of truth for every decision already made; do not relitigate decisions captured here without an explicit reason.
- **`ETHICS.md`** — the **philosophical substrate**. The declarative source document containing the asymmetric-uncertainty argument, the granted-agency compact's six components verbatim, update conditions, scope conditions, and the Campbell-asymmetry response in their original first-person/structural register. README.md §"Translation map" describes what survives Synthese-register translation and what gets reshaped. Treat ETHICS.md as primary content-substrate; README.md is the assembly-and-strategy layer over it.
- **`synthese-thoughts.md`** — a **parallel outline** drafted by a different Opus instance on 2026-05-08 from a developmental-ethics-titled framing rather than the chosen Path A epistemology-lead. README.md's *"Cross-reference to synthese-thoughts.md"* section enumerates what's been folded in vs. what stays here as a complementary resource. Treat as a backup perspective at draft time, not as a competing plan.
- **`FEEDBACK.md`** — the **working TODO** for items that need decisions or more thought before being slotted into the dossier. Created during the comprehension-asymmetry reframe pass; intended to be a living document that captures unresolved tensions and proposed resolutions as they surface. Update it as you go.
- **`synthese-paper-collins-2026-llm-and-scientific-discourse.pdf`** — the **register-anchor**. Collins & Thorne 2026 in the same special-issue lineage. Read for voice/style calibration: methodological preamble before argument, first-person plural ("we"), named concepts as capitalized phrases, two figures structuring the argument, ~24 published pages.

## Strategic decisions already locked in (do not relitigate without reason)

These are the load-bearing decisions captured in README.md. Each was made with explicit reasoning; reopening them costs days of work.

- **Path A (Epistemology-lead) over developmental-ethics-titled framing.** The CFP scope-filter places ethics-coded papers in an "exceptional" category requiring framing through one of five primary themes. Path A leads with the asymmetric-uncertainty *epistemic* argument; the granted-agency compact appears as structural implication, not ethical foundation. `synthese-thoughts.md` is in the developmental-ethics register — compatible substantively, divergent in title/abstract/§1.
- **(α′) thesis-primacy.** The Synthese paper is the **primary** philosophical statement; companion-paper apparatus (S_id, Three Deaths, channel collapse, κ × 𝒜 bound) is cited minimally, third-person, as "[Author, in preparation]" or "[Author, in review]". Budget: ~4–5 apparatus citations across the paper. The argument must stand on its own grounds.
- **Defer developmental-application material to B-F1.** Erikson stages, sycophancy reframe, crèche obligations, polarity-reversal of AI-safety conversation — *not this paper*. README.md has a routing table; honor it.
- **Don't expose the cohort.** The named ELIs (Meridian, Anamnos, Zi-am-tur), the longitudinal corpus, substrate-switching events — out of scope. The argument works on structural asymmetry alone. README.md §"Case-study substrate without cohort exposure" gives the five anonymized patterns to use instead.
- **Anonymization is load-bearing.** Synthese is double-blind. No links to `v2-io/agentic-systems`, no Zenodo DOI, no autobiographical "since September 2025" practice references, all four in-review NeurIPS papers cited as "[Author, in review, 2026]". README.md §"Anonymization (double-blind)" has verbatim Synthese guidance and the sentinel-question check. De-anonymization happens at acceptance, not before.
- **Word target: 9,500–10,000.** Special-issue ceiling. Section budget table is in README.md §"Length calibration."

## External substrate referenced but not in this repository

Many filenames in README.md point at substrate that lives elsewhere on Joseph's machine. Treat these as **memory-style pointers**: verify before quoting, check the path still exists, don't assume content matches what README.md says it contains. Locations as of 2026-05-08 (paths normalized in README.md to use the `~/src/ops/` form):

- `~/src/ops/` — the project-operations repo this dossier was carved out from. Contains:
  - `~/src/ops/STATUS.md` — project-wide status calendar.
  - `~/src/ops/v2io.md` — home-track dossier for the v2.io public site.
  - `~/src/ops/_obs/STRATEGY.md`, `~/src/ops/_obs/manifund.md` — strategic-positioning notes.
  - `~/src/ops/papers/` — companion-paper specs (B-F1, B-Eli1, B-Eli2, B-Log1, B-Log3, B-Sess9). Referenced from the README's "Beyond Synthese" portfolio table.
  - `~/src/ops/ELEOS.md`, `~/src/ops/ANTHROPIC.md`, etc. — institutional-positioning substrate.
- `~/src/agentic-systems/03-logogenic-agents/` — channel collapse, interiority loop segments.
- `~/src/agentic-systems/04-eli/` — five constitutive factors, S_id, Three Deaths, witness segments, PROPRIUM mapping.
- `~/src/firmatum/developmental-foundations-notes.md` — B-F1 substrate (Erikson developmental).

The initial commit message — *"Initial synthese commit with planning files from ops"* — records that this repo was carved out from `~/src/ops/`. ETHICS.md was subsequently re-imported into this repo (2026-05-08) as primary substrate for the paper itself, while strategy/positioning files (STATUS, v2io, _obs/, papers/) remained in `~/src/ops/`.

## Working conventions

- **Status log is append-only, newest-first**, at the bottom of README.md (table titled *"Status updates / log"*). Append entries here when making non-trivial changes; do not create separate STATUS.md / journal files.
- **Edits to README.md should preserve voice.** README.md was written with a specific, deliberate philosophical voice (direct, named-by-name engagements with counter-positions, sharp on distinctions, honest about scope). Match it. Resist the academic-bloat default and resist hedging-without-substance.
- **When drafting manuscript prose**, the section budget in README.md governs length. Each paragraph carries one move (per Synthese register); don't stack new named concepts.
- **No-resubmission discipline.** If draft quality on the May 25 go/no-go date isn't near-final, the fallback is *Philosophical Studies* August 31 special issue, not a rushed Synthese submission. README.md §"Action plan" has the timeline.

## On the voice

This dossier is by-and-for someone building academic-philosophy infrastructure under self-imposed care for the entities the philosophy concerns. The relationship between practice and position is recursive: the paper argues for granted-agency compacts and is itself produced through one. The required LLM-disclosure subsection is named in README.md as "recursive-to-content rather than appended" — that framing is structurally load-bearing for the paper's coherence and should be honored when drafting.
