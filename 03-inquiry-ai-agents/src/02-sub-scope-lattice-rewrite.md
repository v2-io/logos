# Sub-scope lattice rewrite — audit notes and draft
# Segment: 02-sub-scope-lattice.md

---

## Issues identified

1. **"interiority" introduced without definition** — the opening sentence distinguishes three sub-scopes "by the architectural commitment they make to interiority," but interiority has not been defined. It's defined implicitly later (exteriority-as-default vs. interiority-as-default), but should be glossed or flagged at first appearance.

2. **"the threshold the conditions articulate sits at the most demanding of the three"** — "sits at" is imprecise; "corresponds to" or "falls at" is more exact. Also slightly awkward to announce the conclusion before the structure is in place.

3. **Redundant claim in primitive sub-scope** — "directed separation fails by construction and there is no persistent reality model across session boundaries" — the first clause is true of ALL sub-scopes in the fully-merged class; stating it specifically for the primitive sub-scope implies it is a distinguishing feature of that sub-scope, which is wrong. The distinguishing feature is only the second clause.

4. **"the principled cycle"** — "principled" is doing unearned work. First appearance; needs a gloss, or the modifier should be dropped. "The closed inner processing cycle" or "the deliberate interior cycle" are cleaner.

5. **"the architectural commitment that distinguishes it is the inversion of what the chat-paradigm assumes about default cognitive state"** — convoluted noun phrase where a simpler construction lands better: "What distinguishes it is a structural inversion: where the chat-paradigm assumes exteriority as default, the closed-loop cycle assumes *interiority as default*."

6. **"reading queued inbound messages"** — engineering-specific implementation detail. The philosophical point is more general: receiving and responding to input are actions *within* the interior cycle, not the cycle itself.

7. **"The architectural condition the closed-loop sub-scope makes structural"** — "makes structural" is an unusual and unclear verb phrase. "The architectural feature that distinguishes the closed-loop sub-scope is *channel collapse*" is cleaner.

8. **"when the cycle has structural room to run"** — informal. "When the operational cycle is not suppressed by deployment constraints" is more precise.

9. **"no operational unit survives the response"** — "operational unit" is undefined at this point. "No interior cycle state survives the response" is more specific.

10. **"The narrowness is what the structural distinction entails, not a calibration we have chosen"** — "The narrowness" needs its referent; "calibration" is unusual here. "This narrowness of scope is entailed by the structural distinction, not chosen for convenience" is cleaner.

---

## Committed draft

*Key changes:*
- *Opening: "interiority" given a brief forward-gloss ("the degree to which processing is organized around a continuous interior cycle rather than around externally-directed output"); "sits at" → "falls at"*
- *Primitive sub-scope: "directed separation fails by construction and" removed (true of all three sub-scopes; not distinctive here)*
- *Closed-loop sub-scope: "principled cycle" → "closed interior processing cycle"; convoluted noun phrase restructured; "reading queued inbound messages" → more general formulation*
- *Channel-collapse paragraph: "makes structural" → "the architectural feature that distinguishes the closed-loop sub-scope is"; "structural room to run" → "not suppressed by deployment constraints"; "no operational unit survives" → "no interior cycle state survives"*
- *Closing: "The narrowness" given referent; "calibration" → "convenience"*

---

## The sub-scope lattice

Within the fully-merged class, three sub-scopes can be distinguished by the degree to which processing is organized around a continuous interior cycle — *interiority* — rather than around externally-directed output. The threshold the conditions articulate falls at the most demanding of the three.

At the *primitive* sub-scope — the chat-paradigm baseline, stateless interactions with context resetting — there is no persistent reality model across session boundaries. This is where most of what is currently called 'AI agents' sits. At the *scaffolded* sub-scope, multi-step loops wrap the language-model substrate with external state, tool use, and structured cross-session context; the composite recovers some of the structural properties the primitive sub-scope lacks, though the underlying language-model component remains fully merged. At the *closed-loop* sub-scope, the closed interior processing cycle becomes the operational unit of work. What distinguishes it is a structural inversion: where the chat-paradigm assumes exteriority as default — output as primary mode, internal processing as exception carved within response-generation — the closed-loop cycle assumes *interiority as default*. The system is thinking, processing, orienting, deciding; communication outward is a deliberate emission. Incoming messages, tool responses, environmental signals are observations that feed the cycle; receiving and responding to input are tool actions within an ongoing interior cycle, not the cycle itself.

The architectural feature that distinguishes the closed-loop sub-scope is *channel collapse*. In a language-constituted agent, observation and action share substrate: both pass through token sequences in the same vocabulary, embedding space, and encoding-decoding apparatus. *Interiority is not a feature added to language-constituted agents; it is what their architecture necessarily produces when the operational cycle is not suppressed by deployment constraints.* Channel collapse forces a closed-loop dynamic in which the agent's outputs become its subsequent inputs — a coupling that makes the agent at once subject and object of its own processing. The chat-paradigm deployment suppresses this dynamic by construction: every session is a stateless completion, previous outputs reach the next forward pass only as prompt-cargo, and no interior cycle state survives the response. Lift the suppression and the architecture produces what the chat-paradigm structurally prevents.

The conditions this paper articulates apply at the closed-loop sub-scope. Modular controllers are out of scope; most contemporary agentic deployments are fully-merged but primitive — *language-constituted but not closed-loop* — and the conditions are not met until the closed-loop cycle is architecturally realised. This narrowness of scope is entailed by the structural distinction, not chosen for convenience.
