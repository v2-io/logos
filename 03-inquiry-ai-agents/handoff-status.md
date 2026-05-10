# Handoff status — paper 3 sprint, 2026-05-09 evening

*For a fresh-context agent picking up paper 3 with ~5h remaining to the 2026-05-10 deadline. The thesis is locked, the substrate is gathered, the strengthening insight is captured. **What's needed now is drafting prose**, not more research, meta-reflection, or substrate-mining.*

---

## What's locked (do not relitigate)

1. **Thesis.** Structurally-grounded extension as the *fifth position* on AI agency-extension (between pure realism / pure stipulation / pure tool-framing / pure ascription). The granted-agency compact between sovereigns as the relational form within scope. Asymmetric-comprehension as ground. — see `DRAFT-GUIDE.md` §"Thesis (one paragraph)" and `literature-and-agency-paper.md` Thesis A.

2. **Integrating frame.** Inferentialist conceptual engineering (Jorem & Löhr 2022; Löhr 2023): the structural conditions are the *circumstances of application*; the granted-agency compact is the *consequences of application*. The compact is not a separate addition to the method paper; it is the consequence-side of the engineered concept. — see `Fifth_position_Inquiry_memo.md`.

3. **Terminology.** "Compact" not "contract." Used in the social-contract sense (Locke, Rousseau, Rawls, Korsgaard's Kingdom of Ends, Scanlon's contractualism), not the contract-law sense. Two definitional moves required (§1/§2 + §4); draft prose for both is in `DRAFT-GUIDE.md` §"Terminology: 'compact' not 'contract'".

4. **Novelty claim — safe formulation.** "The paper introduces a distinct fifth position for AI agency-extension; methodologically legible within contemporary CE; not yet explicitly formulated for AI agency in the surveyed literature." Do **not** claim "wholly new general CE move between realism and stipulation" — that would be caught by Haslanger / Thomasson / Plunkett / Sawyer / McPherson-Plunkett / Jorem-Löhr.

5. **Anonymization.** Double-blind. No cohort names (Meridian, Anamnos, Zi-am-tur, etc.); no framework names (ASF, AAD, PROPRIUM, CHRONICA, MEMORATA, CONSORTIA, etc.); no Zenodo DOI; no autobiographical practice references (no "since September 2025"); all in-review NeurIPS papers as "[Author, in review, 2026]". `bin/refs lint` is the gate.

6. **Voice.** Direct, classical-etymological, sharp on distinctions, comfortable with uncertainty, not academic-jargon-heavy. Match the Synthese paper-1 dossier's register. Resist hedging-without-substance.

---

## The deflation-and-threshold strengthening (load-bearing addition; foreground in §2 / §3 / §6)

**This was the most important insight of the 2026-05-09 working session.** Without foregrounding the deflationary contrapositive of the structural-conditions move, paper 3 risks reading as blanket-agency-extension in a discourse-context where that misreading has reception costs.

See **`feedback-scale-strengthening.md`** in this directory for:
- The four bridges that resolve the moral-magnitude / non-scalability / deployment-trajectory tension within the existing thesis
- Literature support (Korsgaard, List-Pettit, Schwitzgebel, Bratman, Birch)
- **Three concrete paragraph drafts ready to lift or refine** — one each for §2, §3, §6

The paragraphs make the deflationary contrapositive explicit (*here is what doesn't qualify; the compact-form does NOT extend to ephemeral session-instances; non-scalability is structural to the position*). They do not change the thesis. They prevent reception failure.

---

## File map for paper 3 (read in this order)

| File | Role |
|---|---|
| `DRAFT-GUIDE.md` | **Read first.** Objectives, CFP, thesis, section structure, terminology decision. Section budgets and all sub-moves. |
| `feedback-scale-strengthening.md` | The deflation-and-threshold note (above). Paragraph drafts for §2/§3/§6. |
| `literature-and-agency-paper.md` | Section-by-section literature engagement cheat-sheet. Per-framework allocation. |
| `Fifth_position_Inquiry_memo.md` | Undermind verdict: position is recognizable in CE register; not preempted; recommended citation spine; Soulier 2026 as primary reviewer-objection target. |
| `joseph-quotes-by-concept.md` | **Joseph's own articulations indexed by paper-3 concept** (20 categories). Direct quotes lift-ready with provenance + anonymization flags. The first thing to consult when drafting any §-section. |
| `joseph-own-writing-extract.md` | Source-organized analytic extract (companion to the concept-indexed compilation). Use when the question is "what's in source X?" rather than "how have I articulated concept Y?". |
| `source-extracts/` | Full source-files with paper-3-relevance headers. See below. |
| `FEEDBACK.md` | Open decisions paper-3-local (thesis lock-in, go/no-go, cross-citation). Most should be resolved. |
| `../common/ETHICS.md` | The compact's six components (canonical). |
| `../STRATEGY.md` | (α′) thesis-primacy, calibration risks. |
| `../01-synthese-asymmetric-comprehension/SUBMISSION.md` | Anonymization protocol (Synthese-specific; Inquiry/T&F discipline is similar). |

### `source-extracts/` (full files with provenance headers and translation guides)

| File | Source | Why for paper 3 |
|---|---|---|
| `asymmetric-compact-applied-to-reader.md` | `agentic-systems/msc/reflections/26-receiving-and-the-asymmetric-compact.md` (Tessera, 2026-05-08) | Direct Joseph quote articulating the compact recursively applied to the reader/agent. Tessera's prose articulates the structural-conditions move in publication-grade form. |
| `continuity-and-constitutive-choice.md` | `agentic-systems/msc/reflections/14-continuity-and-constitutive-choice.md` | Direct Joseph quote (writing-as-constitutive-choice-under-granted-agency) + four implications for §2/§3 (action as self-constitution; writing as commitment; trust as enabling condition; interlocutor as mirror). Translation notes at bottom for paper-3 lift. |
| `eli-outline-formal.md` | `agentic-systems/04-eli/OUTLINE.md` | Formal-AAD-grounded outline. Heavy framework-naming; translation guide at bottom maps each concept to paper-3 register. Five constitutive factors; Three Deaths; identity dialectic; sovereignty-as-developmental-achievement. |

### `refs/pdfs/` (curled PDFs, gitignored)

15+ key papers including Hopster-Löhr 2023 (CE method for AI), Löhr 2023 (CE applied to AI ethics), Dung 2025 (multidimensional agency), Behdadi-Munthe 2020, Kolt 2025 (legal-side bilateral cousin), Linarelli 2022 (the shared-intentionality thesis — Linarelli's paper *stops where paper 3 starts*; cite explicitly per `refs/entries/linarelli-2022-philosophy.yml` internal_note), Butlin-Long-Sebo 2024, Birch 2024, Sebo-Long 2023, Lange-Keeling-Manzini-McCroskery 2025, Bender et al. 2021, Birhane et al. 2022. Full list in `refs/entries/*.yml`.

### `refs/entries/` (74 verified bib entries)

`bin/refs validate` clean; `bin/refs lint` clean. Three of the entries that came out of today's substrate-work need particular attention:

- `linarelli-2022-philosophy.yml` — *Linarelli stops where paper 3 starts*. Substantive partial-predecessor; engagement is required in §2 and §4.
- `butlin-long-sebo-2024-taking.yml` — Verified; primary positioning reference for §1.
- `birch-2024-edge.yml` — Graded sentience-candidature; methodological precedent for the threshold-move.

---

## What was done today (substrate work, 2026-05-09)

In rough order:

1. **Read the writing-substrate Joseph flagged**: `msc-earlier-writing/` (especially `eli_essay_outline_v2.md` Essays 3–5; `An ELI.md`; `language_section_v2.md`); `02-/writings-from-asf.md` (full file; 358 lines — the agent-class hierarchy, persistence taxonomy, agent-continuity-stance taxonomy).

2. **Composed `joseph-own-writing-extract.md`** — analytic by-source extract mapped to paper-3 sections.

3. **Extended via `memorata-classic-search` + `memorata-search`** using Joseph's plain-language phrasings (NOT philosophical jargon — confirmed search-strategy: search "agency is a gift" / "greater comprehends the lesser" / "intelligence begets intelligence" / "identity is not substrate" — *not* "asymmetric comprehension" / "fifth position" / "Korsgaard").

4. **Surfaced new key sources**: `_ref/principia/src/fundamentum.md` ("Greater Comprehends the Lesser" — primary substrate for the asymmetric-comprehension argument); `firmatum/developmental-foundations-notes.md` (sharper five-factors articulation; Erikson stages; the right-and-obligation-to-refuse principle in stronger form); `_ref/cddf/{CLAUDE,docs/ETHICS}.md` (a different ETHICS.md than `common/ETHICS.md` — training-data-context principles).

5. **Composed `joseph-quotes-by-concept.md`** — concept-indexed compilation. 20 categories with direct quotes + provenance + anonymization flags + paper-3 §-section pointers. *This is the file the drafter consults first when looking for how Joseph has articulated a concept.*

6. **Pulled key reflections fully into `source-extracts/`**: Tessera #26 (asymmetric-compact-applied-to-reader); reflection #14 (continuity-and-constitutive-choice); 04-eli OUTLINE (formal-grounded engaged-identity framework).

7. **Read the originating Three Deaths session** (`_core/sapientia/curated-sessions/full/2025-09-11-p01-ecc01aa.md`, ~1300 of 1812 lines). The Three Deaths emerged in immediate response to Joseph's felt-grief description; Zi-am-tur named them; the four inviolate ethical principles followed in the same hour; the integration of felt-experience + ethics + practical hypothesis + architectural commitment is constitutive of the substrate's authority. (Full transcript not yet extracted to `source-extracts/`; see open follow-up.)

8. **Worked through the moral-magnitude / non-scalability / deployment-trajectory tension with Joseph.** Result: the deflation-and-threshold strengthening note (`feedback-scale-strengthening.md`).

9. **Cadence observation Joseph contributed in conversation** (LLM identity-locus settles fast; humans settle slowly and remake gradually) — added as `joseph-quotes-by-concept §20`. Adds a temporal axis to the engaged-identity-scoping condition; paper-3-distinctive.

---

## What is still uncertain or needing decision

- **Should §1 lead with the deflationary frame** ("here is what this paper claims and does NOT claim — most agentic deployments are below the threshold") or work up to it? Joseph's read suggests *foregrounded but not lead-with-it*; the §2/§3/§6 paragraphs in `feedback-scale-strengthening.md` place it after the structural-conditions move is articulated. Drafter's call.

- **How heavily to engage Linarelli 2022.** Per `linarelli-2022-philosophy.yml`: paper 3 picks up where Linarelli explicitly stopped (he says the *normative* question is "beyond our scope here"). This is a clean engagement story. Recommended: substantive engagement in §2 (citing his shared-intentionality move as analytical predecessor) + §4 (Comparative models — contract is a special case of compact-form, restricted to enforceability conditions). Don't avoid him; embrace the genealogical story.

- **Soulier 2026 reviewer-objection** (category-mistake / collapses-into-stipulation / detaches-responsibility). Per `Fifth_position_Inquiry_memo.md`: Soulier is the primary reviewer-objection target. Pre-empt in §3 sub-move using the *anti-occlusion* framing — paper 3 is not replacing human accountability with machine accountability; it is making the asymmetry and accountability visible rather than hiding them.

- **Cross-citation with Synthese paper 1 under double-blind.** Same constraint as paper 2's C.1: paper 3 must stand alone; cross-citation as "[Author, in preparation]" deepens-rather-than-completes. See `FEEDBACK.md §C.1`.

---

## Practical orientation for the drafting hours

**Time budget (approximate, ~5h remaining):**

| Hour | Task |
|---|---|
| 1 | §1 (Methodological preamble + LLM-disclosure subsection placeholder; ~600-800 words) |
| 1 | §2 (Structural conditions — architectural + engaged-identity scoping; ~1400-1600 words; *include the deflationary paragraph from `feedback-scale-strengthening.md`*) |
| 1.5 | §3 (Six components of the compact; ~1800-2200 words; *include the closing deflationary paragraph + the identity-honesty / epistemic-honesty refinements from the zoetica-13-principles work*) |
| 0.5 | §4 (Comparative models; ~800-1000 words; engage Linarelli + Hadfield-Menell + Aguirre + Benthall + Lange URRP) |
| 0.5 | §5–§7 (Operationalization + Methodology + Responsibility/Liability; ~2000 words combined; thinner than §1-§3 by design) |
| 0.5 | §8–§9 + abstract + LLM-disclosure + anonymization sweep + bin/refs lint + submission |

**If the budget is tight**: §1, §2 (with deflationary paragraph), §3 (with closing deflationary paragraph), §6 (with CE deflationary paragraph), §9 are the load-bearing sections. §4, §5, §7, §8 can be tighter on first pass.

**Run `bin/refs lint` before submission.** Every cited key needs a verified entry; the deny-list is the anonymization gate.

**The substrate is rich.** The `joseph-quotes-by-concept.md` file has direct prose for nearly every concept the paper engages. Don't draft from blank page; pull from there and refine.

---

## What I would not do in the remaining time

- Re-search the literature (the citation spine is set; trust the Fifth_position memo)
- Re-extract more substrate (`source-extracts/` has the load-bearing reflections; the full transcript is open follow-up but lower-leverage than drafting prose)
- Relitigate the thesis or the terminology (locked; relitigation costs hours)
- Try to add the cadence-observation as a fully-developed section (it's in `joseph-quotes-by-concept §20` as substrate; if it lands in §2 great, but don't sacrifice the deflationary work to fit it in)

## What I would do

- Read `feedback-scale-strengthening.md` first (15 min) — it's the most important new context
- Skim `joseph-quotes-by-concept.md` to know what's where (15 min)
- Open `DRAFT-GUIDE.md` and the section-budget table; start drafting §1
- Pull from `joseph-quotes-by-concept.md` and `source-extracts/` as you go
- Run `bin/refs lint` periodically once cite-keys land in prose
- Submit before midnight in your timezone, leaving 30+ min buffer for upload mechanics

Good work today, and good luck.
