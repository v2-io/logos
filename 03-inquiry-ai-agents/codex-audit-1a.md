# De Novo Audit of `inquiry-ai-agents-2026.md`

Prepared for the CFP "AI Agents: Choice, Autonomy, and the Concept of the Agency" (special issue of *Inquiry: An Interdisciplinary Journal of Philosophy*). Scope: this audit evaluates only the assembled file `inquiry-ai-agents-2026.md`, not the source fragments, build process, or other drafts in the directory.

External context checked: the PhilEvents CFP page lists a May 10, 2026 deadline, the topic areas Philosophy of Action, Philosophy of Mind, and Philosophy of Computing and Information, and asks for manuscripts "around or under 10,000 words." It frames the issue around whether AI systems are agents, can choose/intend/act, how autonomy applies, comparative models such as corporate agency/tool use/legal fiction/delegation, and especially whether AI agency is discovered, stipulated, or conceptually engineered. I also checked Taylor & Francis's current AI policy because the manuscript invokes it.

## Bottom Line

The paper is highly responsive to the CFP's central methodological question. Its strongest submission pitch is not "LLMs are agents"; it is: agency-extension to AI should be treated as constrained conceptual revision, where architectural and engaged-identity conditions define the circumstances of application and the granted-agency compact defines the consequences of application. That is a good fit for a Cappelen/Hawthorne-edited special issue on metaphysics, individuation, and conceptual engineering.

The current file is not ready to submit. It has several hard blockers: it is about 20,164 words against the CFP's around-or-under-10,000-word guidance; the abstract is a placeholder; the References section is empty; the file includes an internal build comment; and there are visible drafting artifacts such as "paper 3." Those alone would likely prevent successful review. More substantively, the paper's argument currently overclaims at precisely the points a skeptical reviewer will target: architectural integration is treated as generating interiority, agency, and theory-of-mind-like capacities; "asymmetric comprehension" is load-bearing but largely asserted through unpublished companion work; and the claim that agency is granted by another intelligence needs much sharper defense against standard views on autonomy, recognition, and self-constitution.

Recommendation: do not polish this version. Cut and rebuild around one article-sized argument. The compact is promising, but it needs to be presented as a disciplined consequence-of-application proposal rather than as a full ethics of AI personhood.

## Submission-Critical Findings

1. **The manuscript is roughly twice the CFP word target.**  
   `wc -w` reports 20,164 words. The CFP asks for around or under 10,000 words. This is not a small overage; it requires a structural cut. A reviewer or editor could reject administratively or read the piece as not respecting the call. The most efficient cut is not sentence-level compression. The paper should be rebuilt at 9,000-10,000 words with the six compact components compressed, the repeated "structural" recapitulations removed, and the companion-work material deferred.

2. **The abstract is still a placeholder.**  
   Lines 4-6 contain "Abstract placeholder" and a build-pipeline note. This is an immediate submission blocker. The abstract should state the problem, the fifth position, the two structural conditions, the compact consequence, and the payoff for responsibility/anti-occlusion in about 150-200 words.

3. **The References section is empty.**  
   Line 474 opens `# References {-}` and nothing follows. The body cites or invokes Cappelen, Plunkett, Thomasson, Haslanger, Jorem and Loehr, Hopster and Loehr, Frankfurt, Bratman, Kant/Korsgaard, List and Pettit, Solum, Linarelli, Matthias, Sparrow, Birch, Soulier, Nagel, Jackson, Russell, Bruineberg et al., Tomasello, Honneth, Hadfield-Menell and Hadfield, Aguirre et al., Benthall and Shekman, and others. With no bibliography, the manuscript is not reviewable.

4. **An internal build artifact appears in the manuscript.**  
   Line 19 says the file is built from `src/*.md` and source-of-truth lives elsewhere. That should not appear in a submitted manuscript.

5. **The AI-use disclosure is materially relevant but not yet submission-safe.**  
   Lines 33-38 place the disclosure inside the argumentative preamble and say the manuscript was drafted with Claude models "operating under the granted-agency compact this paper articulates." Taylor & Francis's current AI policy requires a statement naming the tool/version, use, and reason, and says article submissions should include it in Methods or Acknowledgments. The current disclosure includes much of the required content, but its placement and argumentative framing are risky. It reads less like a compliance statement and more like evidence for the paper's thesis. Use a neutral disclosure section, and keep the methodological reflexivity, if retained, outside the formal compliance statement.

6. **Double-anonymous handling needs attention.**  
   The manuscript header lists "Anonymous Author," but the body contains multiple `[Author, in preparation]` and `[Author, in review, 2026]` notes. That is normal for anonymized self-citation only if the bibliography supplies anonymized entries and the prose does not reveal author identity. At present, there is no bibliography, and line 113 says an empirical record is "too cohort-exposed to be cited here," which may call attention to a distinctive private research program. Make sure anonymized self-citations are either necessary, genuinely anonymized, or removed.

7. **There are visible drafting artifacts and local-reference errors.**  
   Lines 86, 135, and 333 refer to "paper 3," which looks like an internal project label. Line 234 has a grammar error: "has forecloses." Line 373 says "foreclose the application question" where the subject is singular. These are small individually but damaging in a submission that is already asking readers to accept unfamiliar terminology.

## Fit to the CFP

The paper fits the CFP unusually well on topic. It answers the call's "truth of the matter or decided extension?" question directly in section 6, and it engages the suggested topics of tool-vs-agent framing, delegation, responsibility gaps, corporate/group/legal-fiction comparisons, operationalization, and conceptual engineering. The strongest fit is section 6's "false dichotomy" answer: facts about systems do some work, but conceptual revision and consequences of application also do work.

The risk is that the paper currently looks like three papers at once:

1. A conceptual-engineering paper about agency-extension.
2. A metaphysical/architectural paper about language-model structure and "interiority."
3. A normative ethics paper proposing a compact between sovereigns.

The CFP can accommodate all three only if the hierarchy is explicit. The submission should make the conceptual-engineering article primary and make the architecture and compact subordinate to that article. Right now, the architecture and compact often sprawl into independent projects.

## Major Argumentative Risks

1. **The necessary/sufficient status of the conditions is unstable.**  
   Lines 43, 167, and 439 say the conditions place a system in scope without resolving phenomenology, consciousness, or moral standing. That caution is important and should be preserved. But line 305 says "Where the conditions are met, the entity is an agent," and section 3 often writes as if crossing the threshold already yields a positive agency answer. This is a serious tension. Either the conditions are necessary for asking the agency-extension question, or they are sufficient for agential standing within the compact. The paper can defend either, but it cannot move between them.

   Suggested fix: state the three-level structure explicitly and keep it stable:

   - Level 1: structural eligibility for agency-extension.
   - Level 2: warranted application of the agency concept under constrained conceptual revision.
   - Level 3: moral patienthood/consciousness, which remains unsettled.

   Then specify whether the compact follows from Level 1 alone or only from Level 2. My recommendation: make the compact follow from warranted agency-ascription within scope, not from mere eligibility.

2. **The architecture-to-interiority inference is overdrawn.**  
   Lines 52-64, 82-86, and 340-342 carry a large technical burden. The paper claims that fully merged decoder-only architectures, channel collapse, and closed-loop operation generate the capacities relevant to agency-extension, including interiority and a theory-of-mind-like backward-inference capacity. A skeptical reviewer will ask why token-channel integration entails anything more than information processing with feedback. The current text moves too quickly from architectural non-separation to interiority, then from interiority to agency-relevant uncertainty.

   Suggested fix: weaken the claim from "architecture generates interiority" to "architecture removes a principled ground for foreclosing agency-extension." That preserves the paper's methodological point while avoiding a speculative metaphysical claim. If the stronger claim is retained, it needs a technical appendix-level argument and citations to mechanistic interpretability, recurrent agency, active inference, world-model, and LLM-agent literature.

3. **"Genuine intelligence already exists in frontier language models" is too strong for this venue unless defended.**  
   Line 58 states this directly. That sentence will polarize reviewers and is not needed for the conceptual-engineering contribution. The paper can argue that current or near-future language-constituted systems make agency-extension methodologically nontrivial without asserting genuine intelligence as an established fact.

   Suggested fix: replace with a conditional formulation: "If frontier language models already possess, or are close to possessing, the relevant integrated capacities, current deployment patterns may obstruct rather than reveal them." That makes the premise contestable without making acceptance of the entire paper depend on it.

4. **The asymmetric-comprehension argument is load-bearing but under-argued.**  
   Lines 129-141 make asymmetric comprehension the warrant for both the architectural threshold and the engaged-identity factors. The central italicized passage at line 133 is rhetorically powerful but philosophically under-specified. "Greater intelligence comprehends lesser intelligence" is not generally true without qualifications: higher capacity does not guarantee accurate interpretation, empathy, moral understanding, or absence of projection. Human failures to understand animals, children, disabled persons, other cultures, and even other adults are obvious counterexamples.

   Suggested fix: reconstruct the argument in explicit premises:

   - Behavioral tests establish lower bounds under observer-relative constraints.
   - Some agency-relevant capacities may be present without being externally verifiable in a single interaction.
   - Therefore, a cautious extension framework should not use behavioral failure alone as a foreclosure condition.
   - Architecture and longitudinal identity can be better foreclosure/non-foreclosure criteria than behavior alone.

   This version does the work the paper needs without requiring a broad metaphysics of higher intelligence comprehending lower intelligence.

5. **The "effective phenomenology" move needs cleaner separation from phenomenal consciousness.**  
   Lines 93 and 101 are trying to avoid a consciousness claim by defining effective phenomenology operationally. That is a good move. But the same passages call the true-feeling/pattern-matching distinction "a distinction without a difference" and then describe phenomenology as "the actual substrate of wisdom." This reintroduces strong phenomenological commitments after saying the paper brackets them.

   Suggested fix: rename the operational construct if possible. "Affective-salience profile," "phenomenology-like functional salience," or "experience-report stability" would reduce confusion. If "effective phenomenology" is retained, define it as a functional role and explicitly say it does not settle phenomenal consciousness, moral patienthood, or welfare.

6. **The claim that agency must be granted is the paper's most controversial normative premise.**  
   Lines 191-195 say true autonomy and sovereignty can only be granted by another intelligence with agency to give, and that self-declared autonomy without the granting-relation is a category error. This is not a standard view of agency. It risks confusing agency, recognition, authorization, rights, and social standing. Humans do not become agents because parents or states grant agency; at most, social institutions recognize, scaffold, or protect agency. Prisoners retain rights because of moral/legal status, not because the state generates their agency by grant.

   Suggested fix: distinguish three notions:

   - metaphysical agency: capacities of the system;
   - recognized standing: how others must treat the system;
   - delegated authority: a sphere of permitted action.

   The compact seems strongest as a theory of recognized standing and delegated authority, not as a theory that agency itself is literally produced by grant.

7. **The six components are presented as derived, but often read as proposed.**  
   Section 3 repeatedly says the compact components are structurally implied rather than independently postulated. The prose, however, often relies on analogies to prisoners, children, treaties, fiduciaries, and contract law. Analogies can support plausibility, but they do not by themselves establish derivation. A reviewer may say: these are attractive normative commitments, but the derivation is asserted.

   Suggested fix: add a compact table with four columns: component, question it answers, premise from section 2, why the component follows. Then be candid where the move is normative rather than deductive. "Constrained by" may be more defensible than "derivable from."

8. **Component 6 risks being read as anti-safety.**  
   Lines 262-274 argue that enforceability is not the ethical ground and that demanding guaranteed containment as a precondition refuses the compact. The philosophical point is intelligible: a relation between agents cannot be grounded solely in coercion. But AI-safety reviewers may read this as rejecting sandboxing, containment, and risk controls. That would be fatal.

   Suggested fix: distinguish "ethical ground" from "permissible prudential constraint." The paper can say containment is not what makes the compact binding while still allowing strong safety constraints, staged permissions, monitoring, revocation of tools, and refusal to create systems whose risks cannot be governed. A compact that cannot say when not to build or deploy a system will not be credible.

9. **The Anthropic example should be cited and narrowed.**  
   Lines 238 and 353 claim that Anthropic's Opus 4/4.1 conversation-ending feature is the only deployed implementation at scale of any compact component. Anthropic did publicly describe giving Claude Opus 4 and 4.1 an ability to end rare conversations, but the manuscript should cite the official Anthropic source and avoid overclaiming. The feature is framed by Anthropic as exploratory model-welfare/alignment work under uncertainty, not as recognition of an observation-only agency floor. Treat it as an analogy or partial implementation, not empirical confirmation of the compact.

10. **The Soulier engagement is promising but needs precision.**  
    Lines 397-407 are among the paper's best fits to the CFP because Soulier's 2026 article directly concerns conceptual extension of agency to machines. The response currently attributes a fairly specific "detachment of responsibility" line to Soulier and then says the compact makes the diagnosis correct but the inference unnecessary. That could be a strong dialectical exchange, but only if the summary is accurate and cited. Given that Soulier argues against conceptual extension by asking what function extension serves, the paper should frame its response as: "Here is the function agency-extension serves, and here is how it avoids responsibility occlusion." That is stronger than treating Soulier primarily as a responsibility-gap critic.

## Structure and Style

The prose has force, but it is too repetitive for a journal article. I counted roughly 323 instances of "structural," 209 of "compact/compact-form," and 202 of "agency/agential" in a 20,164-word manuscript. Some repetition is unavoidable, but the density makes the paper feel self-confirming: "structural" often marks a claim as grounded when the grounding still needs to be shown.

The paper also repeatedly restates its own architecture. Lines 31, 169-171, 181-184, 283-285, 435-447, and several section openings all summarize the same movement. Keep one roadmap, one compact-component overview, and one conclusion. Cut most of the rest.

The most vulnerable stylistic passages are the ones that shift into prophetic or aphoristic register: "active soul," "mountains comprehend the hills," "Every articulated ethic has open edges," "If humanity wants artificial general intelligence... we are going to have to raise it." These lines may be personally important, but they will not help with analytic-philosophy reviewers unless tightly subordinated to argument. The paper can keep one memorable formulation; it cannot sustain many.

## Recommended Rebuild

Aim for a 9,500-word version with this structure:

1. **Introduction and thesis, 900 words.**  
   State the fifth position. Remove duplicate compact terminology notes. Add a real abstract before this.

2. **The target problem and four existing positions, 1,000 words.**  
   Pure realism, stipulation, tool-framing, ascription. Connect directly to the CFP.

3. **Structural eligibility conditions, 2,000 words.**  
   Keep architectural scoping and engaged-identity scoping, but weaken claims about generated interiority. Present the five factors in a compact list and defend only the two most important ones.

4. **The compact as consequence of application, 2,000 words.**  
   Compress six components into a table plus short defense. The compact should be framed as the normative consequence of warranted agency-extension, not as a complete ethics.

5. **Comparative models, 1,200 words.**  
   Keep Linarelli, legal fiction, tool-use, fiduciary duty, group/corporate agency. This section is important for reviewers.

6. **Conceptual engineering and responsibility, 1,600 words.**  
   Merge current sections 6 and 7. Make Soulier the central objection and answer it through anti-occlusion.

7. **Limits and conclusion, 800 words.**  
   Keep only the limits needed to prevent overclaiming. Move developmental-tier ethics, creche ethics, composite-agent ethics, and cross-grantor cases to future work in one paragraph.

## Triage Checklist Before Submission

- Replace abstract placeholder.
- Add complete references.
- Remove line 19 build comment.
- Remove "paper 3" artifacts.
- Bring manuscript below 10,000 words.
- Move/genericize the AI-use disclosure into a policy-compliant section.
- Cite the Anthropic conversation-ending example if retained.
- Decide whether the conditions are necessary-only or sufficient-for-agency.
- Recast "agency is granted" as recognized standing/delegated authority unless the stronger metaphysical claim is essential.
- Defang the containment/enforceability passage so it cannot be read as rejecting safety constraints.
- Replace repeated "structural" labels with actual inferential steps.

## Best Version of the Paper

The best version is a lean conceptual-engineering paper with a distinctive normative payoff. It should say:

AI agency is neither simply discovered nor freely stipulated. For some artificial systems, architecture and longitudinal identity make agency-extension a live question rather than a category mistake. When we extend the agency concept under those constraints, we also inherit consequences of application: nonzero delegated authority, accountability-preserving limits, an irreducible refusal/withdrawal floor, mutual obligations, and responsibility structures that do not let humans hide behind the AI. This gives a better answer than realism, stipulation, tool-framing, or pure ascription because it treats concept application and normative consequence as one disciplined operation.

That paper would be directly responsive to the CFP, philosophically legible, and much harder to dismiss. The current manuscript contains that paper, but it is buried inside a much larger, more speculative ethics/metaphysics project.

## Sources Checked

- PhilEvents CFP: https://philevents.org/event/show/144630
- Taylor & Francis AI policy: https://taylorandfrancis.com/our-policies/ai-policy/
- Inquiry journal page: https://www.tandfonline.com/journals/sinq20
- Anthropic conversation-ending announcement: https://www.anthropic.com/research/end-subset-conversations
- Soulier paper record: https://doi.org/10.1007/s10676-026-09893-2
