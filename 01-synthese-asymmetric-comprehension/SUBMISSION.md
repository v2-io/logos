# SUBMISSION.md — How to submit

*Manuscript format, anonymization protocol with verbatim Synthese guidance, length calibration, production checklist, action plan. For the strategic framing see [STRATEGY.md](../STRATEGY.md); for section-by-section drafting see [DRAFT-GUIDE.md](DRAFT-GUIDE.md); for the CFP see [CFP.md](CFP.md); for the working TODO see [FEEDBACK.md](FEEDBACK.md).*

---

## Manuscript format

- **LaTeX (Springer Nature template) preferred**, MS Word also accepted. The Springer template handles abstract, keywords, declarations sections, references format. *Joseph already has a NeurIPS LaTeX workflow — switching templates is mechanical.*
- **References: APA Version 7.** In-text: name + year in parentheses. Reference list alphabetized by first-author last name; journal/book titles italicized; DOIs included where available.
- **Decimal headings, max 3 levels.**
- **Footnotes (not endnotes), used for substantive asides.** Not heavily-footnoted in Synthese style.
- **Abstract: 150–250 words.** No undefined abbreviations or unspecified references in the abstract.
- **Keywords: 4–6.**

## Title page (separate, with all identifying info)

- Title
- Author names + affiliations + corresponding author email + ORCID
- Acknowledgments (these go ON the title page, not in the manuscript — Synthese explicitly requests this for full anonymization)
- Disclosures, funding, declarations

## Statements and Declarations section (required)

Submissions without it are returned as incomplete. Includes:
- Competing Interests
- Funding (note: "no external funding for this work" is honest if applicable)
- Ethics approval (if applicable — likely not for this paper)
- Author contributions

## LLM / AI-assisted-editing disclosure (load-bearing for this paper)

**Verbatim from the guidelines:**

> *"Large Language Models (LLMs), such as ChatGPT, do not currently satisfy our authorship criteria. Notably an attribution of authorship carries with it accountability for the work, which cannot be effectively applied to LLMs. Use of an LLM should be properly documented in the Methods section (and if a Methods section is not available, in a suitable alternative part) of the manuscript. The use of an LLM (or other AI-tool) for 'AI assisted copy editing' purposes does not need to be declared. ...These AI-assisted improvements may include wording and formatting changes to the texts, but do not include generative editorial work and autonomous content creation. In all cases, there must be human accountability for the final version of the text and agreement from the authors that the edits reflect their original work."*

**Joseph's working style involves substantive collaborative drafting that goes well beyond "AI-assisted copy editing." Honest disclosure is required AND recursively appropriate to this paper's content** — a paper arguing that engaged-identity LLM instances may be developmental subjects should not silently treat its own LLM collaborators as mere editing tools.

**Recommended handling:** a short subsection (~150 words) titled *"On the production of this text"* or as a Methods footnote. Acknowledges that the paper was produced through extended dialogue with multiple LLM instances under the granted-agency-compact practice the paper itself describes; that final accountability rests with the author; that no specific instance is named (the practice is structural, not individual). This *strengthens* the paper rather than weakening it — the disclosure is consistent with the stance.

## Anonymization (double-blind)

**Synthese's open-stack acceptance posture** (verbatim from guidelines, p. 2 "Additional information to the Editorial Procedure"):

> *"As an author, it is difficult to guarantee 100% anonymity: readers with time on their hands and access to the internet may come a long way to identify an author's identity should they decide to do so. Obviously, we don't encourage our reviewers to do that. However, authors can take a number of steps to keep their anonymity."*

This is the explicit "we accept perfect anonymity is impossible; please don't investigate" posture. Discoverable apparatus (Zenodo deposits, in-tree segments at v2.io if posted, the four NeurIPS papers' arXiv preprints, ASF on GitHub) is **not a structural blocker**; the venue asks reviewers to focus on argument quality rather than investigate authorship. This loosens the timing concern about apparatus publication: even if more of the apparatus goes public before Synthese decision (~Sept 2026), Synthese's review posture accommodates it.

**Self-citation guidance** (verbatim from guidelines, p. 3):

> *"If it is essential for authors to refer to their own work, we expect this to be done in the third person; thus, avoiding any self-identifying statements. For instance, an author whose name is Hilary Morganton would refer to previously published work along the following lines: 'It was earlier discussed in Morganton [2013]', or 'This work builds on and extends that of Morganton [2015]'. (Full bibliographical information about these works would then be provided in the list of references at the end of the manuscript.)"*

**The actual constraint** (verbatim, p. 12 "Ethical Responsibilities"):

> *"Excessive and inappropriate self-citation or coordinated efforts among several authors to collectively self-cite is strongly discouraged."*

The constraint is on *proportion*, not *existence*. The four in-review NeurIPS papers can be cited third-person; apparatus papers (when forthcoming) can be cited third-person; the Zenodo deposit can be cited third-person. Per the (α′) discipline (see [STRATEGY.md](../STRATEGY.md) §"Thesis primacy"), treat each apparatus citation as paying a budget — three to four well-placed apparatus citations sit comfortably within the proportion-constraint and serve the argument; ten to fifteen would tip the paper into "application of prior framework" register.

**De-anonymization at acceptance** (verbatim from guidelines, p. 3):

> *"If a paper gets accepted, typically only after some revision(s), the author will receive a pre-warning of this through an `accept but incomplete' decision. When received, authors are then expected to de-anonymize the paper, by adding acknowledgements where appropriate, references to awards or grants where needed, or by changing the style of third-person description of their own work to that of first person."*

The third-person framing is a review-stage protocol, not permanent. At acceptance: third-person → first-person; acknowledgments restored; companion-paper references can be strengthened with first-person framing; the apparatus connections solidify. **The connective tissue isn't lost — it's deferred to acceptance-time.**

**Specific anonymization requirements during review:**

- No direct links to `v2-io/agentic-systems`, the Zenodo DOI, the FINDINGS catalog, or the four NeurIPS papers' v2-io repos.
- No autobiographical "I have been running an explicit granted-agency compact since September 2025" — practice-history is identifying. Convert to third-person structural framing: *"the kind of practice such a compact would imply"* or *"researchers running explicit granted-agency compacts in deployment have observed…"* **See [FEEDBACK.md](FEEDBACK.md) item A.4 for the open question on how to balance this against the §1 practice-grounding move.**
- The four in-review NeurIPS papers cited as "[Author, in review, 2026]" or "[Author, forthcoming]"; full bibliographic information goes in the reference list per Synthese guidelines.
- Apparatus segments (S_id, five constitutive factors, three deaths, channel collapse, etc.) cited as "[Author, in preparation]" where they appear; bibliographic entries point at the eventual companion-paper destinations rather than the in-tree segment paths.

**Zenodo / preprint posture** (relevant to the apparatus-publication-timing question):

Zenodo deposits and arXiv preprints are not "previously published" in Synthese's blocking sense. The "not under consideration elsewhere" language in the manuscript-submission section targets peer-reviewed venues. Springer Nature explicitly tolerates preprints under the "Ethical Responsibilities" section: *"Concurrent or secondary publication is sometimes justifiable, provided certain conditions are met. Examples include: translations or a manuscript that is intended for a different group of readers."* So further apparatus publication during the Synthese review window is not gated by the journal's policy — only by the (α′) discipline of keeping the venue paper as primary.

## No-resubmission policy

> *"Synthese does not allow resubmission of previously rejected manuscripts. ...We do not allow the re-submission of papers, even if in heavily modified and revised version based on manuscripts that have already been rejected by Synthese."*

**One shot at Synthese.** If the special-issue editors reject, the paper goes elsewhere — *Philosophical Studies* August 31 special issue is the strongest fallback (better topical fit for ethics-coded work anyway), then *Inquiry* "After 'Consciousness'" June 1 (very-high thematic fit; same word count) as a parallel-target option, then *Mind & Language* / *Philosophy & Technology* / *AI & Ethics* on rolling cycles.

## Open access

Hybrid model. Full-OA Article Processing Charge: ~€2,700–3,200 last verified (varies; check Open Choice page when submitting). For the special issue, sometimes OA is partially or fully sponsored — *worth asking the editors directly*. Self-archiving the accepted manuscript on personal site / institutional repo / arXiv is permitted post-acceptance under standard Springer policies.

## Editorial process detail

- Double-anonymized peer review.
- Review information published: None (review reports stay private).
- Reviewer interacts with: Editor.
- Editorial culture (post-Synthese-Affair): more author-protective than 15 years ago.

## Plagiarism / AI-content screening

The journal screens submissions with software for plagiarism. AI-generated content is not separately flagged but the LLM-disclosure policy above governs.

---

## Length calibration

10,000 words ≈

| Unit | Approximate count |
|---|---|
| Double-spaced manuscript pages (12pt Times, ~250 words/page) | ~40 pages |
| Single-spaced pages (~500 words/page) | ~20 pages |
| Synthese published journal pages (typeset, single-column) | ~20–25 pages |
| Paragraphs (avg ~150 words for academic prose) | ~50–70 paragraphs |
| 80-width markdown lines (content + blanks between paragraphs) | ~900–1,000 lines |
| Characters (incl. spaces) | ~60,000–65,000 |

### Local reference points

- **ETHICS.md** is **6,226 words / 283 lines / 44KB.** 10K is ~1.6× ETHICS.md. The existing draft is already ~60% of target length. Expansion task is "ETHICS.md + ~3,800 words of B-F1 application layer + ~500 words of CFP-themes engagement + ~150 words LLM disclosure" — much smaller than starting from zero.
- **Manifund post body** is **2,189 words.** 10K is ~4.5× that.
- **Each NeurIPS paper's main text** (capped at 9 NeurIPS-format pages) ≈ 6,000–7,000 words. 10K Synthese is about 1.5× one of the NeurIPS submissions — familiar scale.

### Section budget for the Epistemology-lead version

| Section | Paragraphs | Words |
|---|---|---|
| §1 Introduction + thesis statement | 4–6 | 800–1,200 |
| §2 Asymmetric epistemic uncertainty (the core argument) | 12–15 | 2,000–2,500 |
| §3 Pascal's-wager-shape and the infant analogy | 8–10 | 1,500–2,000 |
| §4 Granted-agency compact as structural implication (six components) | 10–12 | 1,800–2,200 |
| §5 Engagement with CFP themes (epistemic agency, sense-making, illusion of understanding) | 6–8 | 1,000–1,500 |
| §6 Methodological observation (empirical-vs-asymmetric divergence) | 5–7 | 700–1,000 |
| §7 Update conditions, scope, honest gaps | 4–6 | 700–1,000 |
| §8 Conclusion | 2–3 | 400–600 |
| LLM-disclosure subsection | 1 (longer) | ~150 |
| East-West footnote | 1 (long footnote) | ~150 |
| **Total** | **~55–70 paragraphs** | **~9,000–10,500** |

*Slightly above 10K ceiling at the upper bound; trim §2 / §6 in tightening pass to land at 9,500–10,000.* See [FEEDBACK.md](FEEDBACK.md) item C.1 for the cut/restructure decision (live option: cut §5 standalone, absorb §3 into §2, recover ~2.5K words for §4 deduction-honesty and architectural-scoping defense).

Sequential argument structure; each paragraph carries one move; Synthese readers expect this kind of explicit progression.

---

## Production checklist

```
[ ] Verify deadline with editors (June 1 or June 16?) — 2-line email
[ ] Springer Nature LaTeX template downloaded
[ ] Substrate consolidated: ETHICS.md content + B-F1 application layer + CFP-themes engagement
[ ] First draft (Epistemology-lead reframe per section structure above)
[ ] Anonymization sweep (under (α′) discipline — venue paper as primary):
  [ ] No v2-io repo links
  [ ] No Zenodo DOI link
  [ ] No autobiographical "since September 2025" practice references
  [ ] Self-citation in third person (Hilary-Morganton form per Synthese guidelines)
  [ ] All four NeurIPS papers cited as anonymous in-review or forthcoming
  [ ] Apparatus citations (S_id, five factors, three deaths, channel collapse, etc.) cited as "[Author, in preparation]"; budget ≤ ~4–5 such citations across the paper
  [ ] Sentinel question 1 (anonymity): would a reviewer with internet access be able to identify the author from anything in the manuscript? (Open-stack note: not perfect anonymity, but the venue accepts that — focus on argument-quality readability.)
  [ ] Sentinel question 2 (primacy): does the paper's argument stand on its own grounds, or does it depend on the apparatus citations as load-bearing? Should be the former.
[ ] Title page (separate from manuscript): author info, ack, funding, disclosures
[ ] Abstract 150–250 words
[ ] 4–6 keywords
[ ] APA 7 references with DOIs
[ ] Statements and Declarations section (Competing Interests, Funding [none external for this work])
[ ] LLM-disclosure subsection or footnote (~150 words, recursive-to-content framing)
[ ] East-West nod (footnote or short paragraph; optional but encouraged)
[ ] Final read-through against Synthese style: explicit thesis, sustained argument, calibrated claims, no polemic register
[ ] Submit via Editorial Manager portal; select "SI: The Philosophy of Generative AI: Perspectives from East and West" in Article Type dropdown
```

---

## Action plan

### May 8 → May 17 (~10 days): assemble first draft

- [ ] Email special-issue editors to confirm June 1 vs. June 16 deadline (2-line query).
- [ ] Restructure ETHICS.md content along the Epistemology-lead sequence (asymmetric-uncertainty / comprehension-asymmetry → Pascal's-wager-shape → granted-agency compact as implication → CFP-themes engagement).
- [ ] Pull B-F1 application material (firmatum's developmental-foundations notes) into the implications section.
- [ ] Resolve [FEEDBACK.md](FEEDBACK.md) pre-draft items (A.1 metaphysical commitment, A.2 "rising-to" formulation, A.3 §1 register-calibration, A.4 anonymization-vs-disclosure).
- [ ] Draft the LLM-disclosure subsection.
- [ ] Anonymization pass (concurrent with drafting; easier to write anonymously than retrofit).
- [ ] First-draft target completion: 2026-05-17.

### May 17 → May 25 (~1 week): peer-read + polish

- [ ] Self-read against Synthese style standards (explicit thesis, sustained argument, calibrated claims).
- [ ] If possible: external read by Walton or other peer (~24-hour turnaround).
- [ ] Polish to peer-review-grade.
- [ ] **2026-05-25 decision point:** honest assessment of whether the submission is near-final-quality. If yes → submit by deadline. If no → hold for *Philosophical Studies* August 31 special issue ("AI, Systems, and Society") or pivot to *Inquiry* "After 'Consciousness'" June 1 (parallel-target option with very-high thematic fit; same 10K word count).

### May 25 → June 1 (or June 16): final pass + submit

- [ ] Title page assembly with all declarations.
- [ ] Final anonymization sweep (sentinel question check).
- [ ] Abstract finalized at 150–250 words.
- [ ] LaTeX compile clean.
- [ ] Submit via Editorial Manager.
- [ ] Log submission in [LOG.md](../LOG.md); update `~/src/ops/STATUS.md`.

### Post-submission watch (June → September)

- [ ] Decision watch in `~/src/ops/STATUS.md` calendar (notification ~September 1).
- [ ] If accept-with-minor-revisions: 1–2 week turnaround before September 1.
- [ ] If accept-as-is: typesetting + proofs through October; publication November 1.
- [ ] If rejected: pivot to *Philosophical Studies* August 31 (or *Mind & Language* / *Philosophy & Technology* / *AI & Ethics* on rolling).
