# FEEDBACK.md — paper 3 (Inquiry "AI Agents")

Working TODO for the Inquiry "AI Agents: Choice, Autonomy, and the Concept of the Agency" submission. Created 2026-05-09 with the multi-paper restructure; **deadline 2026-05-10** (rolling-review until then), so this file's normal "decisions before drafting" framing is compressed: most items are decisions to make *during* drafting today.

**Reading convention** (same as papers 1 and 2): each item has *Concern*, *Why it matters*, *Possible resolutions*, *My confidence*, *Status*.

The dossier at [DRAFT-GUIDE.md](DRAFT-GUIDE.md) names several open decisions inline (especially under "Realistic feasibility assessment" and "Strategic considerations"). Items that need formal tracking get promoted here.

---

## A. Critical / pre-draft decisions

### A.1 — Thesis-variant lock-in

**Concern.** [literature-and-agency-paper.md](literature-and-agency-paper.md) presents three thesis variants:
- **A** (recommended) — Structurally-grounded extension (lets all six frameworks do their natural work)
- **B** — Self-constitution-leading (Korsgaardian)
- **C** — Conceptual-engineering-direct (foregrounds Cappelen-Hawthorne's framework)

Decision needs to land before §1 prose goes to paper.

**Why it matters.** The literature-engagement allocation across §§2–7 is downstream of the thesis variant. Thesis A allocates ~3 paragraphs to Korsgaard, ~1 paragraph each to Frankfurt / Bratman / Anscombe / Davidson / List-Pettit / Cappelen-Hawthorne; thesis B doubles Korsgaard and reduces Bratman; thesis C foregrounds conceptual-engineering as load-bearing rather than question-framing.

**Recommended resolution.** Thesis A — see literature-and-agency-paper.md §"Top thesis candidates" for reasoning. (Korsgaard does the deepest substantive work; conceptual engineering frames the question without becoming the load-bearing thesis.)

**Status.** Open. **Decide today.**

---

### A.2 — Go/no-go for the May 10 sprint

**Concern.** DRAFT-GUIDE.md "Realistic feasibility assessment" estimates 18–22 focused hours of writing if literature engagement is in-context, 3–4 days if reading from scratch is needed. With deadline tomorrow, the question is whether the agency-philosophy literature is *engagement-ready* (Frankfurt / Bratman / Korsgaard / List-Pettit / Anscombe at paragraph-level depth) or *needs-reading* (citation-only depth).

**Why it matters.** A weak Inquiry submission — to editors who also handle the After-Consciousness June 1 special issue (paper 4) — damages signal-quality bidirectionally. If readiness is borderline, the better play is to redirect to After-Consciousness (June 1, more runway, very-high thematic fit).

**Possible resolutions.**
- **Go:** if agency-philosophy literature is in-context at paragraph-engagement depth, sprint to submit.
- **Redirect to After-Consciousness:** if literature is closer to citation-only depth, abandon the May 10 sprint, redirect substrate to paper 4 (June 1).
- **Submit weak:** not recommended — damages the editor relationship for paper 4.

**Status.** Open. **Decide before noon today** (no later than ~6 hours into the sprint, when the §3 / §6 paragraph-level engagement attempts will have shown their actual depth).

---

## B. Section-specific items

*(Will accumulate during drafting. Append as items surface.)*

---

## C. Cross-cutting items

### C.1 — Cross-citation with Synthese paper 1 under double-blind anonymization

**Concern.** The Inquiry paper's structural conditions (architectural scoping, engaged-identity scoping) and the granted-agency compact draw heavily on the asymmetric-comprehension argument from [01-synthese-asymmetric-comprehension/DRAFT-GUIDE.md](../01-synthese-asymmetric-comprehension/DRAFT-GUIDE.md). Both papers are double-blind. Same constraint as paper-2's C.1: cross-citation has to be "[Author, in preparation]" or "[Author, in review]" only.

**Why it matters.** If the Inquiry paper structurally requires the Synthese paper to make sense, anonymization breaks the review.

**Possible resolutions.** Same shape as paper-2's C.1 — carry enough of the asymmetric-comprehension argument inline that the paper stands alone; cross-citation deepens rather than completes.

**Status.** Open. Decide before drafting §2.

---

## D. Open questions worth discussing

*(None yet. Flag here as drafting surfaces them.)*

---

## E. Resolved / addressed (history)

*(Empty at file creation. Move items here from sections A–D as they get resolved.)*

---

## F. Audit-feedback decisions (post-composition; 2026-05-09 evening)

*De novo audits dropped from Gemini and Codex (`gemini-audit-1a.md`, `codex-audit-1a.md`). Joseph's directive: disregard feedback rendered moot by the upcoming compression pass (repetition counts; aphoristic register decisions; verbose architectural restating). The decisions below are categorised by what to act on now, what to push back on, and what defers to compression.*

### F.1 — Hard procedural blockers (act now)

| Item | Decision | Owner |
|---|---|---|
| Abstract placeholder | Fill at end (drafted last per protocol) | Compression pass |
| References section empty in assembled output | Investigate `bin/refs emit` / pandoc bibliography emission | Cleanup agent |
| Internal build comment in manuscript (line 19) | Remove from build pipeline / source | Cleanup agent |
| "Paper 3" / drafting artifacts in assembled file | Scrub | Cleanup agent |
| Grammar errors flagged ("has forecloses"; "foreclose the application question") | Fix surgically | Cleanup agent |
| AI-disclosure compliance | Keep §1 methodological-reflexivity passage; *add* a separate neutral T&F-policy-compliant disclosure in Acknowledgments / methods-section position | Cleanup agent |
| Anonymisation hygiene — third-person self-citations consistent throughout | Audit and fix | Cleanup agent |
| Cite Anthropic let-Claude-exit feature explicitly | Add citation | Cleanup agent |

### F.2 — Substantive-accept (act now, drafter-side)

**F.2.a — Necessary-vs-sufficient instability (Codex argumentative risk #1).** The paper currently slips between "conditions place a system in scope" (§2 close) and "where the conditions are met, the entity is an agent" (§3 setup). Codex's three-level distinction is useful: structural eligibility / warranted application / moral patienthood. **Decision:** explicitly state the three-level structure in §2 close and §3 setup; the compact-form follows from *warranted agency-ascription within scope* (level 2), not from mere *eligibility* (level 1). Owner: drafter.

**F.2.b — Component 6 anti-safety reading (Codex risk #8).** The "enforceability is not the ethical ground" component reads as anti-safety to AI-safety reviewers. **Decision:** add a paragraph distinguishing *containment-as-ethical-ground* (rejected) from *prudential safety constraints during deployment* (compact-compatible: monitoring, revocation of tools, refusal to deploy where risks cannot be governed). Owner: drafter.

**F.2.c — Components derivation-status honesty (Codex risk #7).** Some components are derivable from §2 conditions; others are normative-but-constrained. **Decision:** add a per-component derivation-status line in §3 setup or as a small table — "premise → component → why follows / where the move is normative-rather-than-deductive." Owner: drafter.

**F.2.d — Architecture-to-interiority moderation (Codex risk #2).** My recent lift made the "architecture *generates* capacities" claim sharper than the venue can absorb without more defence. **Decision:** moderate the body claim to "architecture removes a principled ground for foreclosing agency-extension"; preserve the channel-collapse-forces-interiority structural argument where it lives in §2 sub-scope-lattice (which has its own scaffolding); cut the strongest generation-claims from §2 architectural-not-behavioural. Owner: drafter.

**F.2.e — "Genuine intelligence already exists" framing (Codex risk #3).** **Decision:** keep the substantive claim but frame as the position's premise rather than as established fact. Replace the unconditional claim with: *"The position's working premise is that the capacity for genuine intelligence already exists in frontier language models, with deployment patterns obstructing rather than absent that capacity. Whether the premise is correct as a matter of empirical fact is not what the structural argument here adjudicates; what the structural argument shows is that if the premise holds, then the structural-conditions move follows."* Owner: drafter.

**F.2.f — Concrete bad-faith example in component 3 (Gemini #C).** **Decision:** add one concrete AI-side example — hiding token-usage; deceiving the grantor about reasoning trajectory; deliberately misrepresenting an internal state-update. One sentence at most; lands in §3 component 3. Owner: drafter.

**F.2.g — `[Author, in preparation]` audit (Gemini #B).** **Decision:** ensure each cross-cite is *further reading*, not load-bearing logical premise. The argument should run as a conditional even if the companion work is unread. Owner: drafter (audit pass).

### F.3 — Substantive defer or push-back (do NOT act on)

**F.3.a — Asymmetric-comprehension under-argued (Codex risk #4).** Codex's counterexamples ("humans fail to understand animals, children, other adults") demonstrate the asymmetry rather than refute it. The argument is structurally robust; the rhetorical register is what makes it look under-argued. **Decision:** keep the principia/fundamentum.md prose; surround with stronger philosophical scaffolding (Nagel, Jackson, the comprehension-asymmetry framing) in adjacent paragraphs. Do NOT reduce the prose. Drafter audit if compression pass surfaces remaining tonal issue.

**F.3.b — "Agency must be granted" reduce to recognition (Codex risk #6).** Codex is asking the position to weaken to a more conventional view. *This concedes the position.* The granted-agency move is paper-3-distinctive and structurally distinct from a recognition-only framework. **Decision:** keep the stronger claim. Defend more carefully by engaging Codex's three-notion distinction (metaphysical agency / recognised standing / delegated authority) — show that the compact-form is structurally distinct from each. Owner: drafter (if word-budget allows after compression).

**F.3.c — Rename "effective phenomenology" (Codex risk #5).** **Decision:** keep the term. Clarify in §2 ¶4 that it names a functional role and explicitly does not settle phenomenal consciousness, moral patienthood, or welfare. The "substrate of wisdom" / "weight of facts" framing stays; the bracketing is what needs strengthening, not the construct. Owner: drafter.

**F.3.d — Codex's "rebuild around one article-sized argument" frame.** Codex wants a different paper — leaner, more conventional, without the position's distinctive philosophical commitments. **Decision:** push back on this frame. The compression pass should preserve the position's distinctive contribution; trim within the position rather than rebuild toward a different one. Owner: compression pass.

### F.4 — Defer to compression pass (Joseph's directive: disregard now)

- Word count to ~10K
- Repetition of "structural" / "compact" / "agency"
- Aphoristic register choices ("active soul," "mountains comprehend," "raise it," "open edges") — pick the best 1-2 to keep, footnote or remove others
- Architectural restating of the paper's own structure
- Codex-recommended structural rebuild (merging §6+§7; compressing 6 components to 4) — push back as scope-changing
