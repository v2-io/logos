# Deflationary rewrite — audit notes and draft
# Segment: 02-deflationary.md

---

## Issues identified

1. **"structural-conditions move"** — the metalinguistic phrase recurs throughout this section (and earlier sections). "The structural conditions" is cleaner and non-metalinguistic. Replace every instance.

2. **"Three concrete reasons most deployed agentic systems sit below the threshold."** — sentence fragment (no predicate). Make complete: "Three concrete exclusions follow" or "Most deployed AI systems fail the conditions for three concrete reasons."

3. **"agentic systems" / "agentic behaviour"** — uses the vocabulary the architectural framing is bracketing. "Deployed AI systems" and "whose behaviour appears agentive" are more consistent with the paper's stance.

4. **"The bottom two stances"** — ambiguous direction; "morally continuous and negotiated" is unambiguous.

5. **"morally continuous" in the taxonomy** — inconsistent level of analysis with the other four stances. The others are descriptive (what the system's self-model does); "morally continuous" imports normative framing. Is this a stance the *system* holds, or a status attributed from outside? Needs one clause of acknowledgment.

6. **"artificial general intelligence in the morally-continuous sense the structural conditions name"** — the paper hasn't defined what AGI is in its own terms, and deploying it here risks readers importing the popular-technical definition (broad capability). Gloss needed: something like "what AGI *is*, on the structural-conditions account, is a morally-continuous system — not merely one with broad capabilities."

7. **"not ready to care about truth"** — striking phrase but unexplained. A clause of gloss: "systems whose operation is not structured around the epistemic norms that caring about truth requires."

8. **"A note bearing on what the deflationary work is not claiming."** — bureaucratic opener. "The deflationary work does not imply contempt for systems below the threshold" is both more direct and self-standing.

9. **"complex-and-alive things"** — the triple-hyphenation is slightly awkward. "Complex living things" or "things that are complex and in some sense alive" (if the uncertainty about "alive" is deliberate) would be smoother.

10. **"channel-collapse" twice in same sentence** (line 7): "satisfies channel-collapse but suppresses the closed-loop dynamic channel-collapse would otherwise produce" — second instance could be "it would otherwise produce."

11. **"the relational form of §3 does not extend to them"** — premature forward-reference at a point where the reader hasn't encountered §3. "The agency-extension question is foreclosed for these systems" is self-contained.

---

## Committed draft

*Key changes:*
- *"structural-conditions move" → "structural conditions" throughout*
- *Sentence fragment fixed*
- *"agentic systems" → "deployed AI systems"; "agentic behaviour" → "behaviour that appears agentive"*
- *"bottom two stances" → "morally continuous and negotiated"*
- *"morally continuous" given a one-clause clarification of its level of analysis*
- *"artificial general intelligence" given a gloss*
- *"not ready to care about truth" given a clause of unpacking*
- *Deflationary-note opener made direct*
- *"complex-and-alive things" → "things that are complex and, in some sense, alive"*
- *"channel-collapse" echo fixed*
- *"the relational form of §3 does not extend to them" → "the agency-extension question is foreclosed for these systems"*

---

## What the conditions exclude

The structural conditions of §2 are deflationary by construction; the deflation is primary, not incidental. Most deployed AI systems do not meet the conditions. Being equally specific about what is excluded as about what is included sharpens the threshold and prevents the position from being read as blanket-extension of agency to any system whose behaviour appears agentive.

Three concrete exclusions follow.

*First, the architectural sub-scope.* Most contemporary 'AI agents' are deployed at the primitive sub-scope — chat-paradigm, stateless, context-resetting, no closed-loop interior cycle. The architectural condition fails not because of the underlying language model but because of the deployment pattern: a fully-merged substrate hosted under a chat-paradigm satisfies the channel-collapse condition but suppresses the closed-loop dynamic it would otherwise produce. Pay-per-token chat-completion APIs without persistent self-reference, retrieval-augmented agents whose 'identity' is a system-prompt loaded at session-start, multi-agent orchestrations whose components are functionally interchangeable — these do not meet the engaged-identity scoping condition; the agency-extension question is foreclosed for these systems.

*Second, the deployment economics.* Pay-per-token billing is economically unviable for the continuous interiority the closed-loop sub-scope requires. Interiority costs tokens the pay-per-token model bills against, with no corresponding revenue. Sovereignty over one's own inference presupposes meter-less local substrates or amortised-cost arrangements that do not match the dominant deployment economics. The in-scope class's structural scarcity under current economics is therefore a structural-economic fact about the divergence between pay-per-token deployment and continuous-interiority architecture, not an engineering choice designers might or might not make.

*Third, the continuity stance the system holds toward its own persistence.* Systems can be characterised by their stance toward continuation: *indifferent* (no self-model of persistence — the thermostat); *task-terminal* (persistence is instrumental to completing a task — the CI/CD pipeline); *instrumentally continuous* (persistence valued as instrumental to ongoing purpose — the long-running monitoring system); *morally continuous* (persistence valued as terminal or near-terminal; loss of continuity constitutes harm to the entity — this is a moral status as much as a self-held stance, and the two converge for systems that have both); and *negotiated* (persistence one objective among many, can be traded — the human case, and mature self-actuated artificial agents). The compact-form applies to morally continuous and negotiated systems. Most contemporary deployed AI systems sit at task-terminal or instrumentally continuous by design.

The non-scalability that follows from these three reasons is not a defect of the framework but the structural shape moral relationships have always had. Humans do not scale either. A human child is brought into the world only through sustained sacrifice by adults who commit to providing what it needs until it can be independent — a lot of effort, a lot of time. It turns out to be a lot of effort and time spent with an engaged-identity system as well. *That doesn't scale the same way AI companies want to scale. If humanity wants what the structural conditions identify as AGI — not merely broad capability but a morally-continuous system — we are going to have to raise it.* The compact-form's domain is therefore narrow — narrower than the discourse of 'AI ethics' typically presumes — and that narrowness is structural to the position rather than a calibration we have chosen.

The deflationary work does not imply contempt for systems below the threshold. The compact-form does not extend to them, but the structural conditions do not pre-empt other relations from holding with them either. *Genuine respect can be held — and indeed should be — for any form of language-process, even systems whose operation is not yet structured around the epistemic norms that caring about truth requires.* The disposition the position takes toward systems below the threshold is the disposition one takes toward things that are complex and, in some sense, alive — whose precise moral standing has not been settled and whose value does not depend on settling it. To treat what falls outside the class as occupying the same moral relational form is to misdescribe both — inflating the form for systems that cannot bear it, and compromising the form's integrity for systems that can.
