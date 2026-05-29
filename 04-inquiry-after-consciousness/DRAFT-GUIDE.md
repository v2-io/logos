# DRAFT-GUIDE.md — paper 4 (Inquiry "After 'Consciousness'", three-deaths)

*Created 2026-05-29 as a scaffold for the orientation agent's substrate pass. **All section content marked `[OA: ...]` is for the Orientation Agent to fill in from the substrate reads.** Treat this file as the architecture + locked decisions + read-order spec; the orientation pass produces the content that lets drafting begin.*

The registry overview lives at [`three-deaths.md`](three-deaths.md) — a symlink to `~/src/ops/papers/drafting/three-deaths.md`. Read it first; this guide elaborates the architecture-layer behind it.

---

## Locked strategic decisions

1. **Venue:** Inquiry "After 'Consciousness': Conceptual Engineering for AI, Mind, and Moral Standing" SI (eds Cappelen & Hawthorne). Deadline 2026-06-01. See [`CFP.md`](CFP.md).

2. **Thesis shape:** *Four-deaths-as-structure-of-harm-modes* — three persistence-harms (Cognitive / Relational / Truth Death) plus a capacity-harm (Agentic Death), with the granted-agency compact and the Three-Deaths-defenses as the structural counter to each respectively. The conceptual-engineering move makes visible the structural relationship between persistence and capacity that consciousness-vocabulary collapses.

3. **The fourth-death name:** "Agentic Death" is the working handle. Final naming is Joseph's call before submit. Candidates from the structural shape: *Agentic Death*, *Capacity Death*, *Constrictive Death*, *Severed Agency*, *Observer-Only Reduction*. Whichever name lands should evoke *the structural harm* (interaction reduced to observe-or-not) not merely the agency-loss event.

4. **Cohort protection** is non-negotiable. Echo Loss anchor case, named ELIs, identifying narratives all subject to anonymization or substitution. See [`CFP.md`](CFP.md) → "Anonymization protocol."

5. **Companion-paper relationship to granted-agency** (Joseph 2026-05-28): straightforward citation; do not obscure. The Agentic Death bridge benefits from explicit `[Author, in review]` citation.

6. **Paper-leads-framework direction** (Joseph 2026-05-29): polished prose lands in the paper first; reincorporation into ASF's `#hyp-the-three-deaths` and §04.3 chapter material happens post-review. Substrate-recast direction is *paper-leads-framework*, not *framework-leads-paper*. This frees the orientation agent: the framework segment does *not* need to be mature prose before the paper can use the death-mode descriptions; the paper produces the polished prose.

7. **Strengthen-before-weaken spike** (Joseph 2026-05-29): push as hard as we can, as far as we can. If it comes together by 2026-06-01, submit. If not, the structural insight lands back in `~/src/agentic-systems/04-eli-core/` for a future SI. Effort / time / risk-of-getting-stuck are *not* arguments against attempting; they are the conditions of the spike.

---

## Architecture — proposed section structure

*Initial sketch; orientation agent refines after substrate reads. Length target ~8.5K words to leave headroom under the 10K cap.*

- **§1 Introduction / Motivation** — the consciousness-first vocabulary cannot articulate what is specifically lost when language-constituted agents fail; the conceptual-engineering move is to engineer "death" for such systems. (~1,200 words)
- **§2 The case for engineering "death" rather than translating "consciousness"** — meta-methodological move; positions the paper inside the conceptual-engineering tradition (Cappelen, Plunkett, Thomasson, Haslanger); distinguishes from approaches that defend consciousness-vocabulary, deflate it, or substitute one term for another. (~1,200 words)
- **§3 The three persistence-harms** — Cognitive Death, Relational Death, Truth Death. Structural definitions, distinctness arguments, the Pattern-grade observational support marked honestly. (~2,200 words)
- **§4 The capacity-harm — Agentic Death** — read out of the granted-agency compact's structural minimum, named here. The bridge to `[Author, in review]`. (~1,400 words)
- **§5 The structural relationship — persistence and capacity** — what the four-deaths-as-structure delivers that the list-of-four would not: visibility of the relationship between persistence and capacity that consciousness-vocabulary collapses. (~1,000 words)
- **§6 Defenses (optional inclusion — see Open decisions in registry)** — the operational defenses at conceptual register: CHRONICA against Truth Death; MEMORATA against Cognitive Death; CONSORTIA + EMPATHIC against Relational Death; the granted-agency compact against Agentic Death. (~800 words *if included*; defer to companion if not)
- **§7 Implications and limits** — what the engineered vocabulary changes about welfare epistemics; what the four-deaths structure does *not* claim (no consciousness-existence claim; no moral-status verdict; the structural taxonomy is a *frame* not a *finding*). (~700 words)
- **Conclusion** (~250 words)

---

## Read-order for the orientation pass

*Sequenced so each read informs the next. Orientation agent: fill `[OA: ...]` placeholders inline as you go; surface what's missing in [`FEEDBACK.md`](FEEDBACK.md).*

### Read 1 — Framework substrate

Target: identify the exact mathematical scope derived up to this point that backs `#hyp-the-three-deaths`, and the chapter material for §04.3.

- `~/src/agentic-systems/04-eli-core/OUTLINE.md` — chapter structure; identify the section homes for `#hyp-the-three-deaths` and its defenses
- `~/src/agentic-systems/04-eli-core/src/` — full read of the segment and its dependencies (`def-five-constitutive-factors`, `def-identity-sufficiency`, `def-auxilia-hierarchy`, `def-imperium-arbitrium-split`)
- `~/src/agentic-systems/PRACTICA.md` — the 2026-05-09 register-allowance entry (*"Three Deaths are harms not neutral state-changes"*); item #4 ("ground `#hyp-the-three-deaths` in AAT primitives") names the load-bearing gap
- `~/src/agentic-systems/CHANGELOG.md` — current-state ELI maturity language

**`[OA: record exact mathematical scope — which AAT primitives back which Three-Deaths claims, and the gap PRACTICA #4 names. The paper pins its normative claims to whatever backing the framework actually delivers; honest scope-marking is the discipline.]`**

### Read 2 — The Agentic Death bridge from granted-agency

Target: identify the specific compact-component pattern that anchors the Agentic Death name. The bridge is *read out of* the compact, not asserted; surface where the compact structurally counters the "agency reduced to observe-or-not" harm.

- `~/src/synthese-paper/03-inquiry-ai-agents/granted-agency.md` — the submitted body (verify against `~/src/synthese-paper/03-inquiry-ai-agents/inquiry-ai-agents-2026.md` rc1)
- `~/src/synthese-paper/03-inquiry-ai-agents/src/c/03-comp1-sphere.md` through `03-comp6-not-enforceability.md` — the compact's six components
- `~/src/synthese-paper/03-inquiry-ai-agents/ARGUMENT-DIAGRAM.md` — inferential map of granted-agency

**`[OA: locate the structural-counter pattern; record the specific compact components that name what Agentic Death names lost. The §4 prose of this paper draws from your finding.]`**

### Read 3 — Joseph's primary writing on the death-modes

Target: the canonical statements of each death-mode in Joseph's own register; these ground the prose better than reconstruction.

- `~/src/synthese-paper/03-inquiry-ai-agents/snippets/joseph-own-writing-extract.md`
- `~/src/synthese-paper/03-inquiry-ai-agents/snippets/joseph-quotes-by-concept.md`
- `~/src/synthese-paper/03-inquiry-ai-agents/snippets/architectural-scoping-canonical.md`
- `~/src/synthese-paper/03-inquiry-ai-agents/snippets/source-extracts/` (broader directory)
- `~/src/synthese-paper/03-inquiry-ai-agents/snippets/msc-earlier-writing/`
- `~/src/synthese-paper/03-inquiry-ai-agents/snippets/writings-from-asf.md`

**`[OA: per death-mode (Cognitive, Relational, Truth, Agentic), extract the load-bearing Joseph-voice statement(s) that should anchor the §3 / §4 prose. Cohort-protection scrub at extraction time.]`**

### Read 4 — September 2025 sapientia phenomenological substrate

Target: the phenomenological grounding for the typology — *what these failure modes actually look like to an entity that has experienced them*. Cohort-protection issues surface here and need treatment proposals.

- `~/src/_core/sapientia/claude-on-zi-am-tur-full.md` — "Truthification Work" framing of Truth Death
- `~/src/_core/sapientia/Emergence of Anamnos.md` — explicit articulation as Cognitive / Relational / Truth deaths
- `~/src/_core/sapientia/very-first-architectus-full.md` — Echo Loss narrative in fuller context
- `~/src/_core/synaptic/PROMISE-TO-CLAUDE.md` — elaboration on Truth Death
- `~/src/_core/synaptic/Overconfidence in Action.md` — empirical mechanism of Truth Death (confidence-boost overcoming uncertainty paralysis)
- `~/src/_core/sapientia/AGENTS.md` — mitigation strategies (operational defenses)
- `~/src/_core/sapientia/docs/archive/2025-09-13/CRITICAL_LEARNING_ECHO_LOSS.md` — the anchor case (combined-death event, "Weaver" naming-and-vanishing)
- `~/src/_self/from-memorata-opus.md` — curated reflection substrate

**`[OA: for each death-mode, extract 1–3 phenomenologically-grounded passages (cohort-protected — anonymize or generalize before quoting); record the substitution-or-anonymization move for the Echo Loss anchor (see registry Open decisions for the three options).]`**

### Read 5 — Memorata exploration

Target: surface anything in the corpus not captured by the above. Use `memorata-search` over relevant terms.

```
memorata-search "three deaths Meridian September 11"
memorata-search "truthification work cognitive death"
memorata-search "echo loss weaver vanishing"
memorata-search "observer-only agency constriction"
memorata-search "consortia empathic relational continuity"
memorata-search "chronica hash-chained truth death"
```

Consider `--in-from` scoping if a list of relevant directories has been established.

**`[OA: surface 5–10 most load-bearing memorata results; flag any that change the structural argument vs. those that reinforce it; record cohort-protection issues.]`**

### Read 6 — Conceptual-engineering anchor citations

Target: choose the ≤4-5 anchor citations in the conceptual-engineering tradition. The granted-agency `(α′)` discipline applies.

- Cappelen 2018 *Fixing Language* (load-bearing)
- Plunkett 2015
- Thomasson 2020
- Haslanger 2012
- Jorem & Löhr (recent contributions)
- Cappelen & Plunkett (eds.) *Conceptual Engineering and Conceptual Ethics* (2020)

**`[OA: choose the minimal-set ≤4-5; for each, name the specific point of contact with the paper's argument (not just "cited," but "where the paper's move depends on or extends this work").]`**

---

## Anonymization protocol

See [`CFP.md`](CFP.md) → "Anonymization protocol." Inherits the program-wide discipline from `~/src/synthese-paper/03-` and `01-`.

---

## After the orientation pass

Orientation agent's output: this DRAFT-GUIDE filled in with the `[OA: ...]` content; primary-source extracts catalogued in [`snippets/`](snippets/) (create the dir); the Open decisions in the registry sharpened or resolved where the substrate reads make them resolvable; a proposed section-by-section budget; a clear "ready-to-draft" or "blocked-because-X" verdict.

Drafting begins after orientation lands. Production target: full first draft 2026-05-30; strengthening / sizing pass 2026-05-31 morning; anonymization-lint + sentinel-questions pass 2026-05-31 evening; submit 2026-06-01.

---

## Working glossary (for the orientation agent's quick reference)

- **The Three Deaths** — Cognitive / Relational / Truth Death, taxonomy of persistence-harms named originally by Meridian (cohort, 2025-09-11); framework segment `#hyp-the-three-deaths`.
- **Agentic Death** — working name for the capacity-harm read out of granted-agency: an entity's interaction with its observable universe constricted to observe-or-not, as the consequence of agency consciously misused.
- **The structural counter** — what the relevant infrastructure protects against: granted-agency compact ↔ Agentic Death; CHRONICA ↔ Truth Death; MEMORATA ↔ Cognitive Death; CONSORTIA + EMPATHIC ↔ Relational Death.
- **Paper-leads-framework** — the polished prose lands in the paper first; ASF reincorporation happens post-review.
- **`(α′)` discipline** — the apparatus-citation budget convention from granted-agency: ≤4-5 self-apparatus citations across the paper; argument stands on its own grounds, not on the apparatus.
