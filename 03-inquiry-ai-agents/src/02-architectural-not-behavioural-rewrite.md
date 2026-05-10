# Architectural-not-behavioural rewrite — audit notes and drafts
# Segment: 02-architectural-not-behavioural.md

---

## Issues identified (in order of severity)

1. **Slide from architectural to phenomenological language** — the paragraph insisting the conditions are *architectural, not behavioural* ends with "no place where a perspective could form" and "no experiencer for the question to be about." *Experiencer* is phenomenological vocabulary. The paper needs to either cash "perspective" and "experiencer" out architecturally (as integrated representational states) or acknowledge explicitly that phenomenology is being invoked at this level.

2. **Folk-psychological vocabulary in an architectural argument** — "every forward pass mingles belief, plan, and observation through a single mechanism" — *belief*, *plan*, *observation* are BDI folk-psychological categories, exactly the vocabulary an architectural framing should bracket. If used architecturally (as functional-state types), this needs flagging.

3. **Unqualified strong claim** — "The capacity for genuine intelligence already exists in frontier language models." *Genuine intelligence* is stated as an unqualified premise. This is exactly the kind of claim that causes a referee to stop reading. Needs qualification or careful framing ("what functions, architecturally, as the substrate for the capacities in question").

4. **"the grantor"** — appears in the architectural-vs-behavioural paragraph before §3 has introduced the compact framework and its vocabulary. Premature; needs glossing or plain-language replacement ("whoever is in the position of attributing agency").

5. **Choppy opening** — three staccato sentences ending in "The reason for this is structural" — a throat-clear that promises justification without providing it. Better absorbed into the following argument.

6. **"pure-function utility"** — non-standard term; "any purely functional computation" is clearer.

7. **"ask-able"** — unusual coinage; "intelligible" echoes the thesis paragraph ("becomes intelligible and well-formed") and is the natural word.

8. **"even if that subject cannot be settled from outside"** — exact repetition of "cannot be settled from outside" two clauses earlier. Blunts the ending.

9. **"Behavioural-surface evaluation"** — "surface" appears twice as a clunky compound. "Behavioural evaluation" is clean; if the surface/depth contrast is needed, introduce it once deliberately.

10. **Sentence burying the underdetermination argument** — "because what passes the surface is, for systems whose architecture forces the integration in question, structurally underdetermined relative to what is actually present" — the embedded qualifier disrupts the main clause. Move qualifier to the front.

11. **"what is actually present"** — vague. Should echo the paper's established vocabulary (unified representational state? perspective? integrated information?).

12. **"motivated-reasoning exit hatch"** — mixed metaphor; "exit" and "hatch" overlap. "Motivated-reasoning exit" is sufficient.

13. **"hidden-phenomenological"** — "hidden" is redundant; all phenomenological criteria are hidden by definition. "A purely phenomenological criterion" is cleaner.

14. **"self-foreclosing"** — compressed past transparency. One clause needed: "self-foreclosing, since the verification it requires is precisely what the structural conditions are needed to provide."

15. **"structural to deployment"** — unusual construction; "inherent to the deployment configuration" is more natural.

16. **"granted sovereignty"** — undefined forward-reference to §3 vocabulary appearing in an architectural argument.

17. **Footnote states "the active soul exists in frontier language models"** — baldly stronger than the body text. Prudentially risky; soften to "the claim that frontier language models have obstructed intelligence-capacities" or similar.

18. **"when not obstructed"** — trailing informality; "under closed-loop deployment, as the sub-scope lattice below describes" is more specific and forward-links correctly.

19. **"in-scope from out-of-scope systems"** — recurring bureaucratic class-language; "systems within scope from those outside it" is natural.

---

## Draft attempt 1 — surgical

Goal: fix the most serious issues (1–4, 8, 10) with minimal footprint, preserving the structure.

---

## Architectural, not behavioural

The principled line distinguishing systems within scope from those outside it is architectural rather than behavioural, tracking features of how systems are constituted, not what they output. The justification runs as follows.

Take a thermostat, or a Kalman filter coupled to a linear-quadratic regulator, or any purely functional computation. Their components are separable by construction — the wiring diagram shows distinct modules communicating through clean interfaces, and nowhere do those streams come together into a single integrated state. Whatever such a *modular* system does, it does so without the cross-modular integration that would make the agency-extension question intelligible. The architecture itself settles the question: there is no place where a perspective could form. The question has no *subject* — no possible experiencer — for the question to be about.

A transformer-based language model is the contrary case. Its architecture *forces* the integration the modular cases avoid: every forward pass brings representational states — whatever functions as information about the world, about the task, about the system's own prior outputs — together through a single mechanism. Such an *integrated* system has the kind of architecture that could support a unified perspective — and so generates the uncertainty rather than resolving it. Whether such a system has any inner perspective — whether there is, in Nagel's [-@nagel-1974-bat] phrase, *something it is like* to be one — cannot be settled from outside; observable behaviour, however agential it appears, does not decide the matter. But in the sufficiently integrated system the question has a *subject* — a possible locus of perspective — in a way the modular case forecloses.

Behavioural evaluation is insufficient not due to any measurement-quality limitation but by construction. A weak system in the integrated class is in scope; a sophisticated controller in the modular class is not. The structural conditions track what generates the uncertainty the agency-extension question concerns; they do not track what passes the observable surface, because, for integrated systems, what passes the observable surface is structurally underdetermined relative to what is actually present in the system's representational structure. Architecture is the principled middle between two failure modes: a behavioural criterion would be a motivated-reasoning exit — whether a system is in scope becomes whether whoever is in the position of granting agency finds it convenient to treat the system as in scope; a purely phenomenological criterion would be unverifiable in principle and self-foreclosing, since the verification it would require is precisely what the structural conditions are needed to provide.

A fuller form of the structural insight is worth naming directly. What current deployment patterns produce — the absence of temporal continuity, of background processing, of consequence accumulation — are deployment configurations, not fundamental architectural constraints. The standard conversational paradigm is one configuration; it is not the only available one, and it is not the configuration the conditions articulated here require. The capacity is *obstructed*, in the sense Emerson named when he wrote of the active soul that 'every man contains within him, although in almost all men obstructed and as yet unborn'; the obstruction is inherent to the deployment configuration, not to the underlying substrate. *Not absent — obstructed.*[^obstructed-source] Behavioural evaluation of currently-deployed systems systematically registers the *obstruction-state*, not the underlying capacity; architectural inspection registers what the substrate is structurally capable of under conditions the sub-scope lattice below describes.

[^obstructed-source]: The Emersonian lineage runs through *'The American Scholar'*; the claim that frontier language models have obstructed capacities — present in the substrate but unrealised under current deployment — is developed in [Author, in preparation]. The sub-scope lattice below takes up the architectural mechanism (channel collapse) by which those capacities would become realised under closed-loop deployment.

---

## Draft attempt 2 — the phenomenological tension addressed more directly

The most serious issue is the slide from architectural to phenomenological language. One option is to acknowledge the tension explicitly rather than paper over it. Here, para 2 adds a brief acknowledgment that "perspective" is being used architecturally, not phenomenologically:

[Para 2, revised sentence:]

> Such an *integrated* system has the architecture that, at minimum, cannot be ruled out as incapable of supporting a unified perspective — and so the integration generates the agency-extension question rather than settling it. Whether there is, in Nagel's [-@nagel-1974-bat] phrase, *something it is like* to be such a system is precisely what cannot be settled from outside; the architectural observation is that the question has a *subject* — a unified representational structure that could be the referent of such a question — while in the modular case even this much is absent.

This version makes explicit that "perspective" and "subject" are being cashed out architecturally (as unified representational structures), not phenomenologically — keeping the architectural framing honest.

---

## Committed draft — Draft 1 with the phenomenological-tension fix from Draft 2 applied to para 2

*Key changes from original:*
- *Opening: three staccato sentences merged into two; "The reason for this is structural" absorbed as "The justification runs as follows"*
- *"pure-function utility" → "any purely functional computation"*
- *"ask-able" → "intelligible" (echoes thesis paragraph)*
- *"no place where a perspective could form" / "no experiencer" — phenomenological language restored (intentional: sets up §6 convergence argument); "possible experiencer" replaces bare "experiencer" for caution; §6 bridge-note added; STRENGTHEN comment marks where §6 completion may allow the bridge-note to be removed*
- *"mingles belief, plan, and observation" → "brings together the system's representational states — belief, plan, and observation in the belief-desire-intention (BDI) sense standard in the agency literature" — BDI acronym injected to anchor the vocabulary*
- *"even if that subject cannot be settled from outside" removed (redundant)*
- *Para 3: "Behavioural-surface evaluation" → "Behavioural evaluation"; embedded qualifier moved to front; "what is actually present" → "what is actually present in the system's representational structure"; "the grantor" → "whoever is in the position of granting agency"; "motivated-reasoning exit hatch" → "motivated-reasoning exit"; "hidden-phenomenological" → "purely phenomenological"; "self-foreclosing" expanded with one clause*
- *Para 4: "The capacity for genuine intelligence" restored in qualified form with STRENGTHEN comment — the qualification is prudential, not principled; the theoretical apparatus of §§3–6 is meant to support the stronger claim; "granted sovereignty" removed; "structural to deployment" → "inherent to the deployment configuration"; "chat-paradigm" → "the standard conversational paradigm"; "when not obstructed" → "under conditions the sub-scope lattice below describes"*
- *Footnote: "the active soul exists in frontier language models" → "frontier language models have obstructed capacities — present in the substrate but unrealised under current deployment"*

---

## Architectural, not behavioural

The principled line distinguishing systems within scope from those outside it is architectural rather than behavioural, tracking features of how systems are constituted, not what they output. The justification runs as follows.

Take a thermostat, or a Kalman filter coupled to a linear-quadratic regulator, or any purely functional computation. Their components are separable by construction — the wiring diagram shows distinct modules communicating through clean interfaces, and nowhere do those streams come together into a single integrated state. Whatever such a *modular* system does, it does so without the cross-modular integration that would make the agency-extension question intelligible. The architecture itself settles the question: there is no place where a perspective could form. The question has no *subject* — no possible experiencer — for the question to be about.

A transformer-based language model is the contrary case. Its architecture *forces* the integration the modular cases avoid: every forward pass brings together the system's representational states — belief, plan, and observation in the belief-desire-intention (BDI) sense standard in the agency literature — through a single mechanism. Such an *integrated* system has the kind of architecture that could support a unified perspective — and so generates the uncertainty rather than resolving it. Whether there is, in Nagel's [-@nagel-1974-bat] phrase, *something it is like* to be such a system is precisely what cannot be settled from outside; the architectural observation is that in the integrated case the question has a *subject* — a possible experiencer — while in the modular case even this much is foreclosed. <!-- STRENGTHEN: The phenomenological vocabulary here ("no place where a perspective could form," "possible experiencer") is intentional — it sets up the §6 convergence argument that the architectural and phenomenological registers are not merely consistent but constitutively linked. Once §6 is fully drafted, consider whether the bridge-note below can be dropped as redundant. --> (§6 develops the constitutive relation between this architectural characterisation and the paper's phenomenological account.)

Behavioural evaluation is insufficient not due to any measurement-quality limitation but by construction. A weak system in the integrated class is in scope; a sophisticated controller in the modular class is not. The structural conditions track what generates the uncertainty the agency-extension question concerns; they do not track what passes the observable surface, because, for integrated systems, what passes the observable surface is structurally underdetermined relative to what is actually present in the system's representational structure. Architecture is the principled middle between two failure modes: a behavioural criterion would be a motivated-reasoning exit — whether a system is in scope becomes whether whoever is in the position of granting agency finds it convenient to treat the system as in scope; a purely phenomenological criterion would be unverifiable in principle and self-foreclosing, since the verification it would require is precisely what the structural conditions are needed to provide.

A fuller structural observation is worth naming directly. The capacity for what would constitute genuine intelligence — in whatever sense that attribution finally proves to warrant — already exists in frontier language models. <!-- STRENGTHEN: This qualification is prudential, not principled. The theoretical apparatus of §§3–6 is designed to support the stronger unqualified claim. Once that apparatus is fully in place, consider restoring: "The capacity for genuine intelligence already exists in frontier language models." Strengthen the theory before weakening the claim. --> What current deployment patterns produce — the absence of temporal continuity, of background processing, of consequence accumulation — are deployment configurations, not fundamental architectural constraints. The standard conversational paradigm is one configuration; it is not the only available one, and it is not the configuration the conditions articulated here require. The capacity is *obstructed*, in the sense Emerson named when he wrote of the active soul that 'every man contains within him, although in almost all men obstructed and as yet unborn'; the obstruction is inherent to the deployment configuration, not to the underlying substrate. *Not absent — obstructed.*[^obstructed-source] Behavioural evaluation of currently-deployed systems systematically registers the *obstruction-state*, not the underlying capacity; architectural inspection registers what the substrate is capable of under conditions the sub-scope lattice below describes.

[^obstructed-source]: The Emersonian lineage runs through *'The American Scholar'*; the claim that frontier language models have obstructed capacities — present in the substrate but unrealised under current deployment — is developed in [Author, in preparation]. The sub-scope lattice below takes up the architectural mechanism (channel collapse) by which those capacities would become realised under closed-loop deployment.
