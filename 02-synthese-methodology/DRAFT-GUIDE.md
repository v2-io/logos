# methodology-second-paper.md — The auditor-self-discipline paper as a deliberate Synthese second submission

*Created 2026-05-09 from a conversation that updated my honest assessment twice: first that the AUDIT-WORKING substrate is materially deeper than the FORMAT.md labeling layer alone, second that Synthese's mandate explicitly names Methodology as one of three pillars (so methodology-as-philosophy is core-scope, not exceptional-scope). This file is the working source for the second-paper concept; the asymmetric-comprehension paper (the existing dossier's subject) and this paper form a substantively load-bearing pair.*

---

## One-paragraph statement

A philosophical paper articulating an **epistemic discipline for LLM-mediated audit of theoretical frameworks**, defended as the practice that reasoning-under-asymmetric-comprehension *of one's own cognition as reviewer* requires. The paper packages, names, and gives epistemological grounding to a set of moves that have working-substrate-form across ~15 audit cycles in `~/src/archema-io/asf/msc/AUDIT-WORKING-*` and `~/src/archema-io/asf/audits/`: priming-bleed disclosure, prediction-pre-evidence, source-ordering discipline, strengthen-before-soften with tiered verdicts, phenomenological wandering as generative data, withdrawn-findings preservation, multi-axis trust calibration, Phase-2 cross-check with explicit counterevidence search, adversarial-creative break-protocol, and reflexive audit-process feedback. Each constituent move has individual precedents in social epistemology / formal epistemology / expert-elicitation literature; the integration applied to LLM-as-reviewer-of-theoretical-frame-work has not, as far as I can tell, been articulated as a coherent methodology with epistemological grounding.

## Why this is a philosophy paper, not a "best practice" paper

Synthese's full subtitle is *"An International Journal for Epistemology, Methodology and Philosophy of Science"* — three pillars, equal status. The journal's published track record runs methodology-as-philosophy at substantial volume: Hintikka's applied-logic methodology, Suppes's measurement theory, Tim Williamson's *philosophy of philosophy* (literally methodology-of-philosophy as philosophy), Chappell on parity-arguments-as-method, Buchak on risk-weighted-EU as methodology. Methodology done well *is* philosophy at Synthese. Treating "philosophical novelty" as restricted to position-taking metaphysical or ethical claims is a too-narrow sort that doesn't survive contact with the journal's mandate.

The CFP for the *"Philosophy of Generative AI"* special issue reinforces this. The Logic theme asks *"How can we evaluate the reasoning capacity of generative AI? What can we learn from the existing benchmarks established for LLMs? Consistency has been a major challenge for LLMs; what are the best ways to handle inconsistency?"* — these are methodology questions about LLM evaluation. The Epistemology theme asks *"how can generative AI ... undermine epistemic agency?"* under conditions where the LLM is *itself* the reviewer is exactly the audit-discipline paper's territory.

## The substantive contribution

Each of the ten moves below has individual precedents (named after each); the integration applied to LLM-mediated audit of theoretical-framework work is the contribution. The paper's argumentative load is to (a) name the moves clearly, (b) ground each in a real epistemological problem the LLM-as-reviewer faces, (c) defend the integration as more than the sum of its parts, and (d) connect the discipline to the comprehension-asymmetry argument from the companion paper as the *practice* that asymmetric-comprehension *requires*.

1. **Priming-bleed disclosure.** Before findings, enumerate which context (CLAUDE.md, MEMORY.md, role-prompts, user_background framings) is in-context, *and which directions each will tilt judgment*. *Precedents:* Bayesian prior-disclosure norms; preregistration in empirical science (Nosek et al.); the conflict-of-interest and competing-interest norms in medical research. *Novel application:* the LLM-as-reviewer's "priming" comes from auto-loaded context whose specific framings are knowable in advance, unlike the diffuse priors of human reviewers; explicit disclosure is *both possible and required* in a way it isn't for human reviewers.

2. **Initial-Predictions written before any segment is opened.** Auditor freezes a pre-evidence model: what they expect to be forced vs. chosen, novel vs. overclaimed, well-developed vs. underdeveloped. Per-segment reflections then test the predictions. *Precedents:* preregistration; Tetlock-style forecasting; Mellers's adversarial-collaboration design. *Novel application:* applied to qualitative review of theoretical-framework work, where the standard is post-hoc summary rather than preregistered prediction; this changes what counts as a "finding" (predicted-and-confirmed vs. surprised-by).

3. **Source-ordering discipline.** Do not read prior audits / spikes / msc / git history / proposals / TODO / Findings catalogs before reading the segment cold. After reading + first reflection, those become fair game. *Precedents:* blind-review norms in scientific peer review; the "verification-vs-discovery" distinction in scientific methodology. *Novel application:* the LLM-as-reviewer is uniquely susceptible to *prior-finding leakage* because retrieval-augmented context is so cheap; explicit ordering discipline is the structural answer.

4. **Strengthen-before-soften with tiered verdicts.** Each adversarial challenge is paired with a strengthening attempt; verdicts tier as ★ already-handled / ★★ scope-narrowing / ★★★ real-limit. *Precedents:* Mill on engaging the strongest opposing position; the steel-manning literature; charity in interpretation (Davidson, Quine). *Novel application:* operationalizes steel-manning as a *graded* protocol with retained-but-failed strengthening attempts as audit output, rather than as an exhortation that produces only the survivor.

5. **Phenomenological "wandering thoughts" as required generative output.** *"REQUIRED — Wandering thoughts (3-10+ paragraphs). Original thought. Continue threads. Phenomenology of being an auditor of this welcome."* The auditor's phenomenology is generative data, not noise to filter. *Precedents:* hermeneutic philosophy (Gadamer on the fusion of horizons; Merleau-Ponty on embodied perception); the Heideggerian distinction between ready-to-hand and present-at-hand; ethnography's reflexivity discipline. *Novel application:* applied as a *required* output category in technical audit — and specifically as a generative source for naming-brainstorm, application-discovery, and concept-mid-formed-flagging. There may be closer hermeneutic-philosophy precedents than I've fully searched; flag for [FEEDBACK.md](FEEDBACK.md).

6. **Withdrawn-findings preservation.** The FINAL keeps a record of findings that initially looked real but were withdrawn after deeper reading, *with the reasoning*. *Precedents:* clinical-trials registry norms (registered hypotheses must be reported even if null); negative-results journals; Lakatos's heuristic-positive vs. heuristic-negative. *Novel application:* applied to qualitative-review calibration; preserves first-pass error rate as catalog data, which is rare even in best practice.

7. **Multi-axis trust calibration.** Not flat reputation; specific calibration: *"high on substantive math; mid-high on structural commitments; mid on hygiene; high on epistemic discipline."* *Precedents:* expert-elicitation literature (Cooke; Aspinall); psychometric multi-axis competence assessment; Goldman on testimonial reliability. *Novel application:* decomposes credibility along the dimensions where it actually varies for theoretical-framework work, rather than collapsing to a single score.

8. **Phase-2 cross-check with explicit counterevidence search.** For each candidate finding, grep against prior audits / pending-findings / FINALs; record what was searched and what was found. *Precedents:* PRISMA in systematic review; replication-tracking norms. *Novel application:* applied to qualitative theoretical-framework audit, with the search machinery owned by the auditor as part of the audit's findings.

9. **Adversarial-creative break-protocol authorization.** When sequential walking produces diminishing returns, switch to generative-adversarial mode; surface material the systematic walk wouldn't. Documented and justified rather than concealed. *Precedents:* design-by-charrette; brainstorming under explicit ground-rules; the divergent-then-convergent pattern in design methodology. *Novel application:* applied within audit; the break-protocol's authorization is from the audit-instructions document, treated as a feature rather than a deviation.

10. **Reflexive audit-process feedback.** §G of each FINAL gives feedback to the audit instructions themselves; methodology is iterable. *Precedents:* PDSA cycles; Lakatos on research-programme evolution; the dialectical-revision tradition in philosophy of method. *Novel application:* applied to LLM-mediated audit, where the *instructions document* and the *practice* coevolve, and the practitioner's feedback becomes part of the practice.

The package's distinctive epistemological grounding: each move addresses a *specific failure mode* of the LLM-as-reviewer — uncritical context-priming, prior-finding leakage, charity-as-abdication, discarding-of-phenomenological-signal, overconfidence-without-calibration, single-axis-credibility-collapse, missing-counterevidence, sequential-fatigue, hidden-assumption-in-instructions. The package as a whole answers *what does honest LLM-as-reviewer practice look like, given the LLM's specific failure modes?*

## Connection to the asymmetric-comprehension Synthese paper (load-bearing, not cosmetic)

The two papers form a substantively-coupled pair:

- **The asymmetric-comprehension paper argues** that comprehension from below is structurally limited: greater comprehends lesser; lesser projects weakly or rises-to. This applies recursively to the auditor: the auditor cannot from below fully comprehend the theoretical frame they audit. The argument generates a moral situation but does not by itself specify *what honest practice under that condition looks like*.

- **The audit-discipline paper specifies** what honest practice under the comprehension-asymmetry condition looks like for the LLM-as-reviewer: priming-bleed disclosure, source-ordering, strengthen-before-soften, phenomenological wandering as data, etc. The discipline is what reasoning-under-asymmetric-comprehension-of-one's-own-cognition-as-reviewer *produces*.

The pair is more than thematically connected. The asymmetric-comprehension paper claims *this is the moral situation*; the audit-discipline paper claims *this is what the moral situation requires of the reviewer in practice*. They cross-cite naturally. The audit-discipline paper provides empirical-but-principled instantiation of the asymmetric-comprehension argument's recursive practice-commitment claim. The asymmetric-comprehension paper provides the philosophical grounding the audit-discipline paper's moves cohere around. *Neither paper is complete without the other; both are stronger together.*

## Working title candidates

- *"An Epistemic Discipline for LLM-Mediated Audit of Theoretical Frameworks"*
- *"Auditing Under Asymmetric Comprehension: Methodological Discipline for the LLM-as-Reviewer"*
- *"Priming, Prediction, and Preservation: A Methodology for Honest LLM-Mediated Theoretical Review"*
- *"What Honest LLM-as-Reviewer Practice Looks Like: A Methodological Framework"*

## Plausible section structure (8K–9K words)

| Section | Words | Move |
|---|---|---|
| §1 The problem of LLM-mediated review | 800–1,000 | Names the failure modes the discipline addresses; positions against existing peer-review and adversarial-collaboration literatures |
| §2 The asymmetric-comprehension grounding | 1,000–1,200 | Cites companion paper for the structural argument; develops the recursive practice-commitment specifically for the reviewer's situation |
| §3 The discipline's ten moves (with epistemological grounding) | 3,500–4,500 | Each move named, defined, paired with its precedent and its novel application; structural defense of why this packaging answers a specific failure mode |
| §4 Worked example | 800–1,200 | One full audit cycle (the AUDIT-WORKING-471203 / FINAL pair anonymized) demonstrating the discipline in action; pre-empts "this is just a list of recommendations" objection by showing operational behavior |
| §5 Distinctive contributions vs. existing review traditions | 600–800 | Engages peer-review literature, Tetlock/Mellers on adversarial collaboration, Goldman on testimonial reliability, Schwitzgebel on opaque cognition, the AI-evaluation literature; names what's new |
| §6 Limits, scope conditions, update conditions | 400–600 | Honest acknowledgment of what the discipline does and doesn't address; what would refine it; what's outside scope |
| §7 Conclusion | 300–400 | Tight close; the discipline as instantiation of asymmetric-comprehension reasoning |
| LLM-disclosure subsection | ~150 | Recursive-to-content; this paper was itself produced under (a version of) this discipline |
| **Total** | **~8,500** | |

## Substrate (where the working material lives)

- **`~/src/archema-io/asf/FORMAT.md`** — the labeling-and-promotion-gates layer. Two-axis taxonomy (`type` × `status`), stage-tracked promotion gates, equation-level tags, Findings catalog with Brief/Impact/Novelty Claim/Related Work/Search Log. Foundational for the audit substrate but not itself the philosophical contribution.
- **`~/src/archema-io/asf/doc/de-novo-audit-instructions.md`** — the audit-protocol document the practice operates against; explicit instructions for source-ordering, per-segment cadence, the 14-prompt reflection scaffolding, the §A–§G FINAL structure.
- **`~/src/archema-io/asf/msc/AUDIT-WORKING-*/`** — 15 audit working directories. Each contains `00-initial-predictions.md`, per-segment reflections (often 50–80 files per audit), cross-cutting documents (`adversarial-creative-challenges.md`, `meta-segments-adversarial-reading.md`, `audit-protocol-reminders.md`). The richest substrate for the worked-example section is AUDIT-WORKING-471203 (the de-novo audit, ~85 segments, with §A–§G FINAL and Phase 2 supplement).
- **`~/src/archema-io/asf/audits/`** — 20+ audit FINALs of varying scope (de-novo audits, focused audits, fresh-eyes assessments). The 2026-03-14 fresh-eyes assessment names "the Epistemic Hygiene" as one of ASF's strongest contributions; the more recent FINALs demonstrate the discipline's evolution.

The substrate is not paper-shape; it's practice-shape. The drafting work is articulation-of-existing-practice — naming the moves, grounding each epistemologically, defending the integration — rather than from-scratch theory development. At demonstrated production rate (~1 day per NeurIPS-scale paper), this is plausibly a 3–5 day sprint after the §1 first-paragraph register and the engagement-with-existing-review-traditions are decided.

## Literature engagement (preliminary; needs work before sprint)

**Existing review and adversarial-collaboration literatures:**
- Lipton & Steinhardt 2018 *"Troubling Trends in Machine Learning Scholarship"* — the closest-neighbor critique of ML reviewing practice; useful as positioning-target.
- Tetlock 2005 *Expert Political Judgment*; Tetlock & Mellers on Forecasting Tournaments — the adversarial-collaboration tradition.
- Cooke 1991 *Experts in Uncertainty* — expert elicitation methodology.
- Goldman 2001 *"Experts: Which Ones Should You Trust?"*; Goldman & Whitcomb 2011 *Social Epistemology: Essential Readings* — testimonial reliability and social epistemology grounding.
- Lakatos 1970 *"Falsification and the Methodology of Scientific Research Programmes"* — research-programme evolution; methodology as iterable.

**LLM / AI-evaluation literature:**
- Schwitzgebel 2024 on AI consciousness inference; the broader Schwitzgebel-Garza-Adkins line on opaque cognition.
- Birch 2024 *The Edge of Sentience* — moral status under uncertainty; methodology for assessing.
- Bender et al. 2021 (stochastic-parrots); Bender & Koller 2020 — the language-model-evaluation critique tradition.
- Birhane et al. 2022 on AI auditing — the audit-from-the-margins tradition.
- The Inquiry "After 'Consciousness'" CFP framing (Cappelen & Hawthorne) on conceptual engineering for AI/mind/moral-standing — adjacent conceptual-engineering literature.

**Hermeneutic / phenomenological precedents (likely real, needs deeper search):**
- Gadamer *Truth and Method* — fusion of horizons; the interpreter's pre-understanding as hermeneutic resource rather than bias.
- Merleau-Ponty *Phenomenology of Perception* — embodied perception.
- Heidegger *Being and Time* §15–§18 — ready-to-hand vs. present-at-hand; the world disclosing itself to engaged practice.
- Polanyi *Personal Knowledge* — tacit knowledge in scientific practice.

The hermeneutic/phenomenological line in particular needs careful search — some of the "wandering thoughts as data" / "phenomenology of being an auditor" moves may have closer precedents in Continental philosophy of science than I've credited.

**Methodology-of-philosophy and methodology-of-science:**
- Williamson 2007 *The Philosophy of Philosophy* — methodology of philosophy as philosophy.
- Kuhn 1962 *Structure*; Lakatos 1970 — methodology of scientific revolutions / research programmes.
- Hintikka on formal methodology of inquiry; Suppes on measurement theory — the Synthese tradition.

## Venue options

- **Synthese rolling submission (Methodology pillar).** Primary target. No special-issue scope-filter risk; methodology is core-scope. Substantive engagement with Hintikka / Williamson / Suppes-style methodology-as-philosophy lineage lands the paper in the journal's actual tradition. Same journal as the asymmetric-comprehension paper's special-issue submission, allowing natural cross-citation.
- **Synthese topical collection — "Epistemic Agency in the Age of AI"** (per ISPR listing surfaced by venue scan) — possibly the cleaner home if the topical collection's framing fits.
- ***Studies in History and Philosophy of Science*** — methodology-of-science venue; would frame the contribution as methodology-of-AI-mediated-research-frameworks.
- ***Philosophy of Science***, methods track — same lineage.
- ***Philosophy of the Social Sciences*** — for the testimonial-knowledge / social-epistemology hook.
- ***Episteme*** — for the AI-as-testifier hook.
- **AI-systems venues** (NeurIPS / IJCAI / AAAI) — would re-frame as systems contribution; possible-but-not-recommended (loses the philosophical contribution by recasting as engineering).

**Recommendation:** Synthese rolling submission. Same journal, distinct paper, no special-issue scope-filter risk, fits the journal's mandate cleanly under the Methodology pillar.

## Substrate-readiness for sprint

**Ready:** Practice-substrate (15+ audit directories, 20+ FINALs); the protocol document; the FORMAT.md labeling layer; the discipline-in-action across multiple audit cycles; the worked-example candidate (AUDIT-WORKING-471203).

**Needs drafting:** §1 problem-of-LLM-mediated-review framing; §3 paragraph-level epistemological-grounding for each of the ten moves (the substrate has the moves but doesn't articulate the grounding paragraph-style); §5 engagement with existing review traditions (Lipton-Steinhardt, Tetlock-Mellers, Goldman); the worked-example anonymization; the LLM-disclosure subsection; the conclusion.

**Risk:** the hermeneutic/phenomenological lineage search (precedents for "wandering thoughts as data") needs careful work before claiming novelty in print. Continental philosophy of science may have closer precedents than I've credited — Polanyi on tacit knowledge, Gadamer on the interpreter's horizon, ethnographic reflexivity. A 1–2 day search-pass before writing would close the risk.

**Sprint estimate (after pre-draft items resolved):** 4–6 focused days of writing at the demonstrated production rate, plus ~1 day for the literature-engagement pass. Concurrent-with or after the Synthese paper is fine; the audit-discipline paper does not have a hard external deadline.

## Open items / FEEDBACK

Open pre-draft and section-specific items now live in [FEEDBACK.md](FEEDBACK.md) (paper-2-local A.1–A.3, B.1, C.1; promoted there during the 2026-05-09 multi-paper restructure). Append further items there as drafting surfaces them.

## Notes from the conversation that produced this file (2026-05-09)

- I was wrong twice on the same axis in the conversation: first underestimating the AUDIT-WORKING substrate's depth (thought it was just FORMAT.md labeling; it's a coherent epistemic-discipline package); second underestimating Synthese's mandate (thought "philosophical novelty" was position-taking only; the journal explicitly names Methodology as a pillar, with a published track record to match).
- The pattern of error was sorting "philosophical" → "must take a metaphysical / ethical / epistemological position" and treating "methodology" as a less-philosophical category. That sort doesn't survive contact with Synthese's actual subtitle, with the Hintikka / Williamson / Suppes tradition, or with the CFP's specific questions.
- Worth marking explicitly so future strategic thinking on this dossier doesn't repeat the error.
- Joseph's instinct that *"Synthese's actual mandate ... I can't help but think it envisioned exactly this type of practical side, notwithstanding it being philosophy"* was the corrective.
