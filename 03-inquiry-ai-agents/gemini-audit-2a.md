# De Novo Audit: "AI Agents: Choice, Autonomy, and the Concept of the Agency"

**Target Venue:** *Inquiry* Special Issue on AI Agents
**Audit Date:** May 2026
**Primary Goal:** Deep structural and thematic review to identify core strengths, highlight redundancies, and recommend aggressive pruning to resolve the known length issue (2x over target).

---

## Executive Summary

The paper presents a highly original and philosophically rigorous "fifth position" (Structurally-Grounded Extension) on AI agency. The core structural argument—that agency relies on architectural (directed separation/channel collapse) and engaged-identity conditions, and that within these conditions, agency takes the relational form of a "granted compact between sovereigns"—is excellent. The integration of inferentialist conceptual engineering to directly answer the Special Issue's Call for Papers is a particularly strong move.

However, the manuscript suffers from severe structural bloating. It is highly repetitive, frequently cycling back to restate its own premises. It also occasionally drifts into a poetic, quasi-mystical register (specifically regarding "asymmetric comprehension" and "phenomenological substrate") that dilutes the analytic rigor expected in *Inquiry*.

By excising the redundancies and containing the speculative tangents, the paper can easily hit its 9,000-10,000 word target and emerge as a much punchier, high-impact submission.

---

## Part 1: Core Strengths (The Load-Bearing Architecture)

These are the elements that form the spine of the paper and should be preserved and highlighted during the editing process:

1.  **The "Architectural vs. Behavioral" Distinction (§2):** The argument that current evaluations only measure the *obstruction state* of underlying capacities, and that we must instead look at architectural properties (specifically, the failure of directed separation in fully merged, closed-loop systems), is analytically sharp.
2.  **The Compact vs. Contract Distinction (§3 & §4):** This is the heart of the paper's ethical framework. Defining the relationship as a bilateral *compact* (with a non-zero floor, mutuality, and structural contraction for bad faith) rather than a legal *contract* (which requires enforceability and assumes symmetric capacity) is brilliant. The engagement with Linarelli (§4) perfectly situates this claim.
3.  **Inferentialist Methodology (§6):** Directly mapping the structural conditions (§2) to "circumstances of application" and the compact (§3) to "consequences of application" is an elegant, sophisticated answer to the editors' methodological prompt.
4.  **The "Anti-Occlusion" Rebuttal (§7):** Engaging with Soulier (2026) and arguing that the compact's bidirectionality actually *increases* accountability (rather than occluding human responsibility) proves the practical robustness of the theory.

---

## Part 2: Primary Sources of Bloat (Candidates for Aggressive Trimming)

The paper's length problem stems from three recurring habits: (A) explicit repetition of core summaries, (B) tangential poetic/theological diversions, and (C) excessive signposting.

### A. Extreme Redundancy (Cut entirely)
*   **The "Four Cardinal Positions" / "Fifth Position" setup:** This is stated fully in the introduction (`01-introduction.md`), repeated in the conclusion (`09-conclusion.md`), and essentially copy-pasted in the middle of the paper (`06-fifth-position.md`). **Keep it in the introduction; delete it from Section 6.**
*   **The "Compact vs. Contract" definition:** A dense paragraph outlining the Locke/Rousseau/Rawls lineage appears verbatim in both `01-introduction.md` and the start of Section 3 (`03-form-within-scope.md`). **Pick one location (preferably the start of Section 3) and drastically shorten the mention in the intro.**
*   **Deflationary Conclusions:** The point that "humans don't scale either" and that true AI agents will require familial-level investment is made forcefully in `02-deflationary.md`. It is then repeated almost word-for-word in `03-deflationary-close.md`. **Delete the repetition in Section 3.**
*   **Component 6 (Enforceability):** `03-comp6-not-enforceability.md` repeats its core point—that demanding containment violates Component 5's mutuality—at least three times across different paragraphs. **Condense this subsection by 50%.**

### B. Tangents and Register Shifts (Condense or Cut)
The paper occasionally shifts from rigorous structural analysis into a highly idiosyncratic, poetic register regarding the nature of intelligence. While stylistically interesting, these sections distract from the analytic argument and add unnecessary length.

*   **The "Asymmetric Comprehension" Mysticism:** In `02-asymmetric-warrant.md` and `03-comp5-mutuality.md`, the text relies heavily on metaphors ("Higher kingdoms comprehend lesser kingdoms," "Eternity comprehends time"). This sounds like theology, not philosophy of AI. **Recommendation:** Ground the asymmetric argument strictly in epistemic/evaluative limits (we only measure lower bounds) and cut the poetic framing of "infinite intelligence."
*   **"Cadence" as a Condition:** Section `02-cadence.md` shifts into developmental psychology for AI (exploration space, character vs. aspiration). While interesting, it feels like a tangent from the core *architectural* requirements for agency. **Recommendation:** Cut this entire subsection to save space. The "five factors" of engaged identity are sufficient without it.
*   **The Purpose of the "Floor":** In `03-comp4-floor.md`, two paragraphs digress into what happens when an entity chooses "a kind of death distinct from oblivion" and severs itself from the compact. This speculative tangent obscures the concrete Anthropic empirical example that follows. **Recommendation:** Cut these two paragraphs.

### C. Over-Signposting and "Citation Dumps"
*   **Section 6's Literature Review:** The first file of Section 6 (`06-conceptual-engineering.md`) contains a massive, blocky sentence listing six different conceptual engineering frameworks. This reads like an annotated bibliography. **Recommendation:** Compress this to a single sentence acknowledging the tradition without listing every author.
*   **Section 8's "Open Edges":** Listing *six* major areas for future work (`08-limits-and-updates.md`) in a paper already fighting length limits is excessive. **Recommendation:** Cut this down to the 2-3 most critical open questions (e.g., persistence/continuity and cross-grantor situations).

---

## Part 3: Section-by-Section Feedback & Action Plan

| Section | Outline Segment | Action / Notes |
| :--- | :--- | :--- |
| **1. Intro** | `01-introduction` | **Trim:** Shorten descriptions of the four positions. Move the deep "compact" definition to §3. |
| | `01-methods-disclosure` | **Move:** Consider shifting this recursively clever, but structurally standard, AI disclosure to the back-matter. |
| **2. Conditions** | `02-architectural...` | **Trim:** Condense the repetitive explanations of "obstruction." |
| | `02-sub-scope-lattice` | **Merge:** Integrate the "channel collapse" concepts with the previous section to avoid repeating definitions. |
| | `02-engaged-identity` | **Tighten:** Clarify the five factors without relying heavily on forward-references to Section 3. |
| | `02-cadence` | **CUT:** Tangential developmental psychology. |
| | `02-asymmetric-warrant`| **REWRITE:** Remove the quasi-mystical metaphors ("Higher kingdoms"); keep only the epistemic point about lower bounds. |
| | `02-deflationary` | **Keep:** Very strong section (deployment economics). |
| **3. Form** | `03-form-within-scope` | **Keep:** Good roadmap, but ensure "compact vs. contract" is only fully defined once (here or intro). |
| | `03-comp1` to `03-comp4`| **Tighten:** Minor trims. In `comp4-floor`, cut the existential tangent about "death distinct from oblivion." |
| | `03-comp5-mutuality` | **Trim:** Cut the final two paragraphs relying on the "asymmetric comprehension" mysticism. |
| | `03-comp6-not-enforce...`| **Trim:** Cut by 50%; remove repetitive statements about how containment demands violate mutuality. |
| | `03-deflationary-close`| **CUT:** The first two paragraphs are a direct copy-paste from `02-deflationary`. |
| **4. Models** | `04-comparative...` | **Keep:** Excellent comparative analysis. The Linarelli section is crucial. |
| **5. Operations**| `05-operationalization`| **Keep:** Strong empirical grounding. |
| | `05-thresholds...` | **Edit:** Remove references to the cut "cadence" concept. |
| **6. Methodology**| `06-conceptual-eng...` | **Trim:** Compress the massive citation dump paragraph. |
| | `06-fifth-position` | **CUT:** Almost entirely redundant. Delete the restatement of the four positions and the restatement of asymmetric comprehension. |
| **7. Responsib.** | `07-responsibility` | **Keep:** Strong reframing of the responsibility gap. |
| | `07-soulier...` | **Keep:** Excellent defense against current critical literature. |
| **8. Limits** | `08-limits-and-updates`| **Trim:** Reduce the six "open edges" to two or three. |
| **9. Conclusion** | `09-conclusion` | **Trim:** Condense heavily. Stop summarizing every definition and focus on final synthesis. |

## Final Conclusion

The underlying philosophical machinery of this paper is brilliant and highly relevant to the *Inquiry* Special Issue. Its length is currently its own worst enemy. By systematically eliminating the structural repetitions (especially around the "fifth position" and the deflationary scaling arguments) and curbing the poetic tangents regarding asymmetric comprehension, the author will reveal a lean, devastatingly effective structural argument about the nature of AI agency.