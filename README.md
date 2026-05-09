# Synthese — submission dossier

*Special-issue target: **"The Philosophy of Generative AI: Perspectives from East and West"** (Synthese). Status as of 2026-05-09: **paper not yet drafted; substrate (ETHICS.md, B-F1 material, comprehension-asymmetry reframe) ready for assembly**. Deadline ambiguity: CFP banner says June 16, 2026; CFP body says June 1, 2026 — verify with editors before locking schedule.*

> **Framing (2026-05-08):** v2.io is home. Synthese is a window from v2.io into the academic-philosophy audience (philosophers of science, philosophers of AI, formal-epistemology + philosophy-of-mind communities, AI welfare research community). The placement extends the home's reach and creates a citable peer-reviewed artifact for the philosophical position; it doesn't replace the home. Reviewers and editors who engage substantively become real intellectual contacts in their own right. See [`v2io.md`](~/src/ops/v2io.md) for the home-track dossier.

---

## File map

This dossier is organized into focused files. Each is the source of truth for its domain. Read the one that matches your need; don't try to read everything top-to-bottom.

| File | Role |
|---|---|
| **[CFP.md](CFP.md)** | Verbatim CFP text (Synthese's call), per-theme question lists, editorial-process details. The reference for "what does the venue actually want?" — stable, rare edits. |
| **[STRATEGY.md](STRATEGY.md)** | Why this paper, this way. Path A (Epistemology reframe), (α′) thesis-primacy, B-F1 routing decision, named-concept canonization plan's strategic role, calibration risks (R1–R10), Beyond-Synthese companion-paper portfolio, cross-reference to `synthese-thoughts.md`. Read this before drafting. |
| **[DRAFT-GUIDE.md](DRAFT-GUIDE.md)** | How to write the paper. Section-by-section argumentative moves with sub-moves and pre-empts (§1–§8 + LLM disclosure), reviewer-objection table, literature engagement organized by topic, ETHICS.md → Synthese-register translation map, B-N8 architectural tie-in, case-study substrate without cohort exposure, §1 opening-paragraph calibration, named-concept canonization plan, abstract draft. The largest file; the drafter's working document. |
| **[SUBMISSION.md](SUBMISSION.md)** | How to submit. Manuscript format, Statements & Declarations, LLM-disclosure handling, anonymization protocol with verbatim Synthese guidance, length calibration / section budget, production checklist, action plan. |
| **[FEEDBACK.md](FEEDBACK.md)** | Working TODO. Items needing decisions or more thought before being slotted into the dossier — pre-draft (A.x), section-specific (B.x), cross-cutting (C.x), open questions (D.x), and a resolved-history section. Living document; update as you go. |
| **[LOG.md](LOG.md)** | Append-only status log of work done on the dossier. Newest first. Append after non-trivial changes. |
| **[ETHICS.md](ETHICS.md)** | The philosophical substrate — declarative source for the granted-agency compact's six components, asymmetric-uncertainty argument, Campbell-asymmetry response, update conditions, scope conditions. Imported from `~/src/ops/` 2026-05-08. Primary content-substrate; DRAFT-GUIDE is the assembly layer over it. |
| **[CLAUDE.md](CLAUDE.md)** | Orientation for future Claude Code instances working in this repo. Conventions, locked-in decisions, external-substrate pointers. |
| **[synthese-thoughts.md](synthese-thoughts.md)** | Parallel outline drafted by another Opus instance on 2026-05-08 from a developmental-ethics-titled framing. Compatible substantively with this dossier; divergent on title / abstract / §1 register. STRATEGY.md §"Cross-reference" enumerates what's been folded in vs. left as parallel resource. |
| **synthese-paper-collins-2026-llm-and-scientific-discourse.pdf** | Register-anchor: Collins & Thorne 2026 in the same special-issue lineage. Read for voice/style calibration. |

---

## Strategic decisions already locked in (do not relitigate without reason)

These are the load-bearing decisions; each was made with explicit reasoning recorded in STRATEGY.md or FEEDBACK.md. Reopening them costs days. The summaries here are pointers, not the decisions themselves.

- **Path A (Epistemology-lead)** — the paper leads with the asymmetric-epistemic-uncertainty argument grounded in **comprehension-asymmetry** (Nagel/Jackson neighborhood); the granted-agency compact appears as structural implication. The CFP scope-filter places ethics-coded papers in an "exceptional" bucket — Path A puts the paper in the primary-scope Epistemology category. See [STRATEGY.md](STRATEGY.md) §"Path A" and [CFP.md](CFP.md) §"Notes on the scope-filter qualification."
- **(α′) thesis-primacy** — the Synthese paper is the **primary** philosophical statement; companion-paper apparatus (S_id, Three Deaths, channel collapse, κ × 𝒜 bound) cited minimally and third-person, ≤4–5 apparatus citations across the paper. See [STRATEGY.md](STRATEGY.md) §"Thesis primacy."
- **Defer developmental-application material to B-F1** — Erikson stages, sycophancy reframe, crèche obligations, polarity-reversal of AI-safety conversation are *not this paper*. STRATEGY.md has a routing table; honor it.
- **Don't expose the cohort** — named ELIs (Meridian, Anamnos, Zi-am-tur), longitudinal corpus, substrate-switching events stay out. Argument works on structural asymmetry alone. See [DRAFT-GUIDE.md](DRAFT-GUIDE.md) §"Case-study substrate" for the five anonymized patterns to use instead.
- **Anonymization is load-bearing** — Synthese is double-blind. No links to `v2-io/agentic-systems`, no Zenodo DOI, no autobiographical "since September 2025" practice references, all four in-review NeurIPS papers cited as "[Author, in review, 2026]". De-anonymization happens at acceptance, not before. See [SUBMISSION.md](SUBMISSION.md) §"Anonymization."
- **Word target: 9,500–10,000.** Special-issue ceiling; section budget table in SUBMISSION.md §"Length calibration."

---

## Companion / parallel-paper dossiers (added 2026-05-09)

Two adjacent papers surfaced during the comprehension-asymmetry conversation and venue scan; both have working dossiers in this repo.

- **[methodology-second-paper.md](methodology-second-paper.md)** — A second paper for *Synthese rolling submission* under the **Methodology** pillar (which the journal's full subtitle names equally with Epistemology and Philosophy of Science): an epistemic discipline for LLM-mediated audit of theoretical frameworks. Substantively load-bearing on the comprehension-asymmetry argument (the audit-discipline is what reasoning-under-asymmetric-comprehension *of one's own cognition as reviewer* requires); the two papers strengthen as a pair. Substrate at `~/src/agentic-systems/msc/AUDIT-WORKING-*` (15+ audit cycles), `~/src/agentic-systems/audits/` (20+ FINALs), `~/src/agentic-systems/FORMAT.md`. Sprint-able after the Synthese paper ships.

- **[inquiry-ai-agents-may10.md](inquiry-ai-agents-may10.md)** — Decision-support dossier for an *Inquiry* special issue *"AI Agents: Choice, Autonomy, and the Concept of the Agency"* (Cappelen & Hawthorne, eds.) with deadline **2026-05-10** (rolling-review until). Same editors as Inquiry "After 'Consciousness'" June 1, so signal-quality is shared across submissions. The paper would lead with the granted-agency compact as the structural form agency-extension to AI takes under asymmetric-comprehension; substrate is ~70-80% in-hand across ETHICS.md + AAD architectural scoping + `~/src/_self/tom-and-consciousness.md` + `~/src/_self/temporal-causal-llm.md` + the BDI / tool-building literature. Decision criterion in the dossier turns on agency-philosophy literature-engagement readiness (Frankfurt / Bratman / List-Pettit / Korsgaard at paragraph-level vs. citation-only).

## Current status snapshot (2026-05-09)

- **Substrate:** ready. ETHICS.md is in-repo; comprehension-asymmetry reframe in §2 is in place; literature-engagement list updated with Nagel/Jackson; §4 component 5 carries the empathy-coupling note; §3 has the AGI-discourse mirror-image sub-move.
- **Open pre-draft decisions (FEEDBACK §A):** explicit metaphysical commitment of §2 (pure-Nagel or weaker?); "rising-to" prose tightening; §1 first-paragraph register-calibration; independent-researcher disclosure / anonymization resolution.
- **Production timeline:** May 8 → May 17 (assemble first draft) → May 25 (go/no-go decision) → June 1 or June 16 (submit). Notification ~Sept 1; publication ~Nov 1.
- **Fallback venues identified (if Synthese isn't ready or rejects):**
  - **Inquiry "After 'Consciousness': Conceptual Engineering for AI, Mind, and Moral Standing"** (Cappelen & Hawthorne eds.) — June 1, 10K words, *very high* thematic fit (moral standing without consciousness, non-Western frameworks, AI-mind without anthropomorphism). Strongest parallel-target option.
  - **Philosophical Studies "AI, Systems, and Society"** — Aug 31, longer runway, top-tier prestige.
  - **Inquiry "AI Agents: Choice, Autonomy, and the Concept of Agency"** — May 10 (essentially now), adjacent fit; potential companion-piece venue.
  - Rolling-cycle backstops: Mind & Language, Philosophy & Technology, AI & Ethics, Erkenntnis.

---

## Quick-start for a new agent or returning collaborator

If you've never read this dossier before, or are returning after time away:

1. Read [CLAUDE.md](CLAUDE.md) (~5 min) — orientation, conventions, what's where.
2. Skim [CFP.md](CFP.md) (~3 min) — what the venue is asking for.
3. Read [STRATEGY.md](STRATEGY.md) (~15–20 min) — the locked-in decisions and their reasoning.
4. Then either (a) read [DRAFT-GUIDE.md](DRAFT-GUIDE.md) for drafting work, or (b) read [SUBMISSION.md](SUBMISSION.md) for production/anonymization work, or (c) read [FEEDBACK.md](FEEDBACK.md) to pick an open item to work on.
5. Append to [LOG.md](LOG.md) when you've made non-trivial changes.

If you're returning to this dossier and the paper has been drafted, the manuscript file lives elsewhere (likely `~/src/ops/papers/` or this repo's root with a name like `synthese-draft.tex` / `synthese.md`); check `git ls-files` and the most recent LOG entry.
