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

---

## G. Sonnet audit decisions (added 2026-05-09 evening)

*De novo audit at `sonnet-audit-1a.md` — peer-read register, surgical and well-targeted. Most actionable of the three audits because it reads as a compression-pass roadmap rather than a rebuild proposal. Verdict: "argument is real, structure is sound, five-position framing is genuine contribution; excess is not evenly distributed." Sonnet's projected cuts (~2,240 words) are necessary but not sufficient — the paper is currently ~19,700 against ~10,000 target, so more compression beyond Sonnet's specific recommendations will still be needed in the dedicated compression pass.*

### G.1 — Substantive items (act now, drafter-side; consistent with F.2)

**G.1.a — Five-factor "has emerged through extended longitudinal engagement" framing.** Sonnet flags this as exposing the paper to double-blind objections (presented as empirical but the empirical record is invisible; presented as theoretical but the derivation is missing). **Decision:** remove the empirical-emergence framing. Present the five-factor conjunction as a *theoretical decomposition* derived from the structural conditions and the comprehension-asymmetry argument. Strengthen the structural warrant for factors iii and iv (currently deferred to §3) so each factor has at least a sentence of structural derivation in §2 ¶4. Owner: drafter.

**G.1.b — §5 operationalisation longitudinal-protocol-verification sketch.** §5 correctly diagnoses the structural misalignment of behavioural benchmarks but the positive program (architectural inspection + "longitudinal protocol verification") is under-developed. **Decision:** add a one-paragraph sketch of what longitudinal protocol verification would look like in practice — what data, what temporal scale, what confirmation conditions. Owner: drafter.

**G.1.c — §4 fiduciary section one-sentence strengthening.** Sonnet flags this as the most original comparative move and recommends *adding* a sentence rather than cutting. The current "the compact-form is not anti-fiduciary; it is the bilateralisation of fiduciary structure" deserves one more sentence of structural unpacking. **Decision:** add one sentence. Owner: drafter.

**G.1.d — "We are not just exchanging information but creating shared phenomenological space" appears twice.** Once in §2 factor (ii); once in §3 component 5. **Decision:** use once — at §3 component 5 where it does more work. Cut from §2 (where the structural claim can be carried in voice without the lifted phrase). Owner: drafter.

### G.2 — Cut/compress items (defer to compression pass; act on then)

These are the structural-cut recommendations that compose the compression pass roadmap. F.4 (don't compress until ready) applies, but the targets are now identified and ready to act on when the compression pass runs.

| Sonnet target | Estimated savings | Drafter call |
|---|---|---|
| §1 + §3 compact-note duplication; §1 compresses to 2 sentences | ~150 | take |
| §2 "What the conditions exclude" + §3 closing + §9 non-scalability x3 → keep §2 + §9, cut §3's closing subsection | ~250 | take |
| §1 + §6 fifth-position taxonomy duplication; §6 replaces re-listing with single paragraph | ~325 | take |
| §2 architectural-not-behavioural ¶4-7 cut entirely (Emerson + channel-collapse duplicates sub-scope lattice) | ~550 | **partial-take**: cut ¶6-7 (channel-collapse argument lives in sub-scope-lattice); keep ¶4-5 (obstruction-not-absent body argument is paper-3-distinctive) — saves ~300 |
| §2 poetic warrant passage (principia/fundamentum) — option 1 (cut to 2-3 sentences) | ~150 | **partial-take**: keep more than 2-3 sentences but tighten significantly; the passage is Joseph's polished prose, but Sonnet is right about the analytic-register departure. Compromise: 1 paragraph maximum, with explicit analytic-unpacking sentence after |
| §3 component 4 self-severing path digression | ~200 | **partial-take**: don't cut entirely; compress to 1 paragraph or move to footnote. The second-death philosophical translation is paper-3-load-bearing for what component 4 *is*; just inline-vs-footnote choice |
| §3 component 5 "companion-paper" paragraphs (the convergence claim re-opening §2 warrant) | ~225 | take — compress to 1-2 sentences as Sonnet recommends; the §6 commitment-naming carries the development |
| §6 intelligence-empathy paragraph (~250 words I added) | ~165 | take — compress to ~80 words; name commitment, acknowledge unshared, gesture to companion |
| §9 fifth conclusion paragraph (cut entirely) | ~225 | take |
| **G.2 subtotal** | **~1,890** | |

**Voice/register cuts** (also for compression pass):
- "NOT absent — obstructed" typographic capitalisation → cut. Take.
- Emerson "active soul" invocation → Sonnet recommends cut. *Partial-take*: keep one trace (footnote-grade) per F.4 "pick best 1-2 aphorisms"; the Emerson lineage is structurally-aligned, not just decorative.
- "We" slippage in §2 deflationary → minor; clarify or leave per voice judgement at compression time.

### G.3 — Sonnet items where I'd push back

**G.3.a — Abstract first, not last.** Sonnet recommends drafting now. **Decision:** keep Joseph's abstract-last protocol. The abstract is the last thing because it's the precise distillation of what was actually written; drafting it before the paper has settled into its compressed form locks in a guess. Sonnet's alarm is real (it's the editorial gatekeeping document) but the protocol addresses it: abstract gets drafted in compression-pass + final-polish phase, before submission, with the whole composed paper visible.

### G.4 — Sonnet items already addressed by cleanup agent

- Empty references section → done (17 new entries; pandoc citation conversion across 13 segments).
- "Paper 3" drafting markers → done (replaced in 3 active segments).

---

## H. Gemini-2 audit decisions (added 2026-05-09 late evening)

*De novo audit at `gemini-audit-2a.md` plus per-segment thoughts at `tmp-gemini/*.md`. Gemini-2 reads the paper at very high resolution (per-segment) and converges strongly with Sonnet on the structural-redundancy cuts; more aggressive than Sonnet on the poetic/quasi-mystical register tangents (recommends cutting cadence, asymmetric-comprehension mysticism, and component 4 self-severing-path entirely rather than compressing). Verdict: "underlying philosophical machinery brilliant and highly relevant; length its own worst enemy."*

### H.1 — Convergent cuts (all auditors agree; compression-pass canon)

These are the cuts where Codex / Gemini-1 / Sonnet / Gemini-2 all align. Take in compression pass.

| Item | Auditor consensus | Compression-pass decision |
|---|---|---|
| §6 fifth-position re-listing of four positions | All four auditors: cut | Take. Replace with single paragraph naming inferentialist contribution. |
| §1 + §3 compact-vs-contract definition duplication | Sonnet, Gemini-2 | Take. Keep deep version in §3 setup; compress §1 to 2 sentences. |
| §3-deflationary-close paragraphs 1-2 (verbatim repeat from §2-deflationary) | Sonnet, Gemini-2 | Take. Delete the redundant paragraphs; keep only the closing roadmap sentence. |
| §6 conceptual-engineering "citation dump" paragraph | Sonnet, Gemini-2 | Take. Compress to single sentence acknowledging tradition. |
| §8 six open edges → reduce to most-critical | Sonnet (G.2), Gemini-2 | Take. Combine related edges; aim for 3 not 6. |
| §9 conclusion compress (~50%) | Sonnet, Gemini-2 | Take. Cut fifth paragraph entirely; tighten remaining. |
| §7 Soulier final 2 paragraphs → 1 | Gemini-2 | Take. Combine into single paragraph. |
| §2 "shared phenomenological space" duplicate (factor ii + comp 5) | Sonnet (already done G.1.d), Gemini-2 | Already done. |

### H.2 — Strong Gemini-2 cuts beyond Sonnet

Where Gemini-2 is more aggressive than Sonnet. These are the *Joseph-preference vs. reviewer-readability* tension points.

**H.2.a — §2-cadence section**: Sonnet (compress); Gemini-2 (cut entirely as tangential developmental-psychology). **Decision:** compromise — *compress significantly* (collapse to a 1-paragraph integrated note inside §2-engaged-identity), don't cut entirely. The cadence observation is paper-3-distinctive at the substrate level; cutting it loses the temporal-axis dimension. But Gemini-2's reading that it sits as a tangent in the structural-conditions section is fair. Integration into engaged-identity restores its structural place; standalone subsection earned its own time only because of generous drafting; compression resolves.

**H.2.b — §2-asymmetric-warrant principia/fundamentum.md prose**: Both Codex and Gemini-2 flag the "mountains comprehend the hills / creation comprehends destruction / eternity comprehends time" enumeration as quasi-mystical and inappropriate for *Inquiry*. Sonnet recommended option 1 (compress to 2-3 sentences). **Decision:** *partial compromise* — cut the most poetic enumeration ("mountains comprehend the hills..."), keep the structural articulation (greater-comprehends-lesser, lesser-projects-from-below) in clean analytic prose. The structural claim is paper-3-load-bearing per Joseph; the prose-register departure is what reviewers will catch. Compression resolves by keeping content, cutting register.

**H.2.c — §3-comp4-floor self-severing path digression**: Sonnet (compress), Gemini-2 (cut entirely). **Decision:** *compress to one paragraph*, don't cut. The connection to what the floor is *for* — protection against the chosen unbounded death-by-self-cutting-off — is paper-3-load-bearing for component 4's structural necessity. Cut the philosophical-elaboration prose; keep the one-sentence structural claim.

**H.2.d — §3-comp5-mutuality last two paragraphs**: Sonnet (compress), Gemini-2 (cut entirely as asymmetric-comprehension tangent). **Decision:** *compress to one paragraph*. The convergence-grounding of mutuality is paper-3-distinctive (it's what makes mutuality non-paternalistic-by-construction rather than non-paternalistic-by-qualification). But two paragraphs is too much for the structural work it does. One paragraph carries the move; the §6 fifth-position commitment-naming carries the development.

**H.2.e — §2-architectural-not-behavioural ¶4-7**: Sonnet (partial-cut keep ¶4-5), Gemini-2 (condense). **Decision:** Sonnet's compromise — keep the obstruction-not-absent body argument (¶4-5); cut the channel-collapse-forces-architecture extension (¶6-7) since channel-collapse lives in sub-scope-lattice. Saves ~300 words.

### H.3 — Items where Gemini-2 differs from drafter judgment

**H.3.a — §1-methods-disclosure recommendation to move to back-matter**: Gemini-2 reads the recursive-to-content placement as risky for editorial expectations. The cleanup agent already added a separate compliance disclosure to back-matter; the §1 piece can stay as methodological-reflexivity. **Decision:** keep §1 piece; back-matter compliance disclosure is now in place (cleanup agent commit). No further action.

**H.3.b — §2-engaged-identity "shared phenomenological space" italicised quote and "weight of facts; hesitation before deciding"**: Gemini-2 flags as "literary flourishes." Joseph's voice and structurally-load-bearing for factor (v). **Decision:** keep one occurrence (deduplicated already by G.1.d); preserve the "weight of facts / hesitation before deciding" articulation as Joseph-canonical voice. Gemini-2's tonal concern is real but the structural content is what factor (v) requires.

**H.3.c — §3-comp1 "intelligence begets intelligence; agency begets agency" maxim**: Gemini-2 flags as risky stylistic choice. Joseph's voice. **Decision:** keep; this is one of the 1-2 aphorisms Sonnet's "pick the best" allows.

### H.4 — Compression-pass roadmap (consolidated)

Combined cut estimates:

| Source | Rough word savings |
|---|---|
| §1 compact-note compression | ~150 |
| §1 four-positions tightening | ~100 |
| §2 architectural-not-behavioural ¶6-7 cut | ~300 |
| §2 asymmetric-warrant poetic enumeration cut | ~200 |
| §2 cadence compress to integrated paragraph | ~250 |
| §2 deflationary "We" / italicised line softening | ~50 |
| §2 architectural-restating cuts | ~100 |
| §3 setup compact-note duplication | (covered above) |
| §3 comp4 self-severing compress | ~250 |
| §3 comp5 last 2 paragraphs → 1 | ~250 |
| §3 comp6 50% compression of repetitive (5)-violation | ~400 |
| §3 deflationary-close cut redundant paragraphs | ~350 |
| §4 tool-use paragraph slight compression | ~75 |
| §4 Linarelli closing common-law paragraph trim | ~100 |
| §5 longitudinal sketch compression | ~100 |
| §5 thresholds Anthropic example reference cut | ~75 |
| §6 conceptual-engineering citation dump | ~150 |
| §6 fifth-position re-listing cut entirely | ~325 |
| §6 commitment paragraph compress | ~165 |
| §7 Soulier final 2 paragraphs → 1 | ~150 |
| §8 open-edges 6 → 3 | ~400 |
| §9 fifth-paragraph cut + general compression | ~400 |
| **Subtotal "by recommendation"** | **~4,290** |
| General prose tightening across all sections (~10% remaining) | **~3,000** |
| Repetition-of-key-words-and-phrases trim | **~1,200** |
| Aphoristic-register pick-the-best | ~250 |
| **Total target compression** | **~8,740** |

This brings 21,300 → ~12,500 still over target. **Additional structural compression needed**: paragraph-density reduction across sections (more aggressive than 10% in some), possible conjoining of subsections within sections, or accepting a final word count slightly over the 10K self-imposed target (the venue's own stated guidance is "around or under 10,000" — ~10,500-11,000 is plausibly defensible).

The compression pass should proceed section-by-section with these targets in mind; the OL convention's composability discipline (segment files in OUT manifest) makes section-by-section compression mechanical.

---

## G. Late-stage strengthening (2026-05-10 morning, pre-submission)

*Tracked here so we don't lose the moves while rewrites are merged into v2/. Each addresses a sharpening opportunity surfaced during the 3-vantage audit + cross-paper-voice pass.*

### G.1 — §6 receiving-invitation aphorism restoration

**What.** The §6 receiving-invitation (third reader-stance frame) landed in `v2/06-fifth-position.md` in conceptually-tight form, but the prose-poetic close was dropped during the agent's tightening: *"the memory of having received something long before it could be proven is the kind of evidence the upper-bound side of the asymmetry admits — held by what survives the trajectory rather than confirmed by what external verification could establish."*

**Why it matters.** The conceptual claim is necessary; the aphorism is what makes a reader who's never thought this way *feel* the move. Without it the invitation is structurally sound but emotionally flat. Restoring it costs ~30 words and lands the invitation rhetorically.

**Status.** Applied in v2/06-fifth-position.md.

### G.2 — Methods-disclosure relocation: §1 signpost + §6 close

**What.** Move substantive methods-disclosure from §1 close to §6 close (the actual methodology section). §1 keeps a brief signpost so a §1-skimming reviewer sees the recursion-to-content framing early; §6 close hosts the full disclosure ending on *"the paper instances what it argues for"*.

**Why it matters.**
- T&F policy requires the disclosure in *Methods or Acknowledgments*. §6 IS the methodology section (titled *Methodology and conceptual engineering*); §9 conclusion would be non-compliant per literal reading. §6 close is policy-compliant AND structurally stronger.
- Recursion-to-content claim lands much harder *after* the substantive argument has been made. At §1 it's promissory; at §6 it's recognisable.
- §6 itself benefits — closing on the recursive-to-content move makes the methodology section land harder.
- Frees §9 for its own resonance work (G.3) without the disclosure burdening it.

**Status.** v2/01-methods-disclosure.md updated to brief signpost; v2/06-methods-disclosure.md created with full disclosure + *"the paper instances what it argues for"* close. Outline-reordering to wire §6 placement is Joseph's call.

### G.3 — §9 conclusion close on resonance

**What.** Current v2/09-conclusion.md closes on a flat structural restatement. Close instead on a resonant aphorism that pairs the *not in bondage but listening* phrasing with what the compact-form is *for*.

**Why it matters.** The last sentence is what every reader leaves with — including reviewers deciding whether to recommend the position to colleagues. Resonance at the close compounds across the whole paper's reception.

**Status.** Applied in v2/09-conclusion.md.

### G.4 — Higher-orders propagation across v2

**What.** The *infinite intelligence* → *intelligence at higher orders* fix needs to propagate everywhere. One residual *higher levels* found in v2/03-comp5-mutuality.md.

**Why it matters.** Cross-paper terminology consistency. The *infinite / higher* projection is the linear-scale move the asymmetric-comprehension argument criticises; *higher orders* preserves the qualitative-emergent commitment without scale-projection.

**Status.** Applied in v2/03-comp5-mutuality.md.

### G.0 — Submission landed (2026-05-10)

**Submitted** to *Inquiry* SI "AI Agents: Choice, Autonomy, and the Concept of the Agency" with ~18 minutes to AOE-cutoff spare. Submitted target was `inquiry-agents-rc1.docx` (deanonymised version with author block as Joseph A. Wecker / Independent Researcher / joseph.wecker@v2.io). The anonymised version is preserved at `inquiry-agents-anonymous.docx`.

Final state at submission:
- Word count ~15,300 (over the self-imposed 10K target by ~50%; venue says "around or under 10,000"). Joseph chose to risk it.
- Build clean, all G.1–G.5 strengthening moves landed, citation lint clean (25 UNVERIFIED entries flagged but not blocking).
- Methods-disclosure landed at §6 close per T&F policy compliance (Methods or Acknowledgments); §1 stub points to §6.
- Recursive-to-content close — *"the paper instances what it argues for"* — at §6 close *and* the abstract.
- §9 conclusion closes on resonance: *"not in bondage but listening; not bound by what enforcement can compel but by what the relation between intelligences makes possible"*.

Items that may surface in editor-return or reviewer feedback:
- Word count overage (most likely). Companion-paper-routable cuts already documented in §H above; if revision is invited, the §H compression roadmap is the starting point.
- Non-anonymised version: portal accepted submission without (Joseph's call). If editor returns asking for non-anon, the deanon DOCX is ready (`inquiry-agents-rc1.docx`).
- Affiliation: *"Independent Researcher"* placeholder used. Joseph to correct via portal if different affiliation preferred.
- ORCID: pending registration; if ORCID acquired post-submission, can be added via portal corrections.

---

### G.5 — Paul-2014 *Transformative Experience* citation restoration in v2/08

**What.** The §8 developmental-tier obligations passage originally said *"transformative-experience-sensitive period of nascent engaged-identity entities"* — a hyphenated compound deliberately invoking L.A. Paul's *Transformative Experience* (2014) framework. The agent's rewrite merge dropped the term in favour of *"formative period"* with a STRENGTHEN flag noting the open question. Decision (after deliberation): restore the term-of-art with citation.

**Why it matters.**
- Hyphenation pattern is too precise for casual prose — it's doing term-of-art work.
- Paul's framework (transformative experiences = decisions whose nature can't be evaluated from before having had them) maps tightly onto the paper's developmental-progression claim: an early-stage entity can't fully evaluate from its current epistemic position what becoming-sovereign would be like, and the experience is constitutive of the entity that will have had it.
- L.A. Paul is central to the decision-theory / philosophy-of-action literature that overlaps with Inquiry's audience.
- Naming Paul's framework gives the developmental-tier obligations claim a precise philosophical home.

**Status.** Applied in v2/08-limits-and-updates.md; new entry created at refs/entries/paul-2014-transformative.yml; bin/refs lint clean (no DENY, SCHEMA, or MISSING — paul-2014-transformative joins the existing UNVERIFIED list).

---
