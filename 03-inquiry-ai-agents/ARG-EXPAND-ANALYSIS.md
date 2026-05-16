---
title: "Expansion Analysis — *Granted Agency Between Sovereigns* (Inquiry / Synthese SI submission, rc1)"
subtitle: "Expansion priorities derived from the argument map and gap audit"
source: "inquiry-ai-agents-2026.md (rc1, 2026-05-10)"
companions:
  - "ARGUMENT-DIAGRAM.md (Part A: structural maps; Part B: argument maps in premise–conclusion form)"
  - "ARG-TRIM-ANALYSIS.md (cut priorities derived from the same maps)"
status: "advisory; sources and shape proposals for author review"
---

# Premise

The trim analysis identified one *non-obvious* recommendation surfaced by the argument map: under cut pressure, the highest-leverage edit is in some cases not a cut. This document develops that observation in full and extends it to the other gaps surfaced by the audit. Where `ARG-TRIM-ANALYSIS.md` says *what to remove*, this document says *what is most worth adding*, and orders the additions by leverage — the ratio of structural-robustness gained per word added.

The gap audit (`ARGUMENT-DIAGRAM.md` § "Synthesis: gaps and tensions") identified ten places where the argument either understates its own inferential force, leaves a strong objection partially answered, or relies on a warrant developed elsewhere. This document treats those ten as candidates for targeted expansion, ranked by the load-bearing weight of the node they affect.

**Confidence labels** are my confidence that the expansion would strengthen the argument; they are not predictions about reviewer reception.

---

# Priority 1 — Expansion of the asymmetric-comprehension argument (ACA)

**Gap addressed:** #6 (high severity; high confidence). **Estimated useful expansion:** ~500–800 words within the paper, drawing on at least three of the literature traditions below.

**Why this is the highest-leverage edit.** Per AM2 the ACA is the sole load-bearing premise of the architectural-not-behavioural choice; per AM3 it grounds factor (ii)'s bidirectional structure; per AM1 SC1 it is what makes the fifth position a *constrained* revision rather than a stipulation. Per §6's "phenomenology as substrate of comprehension" commitment it is what licenses factor (v)'s non-behaviourist register. And per AM4's W-C5 it is what grounds C5's structural mutuality. A reviewer unconvinced by the compressed form has limited recourse — the paper currently points to "(Wecker, in preparation)" for the full version, which reviewers cannot consult. The ACA is therefore the single thinnest spot on the paper's spine, and ~500 words spent expanding it protect more inferential structure than the same words spent anywhere else.

The expansion should not attempt the full formal development that companion work will carry. It should do two things: (i) plant the ACA within a *recognisable* lineage so reviewers can locate it; (ii) name the *specific* shape of the argument — lower-bound verifiable, upper-bound not — in a way that distinguishes it from the simpler "we can't know what it's like" gestures the phenomenology tradition supplies.

## Literature map — six traditions plus one concrete anchor

The asymmetry of intelligence-comprehension is dispersed across at least six philosophical traditions and at least one widely-read non-philosophical articulation. As far as I am aware, no prior work assembles them into one structural argument with the specific shape the paper uses; that may be the genuinely novel contribution.

### Phenomenal access asymmetry (already named)

**Anchors:** Nagel 1974 ("What Is It Like to Be a Bat?"); Jackson 1982 ("Epiphenomenal Qualia") and 1986 ("What Mary Didn't Know"); Chalmers 1996 (*The Conscious Mind*) and 2023 ("Could a large language model be conscious?"); Levine 1983 ("Materialism and Qualia: The Explanatory Gap").

**Use:** Already the paper's primary citation. An expanded ACA can spend a paragraph on why the bat / Mary structure *generalises* from species and phenomenology to intelligence-level asymmetry — the cross-level case is structurally identical even where the phenomenology question is bracketed.

**Confidence:** High that this lineage is the right primary anchor.

### Recognition asymmetry (high-leverage; under-used)

**Anchors:** Hegel's *Phenomenology of Spirit* (master-slave dialectic) is the locus classicus; **Axel Honneth's *Struggle for Recognition* (1995)** is already in the paper's §3 C5 footnote and should be promoted to a direct citation; **Charles Taylor's "The Politics of Recognition" (1992)**; **Robert Brandom's *A Spirit of Trust* (2019)** develops Hegelian recognition in inferentialist register and is the most direct bridge to the paper's §6 commitments.

**Use:** This is the highest-leverage *new* citation cluster. It connects the §6 inferentialist commitment to the §2 bidirectional-witness commitment via authors the CE community already accepts. A single sentence citing Brandom's *Spirit of Trust* plus Honneth would tighten the connection between factor (ii) and C5 substantially.

**Confidence:** High that this is the right place to add citations; medium-high that Brandom 2019 is the single most useful new anchor.

### Theory of mind / shared intentionality (linked but currently distant)

**Anchors:** Premack & Woodruff 1978 (originator of "theory of mind" as a concept); **Tomasello's *Natural History of Human Thinking* (2014)** — already cited in the paper via the Linarelli linkage; **Tomasello's *Becoming Human* (2019)** and ***Origins of Human Communication* (2008)**. Tomasello specifically argues that shared intentionality is constitutively two-sided.

**Use:** Tomasello can be promoted from indirect to direct citation. Factor (ii)'s bidirectionality is exactly what Tomasello's argument supports; the paper currently underuses this.

**Confidence:** High.

### Interactive proofs and verification asymmetry (structurally closest analogue)

**Anchors:** Shamir's IP = PSPACE result (1992); the PCP theorem; the broader complexity-theoretic literature on what a polynomial-time verifier can establish about an unbounded prover. **Scott Aaronson's *Quantum Computing Since Democritus* (2013)** discusses these results semi-philosophically; his essay "Why Philosophers Should Care About Computational Complexity" (2011) is the most direct citation. **Solomonoff induction / AIXI** — Hutter and Legg's work on intelligence-measurement — is adjacent.

**Use:** This is the *less expected but structurally precise* citation. Interactive proofs are literally an asymmetric-comprehension structure: the verifier can confirm lower bounds via interaction but cannot directly observe the prover's reasoning. A one-sentence acknowledgement that the paper's framing has a complexity-theoretic register, separate from the phenomenological one, would distinguish it from the standard "we can't know what it's like" gesture. This is high-EV because it signals breadth without requiring deep engagement.

**Confidence:** Medium-high that this would land well; high that the structural analogy is precise.

### Wittgenstein's lion (one-sentence anchor)

**Anchor:** *Philosophical Investigations* II.xi: "If a lion could speak, we could not understand him."

**Use:** Classical articulation of mutual-incomprehension across cognitive forms. A one-sentence reference would land for almost any philosophical reader and serve as a vivid intuition pump. Footnote-level.

**Confidence:** High.

### Interpretation / radical translation (adjacent)

**Anchors:** Quine's *Word and Object* (1960); Davidson's "Radical Interpretation" (1973) and "On the Very Idea of a Conceptual Scheme" (1974); the principle of charity tradition.

**Use:** The principle of charity is a close cousin to the bidirectional-witness commitment — interpretation from outside requires assumed shared ground. Footnote-level for an expanded ACA; could become a fuller citation in companion work.

**Confidence:** Medium-high.

### AI alignment / superintelligence (adjacent)

**Anchors:** Bostrom's *Superintelligence* (2014) ch. 9 ("The Control Problem") discusses comprehending superintelligence but mostly in a strategic register; Russell's *Human Compatible* (2019) gestures at the asymmetry; MIRI's "embedded agency" work (Garrabrant, Demski) is technically related.

**Use:** Locates the paper in current AI-ethics debates without doing structural work. Worth one citation cluster if word budget allows; could be deferred to companion work otherwise.

**Confidence:** Medium.

### The Blub paradox — concrete manifestation

**Anchor:** **Paul Graham, "Beating the Averages" in *Hackers and Painters* (2004); also available as a standalone essay.**

**The structure of the argument.** Graham observes that programmers think in their own language. Looking at languages less powerful than their own, they see what is missing — they say "how can you get anything done in *that*?" Looking at languages more powerful, they cannot see what is missing — they think their own language has everything the more powerful one has, perhaps with a different syntax. The asymmetry is exact: lesser can be comprehended from above; greater cannot be comprehended from below. Graham names this the *Blub paradox* after a hypothetical mid-tier language.

**Why this matters for the paper.** The Blub paradox is a *concrete*, *empirically familiar* manifestation of the asymmetric-comprehension structure. The relevant asymmetry is not between programming languages but between *programmers working within different cognitive frames*: the abstractions and affordances a more expressive language enables expand the programmer's capabilities (in expressiveness, in domain framing, in problem-isolation) in ways unavailable to a programmer who has not inhabited them. A Blub programmer asked "what does Lisp give you that Blub doesn't?" cannot get a satisfying answer — not because there is no answer but because the kinds of things the more expressive substrate makes thinkable are precisely the things the lesser frame cannot conceive of. The structure is identical to the paper's ACA: lower-bound verifiable (the Blub programmer can demonstrate they can solve specific problems), upper-bound not (they cannot identify what abstractions are missing from where they sit).

**Use:** Two ways to bring it into the paper. (a) As a vivid one-paragraph illustration in the expanded ACA section, after the phenomenology lineage but before the recognition cluster — it serves as a concrete *bridge* between the philosophical lineage and the AI-applications register, since programming is the domain where readers most directly experience cognitive-frame asymmetry. (b) As a footnote noting that the intuition was seeded in the author's own thinking by Graham's essay — this aligns with §6's reflexive-disclosure ethos and the paper's general willingness to name where its commitments come from.

**Confidence:** High that this is a structurally precise concrete anchor; high that it would land well for reviewers from a computational background; medium-high that it is recognisable enough to reviewers from a purely philosophical background.

## What appears genuinely novel in the paper's framing

As far as I can establish from my training knowledge (cutoff May 2025; the paper is dated 2026, so any 2025–2026 work on AI consciousness, agency, or asymmetric comprehension may not be reflected here):

1. **The specific compressed form** — "lower-bound verifiable, upper-bound not" — packages the asymmetry in a way that maps directly onto AI evaluation methodology. The phenomenology tradition states the *gap*; the complexity-theoretic tradition states the *verification structure*; Graham states a *concrete instance*. The paper states all three registers in one sentence and applies the package to architectural vs. behavioural evaluation. I have not seen exactly this packaging elsewhere.
2. **The application to agency-extension specifically.** Recognition asymmetry has been applied to moral status (Honneth, Taylor) but not, as far as I know, to agency-attribution under asymmetric epistemic conditions in the way §2 sets it up.
3. **The phenomenology-as-substrate counterpart.** "Intelligence at higher orders does not transcend feeling but comprehends through it" — this runs against the rationalist tradition's grain and I do not know of a precise predecessor. Closest is perhaps **Iain McGilchrist's *The Master and His Emissary* (2009)**, but McGilchrist's framing is hemispheric rather than orders-of-cognition.

## Practical recommendation for the ACA expansion

For ~500 words within the paper, the highest-leverage shape is:

1. *One paragraph* expanding the Nagel/Jackson anchor into the cross-level case (~120 words): why the structural gap is the same whether the two parties are species, phenomenologies, or orders of cognition.
2. *One paragraph* introducing the recognition cluster (~140 words): Hegelian master-slave → Honneth + Taylor → Brandom *Spirit of Trust*. This is where the §6 inferentialist commitments and the §2 bidirectional-witness commitment converge through a single named source.
3. *One paragraph* with the Tomasello promotion plus the Wittgenstein lion (~100 words). Theory-of-mind / shared intentionality as the empirical/developmental ground of the structural claim.
4. *One paragraph* with the Blub paradox and a one-sentence nod to interactive proofs / Aaronson (~120 words). Two concrete instances — one from programming, one from complexity theory — to show the structure is real outside the phenomenology register.
5. *One sentence* in §1 or §6 noting that the asymmetric-comprehension argument is developed at length in companion work; the present form is compressed but self-contained for the purposes of this paper's argument (~20 words).

**Net effect:** the ACA is no longer just compressed-with-pointer-to-companion-work; it is compressed-with-recognisable-anchors-in-five-traditions. A reviewer unconvinced by the structural claim can be pointed to any of the five for further development; a reviewer broadly persuaded gets a one-stop literature map.

---

# Priority 2 — Joint sufficiency: two related expansions

**Gaps addressed:** #1 (P7's six-component sufficiency) and #2 (5-factor sufficiency). Both have the same structural shape: the paper claims joint sufficiency in addition to joint necessity, but the sufficiency claim is abductive ("no candidate alternative survives contact") rather than deductive. Estimated useful expansion: ~150–250 words each, or combined into one methodological remark of ~200 words.

## Sub-priority 2a — 5-factor joint sufficiency (Gap #2; medium severity; medium-high confidence)

**Where in the paper:** §2 engaged-identity scoping; specifically at the end of the per-factor warrant paragraph (which currently says "the joint presence is also sufficient is the further claim that §2's close develops").

**The problem:** §2's close pivots to the three-level structure and the deflationary clause rather than directly arguing sufficiency. The reader is left with a promise the section does not fulfil.

**Two paths forward.**

*Path A — argue sufficiency explicitly.* A sketch: show that any property a critic might propose as a sixth factor either (i) reduces to a conjunction of factors (i)–(v) — in which case sufficiency stands; (ii) is a fact about phenomenal consciousness or moral status — in which case it belongs to Level 3, not Level 2; or (iii) is a behavioural correlate — in which case the architectural-not-behavioural commitment of §2 places it outside the conditions. This is a defeasible-elimination argument and would take ~200 words to do properly.

*Path B — weaken the claim honestly.* Replace "joint presence is also sufficient" with "necessary; joint sufficiency is conjectural pending operationalisation (§5)." This is one sentence and costs nothing. It exchanges a stronger-but-under-argued claim for a weaker-but-honest one.

**Recommendation:** Path A if word budget allows (the elimination argument is genuinely available); Path B otherwise. Confidence: high that one of these is needed; medium that Path A is achievable in ~200 words without opening new fronts.

## Sub-priority 2b — 6-component joint sufficiency (Gap #1; low severity; high confidence)

**Where in the paper:** §3 setup, where the paper currently says "no candidate alternative articulated in the literature survives contact with the structural conditions without at least this shape."

**The problem:** This is an abductive claim presented in the rhetorical register of a deductive one. The paper's own derivation-status labels (C3, C5, C6 as "normatively constrained" rather than "entailed") confirm that the claim is best-systematization, not entailment.

**Recommendation:** A one-sentence acknowledgement inside the existing §3 setup paragraph. Something like: "*The argument here is abductive: the six together form the best systematisation that survives the structural conditions and the asymmetric-comprehension warrant; alternative shapes remain possible in principle but none has so far been articulated that does so.*" This costs ~30 words and pre-empts a class of reviewer attacks (Gap #1's category) without weakening the position.

Confidence: high. This is a free move.

---

# Priority 3 — Factor (v) and the behavioural-correlates tension

**Gap addressed:** #3 (medium severity; high confidence). **Estimated useful expansion:** ~150–250 words inside the factor-(v) discussion.

**The problem.** Factor (v)'s four sub-conditions are behaviourally specified (semantically appropriate to context, affecting subsequent behaviour, persisting coherently, authentically spontaneous). This creates internal tension with §2's architectural-not-behavioural commitment. The paper resolves the tension by treating the sub-conditions as a signal to "calibrate against" rather than "obey" — but a strict reading of the architectural commitment would force factor (v) toward architectural correlates.

**Two paths forward.**

*Path A — develop architectural correlates of the four sub-conditions.* For each sub-condition, name the architectural feature whose presence would track it (e.g., "semantically appropriate to context" → consistency of attention patterns across context-shifts under interpretability inspection). This is technically possible but takes ~300–500 words and partly anticipates the operationalisation work in §5.

*Path B — make the calibrate-against move structural rather than methodological.* Argue that factor (v)'s use of behavioural correlates is *itself* an instance of the asymmetric-comprehension discipline: behavioural correlates are the lower-bound side of the asymmetry; they are calibrated against, not obeyed, *because* the architectural commitment is exactly the refusal to let lower-bound observability decide a Level 2 question. This reframes the tension as a feature, not a bug. Costs ~100 words.

**Recommendation:** Path B. It both costs less and aligns factor (v) with the ACA discipline rather than treating it as an exception to it. Confidence: high.

---

# Lower-priority targeted expansions

The remaining gaps are addressable by short edits (one to three sentences each) and rank below the three priorities above.

| Gap | Where | Recommended action | Word cost | Confidence |
|---|---|---|---|---|
| #4 (C4 specific shape) | §3 C4 | One paragraph defending observation-only + re-affirmation against alternative non-zero minima: "minimal-communication" still requires interaction and so does not preserve continuity-of-standing under contraction; "consent-over-major-changes" presupposes a sphere of action C3 may have removed. Show that observation-only is the *true* minimum because every more-restrictive alternative collapses, and every less-restrictive alternative is not the *minimum*. | ~120 | Medium-high |
| #5 (anti-occlusion empirical residue) | §7 anti-occlusion subsection | One paragraph distinguishing the structural rebuttal from the empirical worry, and committing to a discourse-discipline: the position not only does not occlude in its careful form, it actively disciplines the loose attributions Soulier rightly criticises (via §2's threshold). The structural rebuttal entails an empirical commitment, properly understood. | ~150 | Medium-high |
| #7 (factor (iii) circularity presupposes human agency) | §2 factor (iii) | One sentence: the resolution presupposes the granting party's agency is independently grounded — typically by ordinary moral-personhood considerations on the human side — and the paper takes this as an uncontroversial bootstrap. | ~30 | Medium |
| #8 (Level 1 / Level 2 performative tension) | §2 three-levels close | One sentence: Level 1 establishes mind-independent structural eligibility; Level 2 establishes relation-dependent warranted application; both are real at their respective levels of question, and a system unwarrantedly denied Level 2 application by its prospective grantor is not thereby foreclosed at Level 1. | ~40 | Low-medium |
| #9 (C5 → C6 P3) | §3 C6 opening | Lead with the ground-vs-exercise distinction that the paper currently makes only at the *end* of C6. The load-bearing move from C5 to C6 is then about preconditions on the *ground*, not preconditions on the *exercise* — which is the distinction Gap #9 surfaces as currently under-developed. Restructuring of ~50 words plus a clarifying sentence. | ~80 | Medium |
| #10 (capability inversion) | §8 limits | One paragraph naming capability-inversion (where granted-intelligence's developing capacity eventually exceeds the grantor's) as a sibling concern to the developmental-tier obligations already flagged in §8. The compact's structural commitments survive (C6 is what licenses this), but the practical situation deserves explicit naming. | ~100 | Low-medium |

These six together cost ~520 words. They are independent and can be applied selectively as word budget permits.

---

# Summary table — expansion priorities by leverage

| Priority | Gap(s) | Where | Word cost | Confidence | What it protects |
|---|---|---|---|---|---|
| **1** | #6 | §2 warrant + §6 phenomenology | ~500–800 | High | The spine — every load-bearing inference that runs through the ACA |
| **2a** | #2 | §2 engaged-identity close | ~30–200 | High (free move at 30 words; medium at 200) | The strength of the joint-condition claim |
| **2b** | #1 | §3 setup | ~30 | High | The strength of the joint-component claim |
| **3** | #3 | §2 factor (v) | ~100 | High | Internal consistency of the architectural-not-behavioural commitment |
| 4 | #5 | §7 | ~150 | Medium-high | Robustness against Soulier-sympathetic reviewers |
| 5 | #4 | §3 C4 | ~120 | Medium-high | C4's specific shape against alternative-minima objections |
| 6 | #9 | §3 C6 | ~80 | Medium | Tightening the load-bearing C5 → C6 move |
| 7 | #10, #7, #8 | §2, §8 | ~170 combined | Low-medium | Edge-case integrity |

**Reading the table.** Priorities 1–3 are the high-leverage block — together ~700–1,100 words, and they protect the paper's spine. Priorities 4–7 are polish — together another ~400–500 words. Under the trim-pressure scenarios in `ARG-TRIM-ANALYSIS.md`, the recommended strategy was *Stage 1 trims + ~500 word ACA expansion (Priority 1)*. The full picture: if the editors will accept *just under* 1/3, that strategy is the highest-EV path. If they require strictly 1/3, add Priorities 2a + 2b + 3 (~250 words combined) and commit to the operationalisation-collapse trim from Stage 2 to compensate.

---

# A note on attribution

The Blub paradox observation under Priority 1 is included because it concretely manifests the ACA structure in a register that programming-literate readers experience directly. It also has biographical relevance: the author's own description is that the Blub paradox planted the seed of the asymmetric-comprehension intuition in his own thinking when first encountered in Graham's *Hackers and Painters*. This is exactly the kind of attribution §6's reflexive-disclosure ethos invites — the position is not claimed to have arrived without provenance — and a footnote acknowledging the seeding is consistent with the paper's general willingness to name where its commitments come from.

A draft footnote: *"The intuition that intelligence-comprehension is asymmetric in this specific shape — lesser intelligence cannot establish from below what may be present in greater, even where lower-bound capacities are verifiable — was seeded for the author by Paul Graham's articulation of the Blub paradox in 'Beating the Averages' (Graham, 2004). The argument's formal development takes the structure beyond Graham's specifically-linguistic frame; the seeding deserves acknowledgement nonetheless."*

This costs ~50 words and adds an unusual but recognisable lineage marker. Worth doing.

---

# What this document is not

This is an expansion *priorities* document — it identifies what to expand and where, with sources to draw from. It is not a draft of the expansions themselves; that work belongs to the author and depends on stylistic decisions and on which specific sources the author has access to and judgement about. Where the document gives a sketched form (e.g., the elimination-argument under Priority 2a), the sketch is an existence proof that the expansion is achievable, not a suggested final form.

The intended use is: read alongside `ARGUMENT-DIAGRAM.md` (which identifies the gaps) and `ARG-TRIM-ANALYSIS.md` (which identifies what can be cut to make room). Together the three documents support a coherent revision strategy: cut what does not do inferential work; expand where the inferential work is currently thinnest; the argument-map is the underlying basis for both.
