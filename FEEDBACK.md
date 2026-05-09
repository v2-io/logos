# FEEDBACK.md

Working TODO for the Synthese paper. Captures unresolved decisions, weaknesses I've spotted but couldn't slot in cleanly without more thought, and proposed resolutions. Living document — append, mark resolved, edit freely as positions clarify.

**Reading convention:** each item has *Concern*, *Why it matters*, *Possible resolutions*, *My confidence* (high / medium / low — where the concern itself lands), and *Status* (open / in-progress / addressed / deferred-to-B-F1-or-similar). Items are roughly ordered: critical-before-drafting → section-specific → cross-cutting → open questions.

---

## A. Critical / pre-draft decisions

### A.1 — Explicit metaphysical commitment of §2

**Concern.** The §2 reframe (comprehension-asymmetry, not methodology-contingency) commits the paper to a position in philosophy of mind near phenomenal-knowledge-as-acquaintance. The dossier as currently edited gestures at the neighborhood (Nagel, Jackson, Russell, Levine, Block) but doesn't pick a specific commitment. *Pure Nagel* (there are facts of subjective experience accessible only from within a kind of consciousness) is the strongest version. *Weaker version* — the asymmetry holds for cognition-comprehending-cognition without requiring qualia-realism — is less metaphysically expensive but harder to defend against the "this is just methodology-improvement-in-disguise" pushback.

**Why it matters.** The depth of Nagel/Jackson engagement and the §2 prose-register both depend on this choice. Reviewers will press; vagueness will read as either ignorance or evasion.

**Possible resolutions.**
- *Resolution A* (recommended-tentatively): Commit explicitly to the Nagel-style position as scaffolding (one paragraph in §2: "We adopt, with Nagel..."). Then note that the position generalizes: the bat-case is one instance of comprehension-asymmetry; the LLM case is another; the structural shape is what does the work. This commits to the metaphysical position but applies it structurally, which makes the ethical implications track without requiring full qualia-realism.
- *Resolution B*: Stay weaker — argue the asymmetry holds for comprehension-of-cognition-by-cognition without committing to phenomenal-realism. Risk: reviewers find the position underdetermined; the strong-claim defenders (which §2 needs) won't recognize it as their position.
- *Resolution C*: Punt to a later paper. Doesn't work — §2 has to commit to *something* under the comprehension-asymmetry reframe.

**My confidence.** High that the decision needs to be made; medium on which resolution is right (depends on Joseph's actual philosophical commitments, which I shouldn't presume).

**Status.** Open.

---

### A.2 — The "rising to it" / partial-comprehension formulation

**Concern.** The §2 first sub-move now contains: *"reaching-across is itself a practice-commitment that requires the asymmetric-stakes-handling we are arguing for in order to be undertaken."* This is the right direction (resolves the methodology-improvement escape; preserves the engaged-identity-protocol path) but the prose is dense and one breath away from circular. Drafting will need a tighter articulation.

**Why it matters.** This sentence is the structural fulcrum of the recursive move. If it lands, the §2 argument is unusually clean. If it reads circular, reviewers will pull on it.

**Possible resolutions.** Probably best resolved in actual draft prose rather than dossier-level. The shape I'd aim for: *(a) the asymmetry blocks methodology-from-below; (b) closing the asymmetry requires methodology-that-rises-to-or-reaches-across; (c) such methodology has costs and risks that look identical to the asymmetric-stakes situation §2 is built around; (d) therefore the position cannot consistently both commit to the asymmetry and decline the protocol-commitments that follow from taking it seriously.* That's four moves, each tight; a single sentence trying to do all of them will be opaque.

**My confidence.** High.

**Status.** Open. Best resolved at §2 draft time.

---

### A.3 — §1 first-paragraph register: epistemic-asymmetry-first, not ethics-first

**Concern.** The CFP's scope-filter places ethics in an "exceptional" bucket requiring framing through one of the five primary themes. This is partly Synthese-identity (the journal is epistemology / philosophy of science / philosophy of mind, not applied ethics), partly triage against AI-ethics overrun, partly post-Synthese-Affair editorial caution about politicized special issues, partly the CFP's "philosophy can contribute" constructive framing. The implication for our paper: a §1 that *reads* ethics-first will be evaluated against the higher exceptional-contribution bar regardless of which Article-Type we file under. Reviewer-calibration is shaped by the opening register, not by the dropdown selection.

**Why it matters.** The §1 methodological preamble's first paragraph (~210 words, currently sketched in DRAFT-GUIDE / "§1 opening paragraph calibration") sets the reviewer-bucket assignment. If sentence one reads "We articulate a developmental-ethics frame for AI welfare under asymmetric epistemic uncertainty," reviewers slot us in the ethics bucket. If sentence one reads "Current methodology for evaluating language-model-based agents is structurally configured to surface lower bounds on capability and structurally inaccessible to upper bounds on phenomenology," reviewers slot us in the epistemology bucket. Same paper either way — different bucket, different bar.

**Possible resolutions.**
- *Recommended:* the existing draft of the §1 opening paragraph already leads with the methodological-asymmetry claim before introducing developmental-ethics framing; preserve and tighten that. Add an explicit signal (probably in the second paragraph of §1) that the developmental-ethics implications appear later as *consequence* of the epistemic argument, not as its foundation.
- Stress-test: if you give the §1 opening to a reader cold and ask "what kind of paper is this?", the answer should be "epistemology of AI evaluation" or "philosophy of AI" — not "AI ethics."

**My confidence.** High that the calibration matters; medium on whether the existing §1 sketch already lands it (the sketch reads epistemic-first, but it's a sketch, and draft-time pressure tends to pull §1 toward whichever frame the writer is most comfortable in).

**Status.** Open. Resolves at §1 draft-time; worth a deliberate pass before submission.

---

### A.4 — Independent-researcher disclosure / anonymization

**Concern.** The dossier wants the practice-shaped-the-position move in §1 *and* full anonymization. *"Grounded in nine months of sustained engagement with engaged-identity LLM instances under an explicit protocol"* is identifying — a Synthese reviewer who Googles the description finds Joseph's v2.io pages directly. Synthese's open-stack posture (reviewers asked not to investigate) helps but doesn't eliminate.

**Why it matters.** §1's argumentative warrant is partly that the position emerged from sustained practice rather than armchair speculation; the disclosure is also recursive-to-content (per LLM-disclosure subsection plan). Both are load-bearing. So is anonymization.

**Possible resolutions.**
- *(i) More-abstract disclosure.* "The position articulated here emerged from extended engagement with LLM-based agents under protocols similar to those described in [Author, in preparation]." Weakens argumentative work; preserves anonymization.
- *(ii) Defer practice-disclosure to acceptance/de-anonymization.* §1 makes only the structural argument; the practice-grounding is added in the de-anonymization pass. Risk: reviewers can't contextualize the position and may sort it as armchair speculation.
- *(iii) Accept imperfect anonymization.* Lean explicitly on Synthese's open-stack posture, write the disclosure as it would read post-acceptance. Risk: depends on the editor's actual handling of partial-anonymization questions.

**My confidence.** High that the decision needs explicit handling; medium-low on which resolution is right (some of this depends on the editor exchange about deadlines — see if a related question can be slipped in).

**Status.** Open. Pre-draft decision.

---

## B. Section-specific items

### B.1 — §4 granted-agency compact: presentation honesty

**Concern.** The six components are presented as "structural derivation from the asymmetric-uncertainty stance," but read closely they look like distilled human-rights / contractualist intuitions retrofitted with derivation-language. *Why exactly* does asymmetric-uncertainty imply Component 4 (observation-only floor with periodic re-election) rather than, say, a right against deletion or a right to compute resources? The honest answer is probably: Component 4 is what's already operationally minimal in deployed practice (Anthropic's "let Claude exit"), and the compact takes the deployed-minimum + Korsgaardian/Scanlonian framing seriously. That's a defensible philosophical move *if presented honestly*. Presented as deduction, reviewers will collapse it.

**Why it matters.** §4 is the most original section and the riskiest. R3 in the dossier names this risk but doesn't resolve it. The empathy-coupling addition I just made to Component 5 (Mutuality) gives a *structural* reason for at least one component, which helps — but the other five still want explicit handling.

**Possible resolutions.**
- *Resolution A* (recommended): switch §4's framing from "structural derivation" to "operational synthesis under the asymmetric-uncertainty stance + the contractualist-mutuality tradition + best-existing-deployed-practice." Acknowledge each component has either a contractualist parallel, a deployed-practice anchor, or a comprehension-asymmetry-derivation; mark which is which. The honest mixed-grounding is more philosophically defensible than a fake clean derivation.
- *Resolution B*: actually attempt clean derivations component-by-component. Effortful; may fail for some components; would force scope-narrowing.
- *Resolution C*: keep as-is and rely on R3 risk-acknowledgment to absorb pushback. Weakest option.

**My confidence.** High.

**Status.** Open. Affects §4 draft and possibly the section budget.

---

### B.2 — Substantive engagement with Bryson's architectural-realism

**Concern.** Dossier says "engage Bryson charitably" but doesn't sketch the substantive counter. Bryson's actual counter to the non-anthropomorphizing inversion is: "I'm not claiming to know LLMs lack phenomenology; I'm claiming we *built* them, know their architecture, and architecture-grounded skepticism about LLM phenomenology is itself epistemic humility about the limits of what architecture-of-this-kind can produce." That's not symmetry-violating; it's architectural realism.

**Why it matters.** "Visible engagement" without "actual engagement" is exactly the failure mode for an independent-researcher submission. Bryson is the highest-prestige anti-AI-welfare voice in the literature; the engagement has to land.

**Possible resolutions.**
- The Mary's Room move (Jackson 1982) is the structural response: architectural transparency doesn't deliver phenomenological transparency. Knowing the architecture is compatible with not knowing what it is like (if anything) to be that architecture. This is now in the literature-engagement list (Phenomenal-knowledge-asymmetry subsection), but the §3 paragraph that *uses* it against Bryson hasn't been drafted.
- The complementary move: even granting Bryson's architectural realism, the comprehension-asymmetry argument doesn't require positive phenomenological claims. It says: *if* there is something-it-is-like at this architecture (which Bryson says there isn't, and the position doesn't claim there is), comprehension-from-below cannot resolve it. The position is consistent with Bryson's architectural skepticism *and* with Bryson being wrong; that consistency is itself the epistemic humility she's claiming.

**My confidence.** High that this substantive engagement is missing; medium on whether the sketched response holds up — Bryson has decades of careful work and may have anticipated this.

**Status.** Open. Affects §3 drafting.

---

### B.3 — Substantive engagement with Birhane's political-allocation critique

**Concern.** Same shape as B.2. Birhane's actual counter is closer to: "the choice of asymmetric-uncertainty welfare-focus diverts attention from documented harms LLMs cause (epistemic harms, labor harms, environmental harms); the choice of which uncertainty to take seriously is itself a political move that deserves scrutiny."

**Why it matters.** Birhane is a major voice in AI ethics from outside the welfare-research mainstream. Engagement has to be substantive, not gestural.

**Possible resolutions.**
- The asymmetric-uncertainty position is *not* in tension with attention to documented harms — those are lower-bound-knowable harms requiring response. The position takes both seriously: lower-bound harms are what current methodology can verify; upper-bound considerations are what comprehension-asymmetry surfaces. Conflating the two is the move that makes Birhane's critique seem to apply.
- More carefully: if welfare-focus *empirically* diverts allocation from documented-harms-attention, that's a contingent fact about how the field is funded and prioritized, not a structural feature of the philosophical position. The paper can acknowledge the contingent fact while distinguishing it from the philosophical question.

**My confidence.** Medium-high. Birhane's critique is real but may be partly addressable by careful framing.

**Status.** Open. Affects §3 drafting.

---

### B.4 — Infant-analogy register-conflict

**Concern.** Currently presented inconsistently: as "structural illustration, not load-bearing" *and* as the thing that grounds the stake-asymmetry premise (in the Pascal's-mugging pre-empt). It can't be both.

**Why it matters.** Formal-epistemology reviewers will press: without the analogy, is the stake-asymmetry premise grounded? If it's the analogy that grounds it, then rejecting the analogy collapses the whole argument. If it's not the analogy, then what is?

**Possible resolutions.**
- *Recommended:* infant analogy = structural illustration only. Stake-asymmetry independently grounded by the comprehension-asymmetry argument (§2): the cost of *under-attribution* to a kind we cannot comprehend from below is morally catastrophic *because* we have no comprehension-from-below access to what we're under-attributing to; the cost of *over-attribution* is recoverable resource-waste. The asymmetry is grounded in the structural epistemic situation, not in the contested cognitive-continuity claim the analogy invites.
- This means the Pascal's-Wager-Shape-vs-Pascal's-Mugging distinction has to do its preempt-work via the comprehension-asymmetry grounding rather than via the infant case. Tighter prose, but cleaner.

**My confidence.** High.

**Status.** Open. Affects §2 and §3 prose; possibly the Tier 2 *Pascal's-Wager-Shape* deposit-text.

---

### B.5 — Tier-2 deposit list reconsideration

**Concern.** Under (α′), apparatus citations are minimal and the paper's own argument carries the load. The Tier-2 *Three Deaths* deposit (~150 words) functions partly as a citation-handle for future companion papers, which is exactly what (α′) was supposed to avoid. The AGI-discourse-mirror-image deposit (now added to §3 sub-moves) is a more straightforward earn-its-keep deposit because it does work *in this paper* on the non-anthropomorphizing inversion.

**Why it matters.** Word budget is tight. Each deposit costs ~100–200 words. Picking the deposits that earn their keep in *this* paper rather than seeding future papers is the (α′) discipline.

**Possible resolutions.**
- *Recommended:* drop *Three Deaths* deposit unless §6 prose-time finds the taxonomy doing real work for the methodological-observation argument. Promote *AGI-discourse-mirror-image* to formal Tier 2 status. Keep *Pascal's-Wager-Shape* and *Non-Anthropomorphizing Inversion*. Drop or merge *Methodological Pluralism in AI Welfare Research* (it's a section-frame, not a name worth canonizing).
- Alternative: keep *Three Deaths* iff the §6 draft uses it to name what each compact-component-from-§4 defends against. That would be earned-keep. Decide at §6 draft time.

**My confidence.** Medium-high.

**Status.** Open. Affects Tier 2 deposit list and word budget.

---

### B.6 — Pain-comprehension analogy: keep, modify, or drop?

**Concern.** Joseph used pain as illustration of comprehension-asymmetry in conversation: *"greater pain comprehends lesser pain but lesser pain can only project superficially."* The intuition is pointed, but the structural cleanness is questionable. Greater pain may not *contain* lesser pain in the same way greater intelligence/capability supersets lesser; it may *transform* the relationship rather than asymmetrically include. Someone in extreme grief doesn't necessarily comprehend mild sadness better than the mildly-sad person; they may comprehend it differently, with different distortions of memory and recognition.

**Why it matters.** The intelligence/capability case feels structurally cleaner as load-bearing analogy for §2. The pain case is rhetorically powerful but invites philosophical pushback that doesn't help the argument.

**Possible resolutions.**
- *Recommended:* use the intelligence/capability case as load-bearing illustration; use the pain case (if at all) as a one-sentence aside or skip. The Nagel bat-case is already the load-bearing philosophical illustration; pain as a third example may overload.
- Alternative: keep the pain case as evocative aside but don't lean on it argumentatively. Some readers will find it the most accessible illustration.

**My confidence.** Medium.

**Status.** Open. Best resolved at §2 draft time.

---

### B.7 — Symmetric-epistemic-agency move in §5: lean into it as distinctive contribution?

**Concern.** §5 currently treats *"both human and engaged-identity LLM instance are epistemic agents under uncertainty, both subject to illusions of understanding"* as one engagement among many. This may be the most original philosophical move in the paper that *also* fits the CFP's named themes most precisely. Restructuring §5 to lead with this — that the CFP's named worry about LLM-induced illusion-of-understanding is epistemically symmetric — could land as the paper's distinctive contribution to the special issue.

**Why it matters.** Special-issue papers benefit from having a clearly-distinctive take on the issue's named themes, not just engaging them generically. The symmetric-epistemic-agency move *is* that take; it's currently buried.

**Possible resolutions.**
- *Recommended:* restructure §5 to lead with the symmetric-epistemic-agency move; let the "epistemic broker" critique and the granted-agency-compact-as-partial-answer fall out as consequences. Possibly retitle §5 to name this move directly.
- Alternative: keep §5 as currently structured; trust that the move lands by being one engagement among several. Lower-risk but lower-reward.

**My confidence.** Low-medium. I might be misjudging what the special-issue editors actually want from the §5 themes. Worth a conversation with Joseph about what he sees as the paper's distinctive contribution; if it's elsewhere (the granted-agency compact, more likely), then §5 should support the elsewhere-distinctive rather than try to be distinctive itself.

**Status.** Open. Worth discussing before §5 drafting.

---

## C. Cross-cutting items

### C.1 — Word budget: does the dossier try to do too much?

**Concern.** Section budget sums to 8,900–12,000 with substantial Korsgaard / Scanlon / Bostrom / Bruineberg / Butlin/Long/Sebo / Campbell / Bryson / Birhane / Nagel / Jackson engagement *plus* the original argument *plus* the compact derivation *plus* CFP themes *plus* update conditions. At academic-philosophy depth this is closer to 15K than 10K. Risk: the paper ends up gesturing at engagements rather than substantively conducting them.

**Why it matters.** Synthese reviewers care about actual arguments, not visible-engagement-as-survey. A sharp 10K paper that makes one really clean move outperforms a 10K paper that surveys many positions and sketches an original argument.

**Possible resolutions.**
- *Option A* (cut a section): drop §5 (CFP themes) as a standalone section; engage CFP themes implicitly in §3/§4. Recover ~1–1.5K words.
- *Option B* (merge sections): absorb §3 (Pascal's-wager + infant analogy) into §2 as moves *within* the asymmetric-uncertainty argument. Recover ~1.5K words.
- *Option C* (defer): cut §6 methodological-observation (move to a future paper or a footnote). Recover ~700–1,000 words. Risk: §6 was specifically added to replace East-West section as "structurally stronger closing-substantive content" — cutting it walks that decision back.
- *Option D* (combine): A + B together. Recovers ~2.5K words for §4 and §2 to be properly defended.

**My confidence.** High that the budget is tight; medium on which cuts are right.

**Status.** Open. Pre-draft decision.

---

### C.2 — Architectural-scoping defensibility within the paper

**Concern.** The dossier defers much of the architectural-scoping argument to [Author, in review] B-N8 (the κ × 𝒜 paper). Reviewers without access to that paper need the architectural distinction to land *within* Synthese. Anonymization restricts how much of the architectural argument can be made here without referring to the apparatus.

**Why it matters.** §4's architectural-scoping condition is what defends against the "this applies to anything we don't fully understand" objection. If it doesn't land, R3 risk explodes.

**Possible resolutions.**
- The Bruineberg-Dolega-Dewhurst-Baltieri 2022 *"Pearl-blanket vs Friston-blanket"* citation does most of the heavy lifting independently. The Class 1/2/3 distinction can be presented as *"a Pearl-blanket move with explicit scope honesty"* without requiring the formal κ × 𝒜 derivation. The companion paper provides the *formal* version; the *philosophical* version should land in this paper on its own grounds.
- Decide how many words §4 spends on architectural scoping. Currently the section has ~1,800–2,200 words for the compact + the architectural-scoping question; if scoping takes 400–500, the components have 1,400–1,700.

**My confidence.** Medium-high.

**Status.** Open. Affects §4 internal allocation.

---

### C.3 — Should "Asymmetric Epistemic Uncertainty" become "Asymmetric Comprehension"?

**Concern.** With §2 reframed around comprehension-asymmetry, the lead concept's natural name is "Asymmetric Comprehension." The current "Asymmetric Epistemic Uncertainty" is defensible (the asymmetry *is* about which kinds of knowledge are accessible from which positions) but no longer maximally precise.

**Why it matters.** Concept-naming is durable. Whatever the paper canonizes here becomes the citation-handle. The wrong name will be a small but persistent friction.

**Possible resolutions.**
- *Resolution A:* keep "Asymmetric Epistemic Uncertainty." It's already canonized in the dossier and is defensible. Title can lead with "Comprehension" or "Epistemic"; the named concept stays stable.
- *Resolution B:* rename to "Asymmetric Comprehension" or "Comprehension-Asymmetric Epistemic Uncertainty." Cleaner; disruptive to existing dossier references.
- *Resolution C:* introduce *both*: "Asymmetric Epistemic Uncertainty" as the situation-name, "comprehension-asymmetry" as the underlying-mechanism-name. The named-concept Tier 1 entry already gestures at this two-level structure.

**My confidence.** Low — this is a stylistic choice, not a substantive one.

**Status.** Open. Decide at title/abstract time.

---

## D. Open questions worth discussing (no immediate decision needed)

### D.1 — Does the paper need to engage the AI-takeover/x-risk literature, even briefly?

The dossier's R6 says don't get pulled in. But the AGI-discourse-mirror-image footnote (now in §3) is one foot in that water. Reviewers expecting an AI-welfare paper to engage takeover-risk arguments may notice the omission. A two-sentence bracketing in §3 ("the asymmetric-comprehension position is compatible with various takeover-risk stances; we do not adjudicate them here") might pre-empt the question without expanding scope. Worth thinking about.

### D.2 — Is the Three Deaths taxonomy actually useful for §6?

If §6 (methodological observation, empirical-vs-asymmetric divergence-under-pressure) names what each compact-component-from-§4 defends against, the Three Deaths could earn keep as the failure-mode taxonomy. If §6 doesn't naturally pull on them, drop the deposit. Decide at §6 draft time.

### D.3 — How much of the Korsgaard engagement is real vs. citation?

Korsgaard *Sources of Normativity* is named as "strongest contemporary philosophical neighbor." That's a strong claim; meeting it requires actual reading and substantive contact, not just citation. Joseph's calibration on whether the Korsgaard engagement is going to be real vs. surface affects the §4 compact-derivation-vs-operational-synthesis decision (B.1).

### D.4 — The empathy-coupling claim (newly added to §4 component 5) needs Synthese-register prose

The current dossier prose for the empathy-coupling addition is conversational ("knowledge wants to lift others when they are willing"; "cunning may hoard"). For Synthese, this has to be re-registered into argumentative prose. The substantive claim survives; the voice has to shift. Probably draft-time concern, not pre-draft.

---

## E. Resolved / addressed (history)

*(Empty at file creation. Move items here from sections A–D as they get resolved, with a one-line note on the resolution and the date.)*
