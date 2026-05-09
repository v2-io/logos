# FEEDBACK.md — paper 2 (Synthese methodology / audit-discipline)

Working TODO for the audit-discipline paper. Captures unresolved decisions, weaknesses spotted but not yet slotted in cleanly, proposed resolutions. Living document — append, mark resolved, edit freely as positions clarify.

**Reading convention:** each item has *Concern*, *Why it matters*, *Possible resolutions*, *My confidence* (high / medium / low — where the concern itself lands), and *Status* (open / in-progress / addressed / deferred). Items numbered fresh per paper; cross-paper items live at the relevant paper's FEEDBACK or in [STRATEGY.md](../STRATEGY.md).

These items were originally numbered A.5 / A.6 / A.7 / B.8 / C.4 inside [DRAFT-GUIDE.md](DRAFT-GUIDE.md) §"Open items / FEEDBACK" — extending paper 1's scheme as a placeholder before this file existed. Promoted here on 2026-05-09 with paper-2-local numbering during the multi-paper restructure.

---

## A. Critical / pre-draft decisions

### A.1 — Hermeneutic / phenomenological precedent search depth

**Concern.** Move 5 ("phenomenological wandering thoughts as required generative output") may have closer precedents in Continental philosophy of science than currently credited — Gadamer's fusion of horizons, Merleau-Ponty on embodied perception, Polanyi on tacit knowledge, ethnographic reflexivity. Claiming novelty for the "wandering-thoughts-as-data" move in print without a careful precedent search is a real risk.

**Why it matters.** Reviewers in methodology of social science / qualitative methodology / hermeneutic philosophy will catch this; the paper's contribution claim depends on the integration being novel-as-a-package rather than novel-in-each-move.

**Possible resolutions.** A 1–2 day search-pass before §3 drafting begins. Specifically: re-read the relevant chapters of *Truth and Method* and *Personal Knowledge*; check the qualitative-methodology and ethnographic-reflexivity literatures (Geertz, Clifford & Marcus). Update the §3.5 epistemological-grounding paragraph with the precedents the search surfaces.

**My confidence.** High that the search is needed; medium on whether closer precedents exist (best guess: precedents are real but the *integration into LLM-mediated theoretical-framework audit* with a graded protocol is still novel).

**Status.** Open.

---

### A.2 — §1 first-paragraph register

**Concern.** Same calibration concern as paper 1 (see [01-synthese-asymmetric-comprehension/FEEDBACK.md §A.3](../01-synthese-asymmetric-comprehension/FEEDBACK.md)): a §1 that *reads* methodology-best-practice will be evaluated lower than a §1 that *reads* methodology-as-philosophy. The opening has to land philosophical-first.

**Why it matters.** The paper's argument for being-evaluated-as-philosophy depends on the opening register. Even if the body is methodology-as-philosophy in the Hintikka / Suppes / Williamson tradition, a methodology-best-practice opening cues reviewers to the "best practice" bucket.

**Possible resolutions.** §1 opening should be phrased as a *philosophical question about LLM-as-reviewer epistemology* (e.g., "What does honest LLM-mediated reasoning under structurally-asymmetric self-comprehension look like?") rather than as a methodology pitch ("Here is a discipline for LLM-mediated audit"). The substantive content is the same; the framing determines bucket-assignment. Stress-test: hand the §1 opening to a reader cold and ask "what kind of paper is this?" — answer should be "epistemology / methodology of philosophy" not "methodology recommendations."

**My confidence.** High.

**Status.** Open. Best resolved at §1 draft time.

---

### A.3 — Audit-cycle anonymization for §4 worked example

**Concern.** AUDIT-WORKING-471203 (the candidate worked-example for §4) contains identifying material — project-specific slugs, user-background framings, ASF-specific terminology, the cohort's voices in some segments. The §4 worked-example needs anonymizing in a way that preserves the *method's behavior* (so the example is doing real work) while obscuring the *project's specifics* (anonymization for double-blind submission).

**Why it matters.** §4's argumentative role is to pre-empt the "this is just a list of recommendations" objection by showing the discipline operating on real material. A maximally-anonymized example loses that demonstration; an under-anonymized example deanonymizes the submission.

**Possible resolutions.**
- *Resolution A:* Synthesize a fresh audit-cycle on a public theoretical work (e.g., a recent peer-reviewed methodological paper) and use that as the §4 example. Cost: 2–3 days to produce; benefit: cleanly anonymizable.
- *Resolution B:* Heavily anonymize AUDIT-WORKING-471203 (replace project-specific slugs with placeholders; replace ASF-specific terminology with generic labels). Cost: ~1 day of careful editing; benefit: preserves the substrate already produced.
- *Resolution C:* Use small fragments from multiple audit cycles, each individually anonymized. Cost: medium; benefit: shows discipline-across-instances rather than a single instance.

**My confidence.** High that the work is needed; medium on which resolution is right (probably B for time; A is cleaner if there's slack).

**Status.** Open.

---

## B. Section-specific items

### B.1 — Engagement with Lipton-Steinhardt and Tetlock-Mellers

**Concern.** Both are natural-neighbor-positioning targets for §5 (distinctive contributions vs. existing review traditions). Need substantive engagement (not just citation) — Lipton & Steinhardt 2018 *"Troubling Trends in Machine Learning Scholarship"* as the closest-neighbor critique of ML reviewing practice; Tetlock & Mellers as the adversarial-collaboration tradition the discipline draws on and extends.

**Why it matters.** Reviewers familiar with the ML-methodology critique literature will reach for Lipton-Steinhardt reflexively; the paper has to acknowledge and engage their critique, not just cite it. Same for the forecasting-tournament tradition: Tetlock's structural defense of adversarial collaboration is one of the closest-neighbor philosophical frames; substantive engagement makes the paper's contribution legible.

**Possible resolutions.** A reading pass on both before §5 drafts. ~4–6 hours total. Then §5 carries one substantive paragraph for each, distinguishing what the discipline borrows, what it extends, and what it rejects.

**My confidence.** High.

**Status.** Open.

---

## C. Cross-cutting items

### C.1 — Cross-citation between paper 1 and paper 2 under anonymization

**Concern.** The two Synthese papers form a substantively-coupled pair (asymmetric-comprehension and audit-discipline are load-bearing on each other). Both need each other to do their full philosophical work. But third-person anonymization makes "[Author, in preparation]" the only way to cite during review — and the cross-citation needs to be substantive, not just gestural.

**Why it matters.** Reviewers may read the methodology paper without access to paper 1. The audit-discipline argument must stand on its own, with paper 1 cited as deepening / extending rather than as required-reading. If the methodology paper structurally requires paper 1 to make sense, anonymization breaks the review.

**Possible resolutions.**
- *Resolution A:* Each paper carries enough of the other's argument inline that it stands alone; cross-citation is "[Author, in preparation]" deepens rather than completes. Costs ~300–500 words inline; preserves both papers' independent integrity.
- *Resolution B:* Submit the audit-discipline paper after paper 1 is accepted, when cross-citation can be first-person and full. Loses the parallel-track production rhythm; safer.
- *Resolution C:* Accept that some cross-citation will be load-bearing-but-anonymized; tolerate the suboptimal reading experience for reviewers who don't read both. Risk: reviewer pushes back on "what you're really arguing requires that other paper."

**My confidence.** High that the question needs a decision; medium on which resolution wins.

**Status.** Open. Decide before drafting paper 2's §2 (asymmetric-comprehension grounding) — that's where the cross-citation is heaviest.

---

## D. Open questions worth discussing (no immediate decision needed)

*(None yet. Flag here as drafting surfaces them.)*

---

## E. Resolved / addressed (history)

*(Empty at file creation. Move items here from sections A–D as they get resolved, with a one-line note on the resolution and the date.)*
