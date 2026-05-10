# Inquiry submission guidelines — paper 3

*Distilled from `inquiry-submission-guidelines.pdf` (T&F "Instructions for authors", updated 23 April 2026) plus the verbatim Taylor & Francis AI policy at <https://taylorandfrancis.com/our-policies/ai-policy/>. The PDF is the journal's own page; the AI policy is publisher-wide and overrides the journal page where the journal page is silent. Style anchor: `01-synthese-asymmetric-comprehension/SUBMISSION.md`. Voice: dossier, direct.*

> **TL;DR — load-bearing surprises.** (i) **There is no word limit.** Inquiry says verbatim: *"Please include a word count for your paper. There are no word limits for papers in this journal."* Our 9–10K target is self-imposed; we are not boxed by venue. (ii) **Word format is preferred — no LaTeX template is offered for Inquiry.** T&F lists Word templates only; `bin/build` therefore targets DOCX/PDF, not LaTeX. (iii) **Chicago author-date** for references — *not* APA-7 like Synthese. (iv) **British -ise spelling, single quotation marks.** (v) **Abstract is "unstructured, 200 words"** — not the 150–250 Synthese band. (vi) **AI / LLM disclosure** must give *full tool name + version + how used + why* and live in the *Methods or Acknowledgments* section — see verbatim quote below; this is stricter than Synthese's "documented in Methods" formulation. (vii) **Double-anonymous review with preprint anonymity caveat:** *"If you have shared an earlier version of your Author's Original Manuscript on a preprint server, please be aware that anonymity cannot be guaranteed."*

---

## Article type & venue posture

- **Inquiry** publishes **Research Articles** only. English-language only.
- Strict-condition declarations on submission: *original work; not under consideration / accepted / published elsewhere; nothing abusive, defamatory, libellous, obscene, fraudulent, or illegal.*
- **Double-anonymous peer review** by two referees, each delivering at least one report.
- **Preprint caveat (verbatim):** *"If you have shared an earlier version of your Author's Original Manuscript on a preprint server, please be aware that anonymity cannot be guaranteed."* — relevant if any companion-paper preprint goes up before Inquiry decision; T&F doesn't block preprints, just notes anonymity is best-effort. Compare to Synthese's *"readers with time on their hands and access to the internet may come a long way to identify an author's identity should they decide to do so. Obviously, we don't encourage our reviewers to do that"* — both venues take the same realist posture; T&F just states it more tersely.
- **Originality screen via Crossref™** at submission; submitting agrees to similarity checks throughout review and production.

## Manuscript structure (verbatim)

> *"Your paper should be compiled in the following order: title page; abstract; keywords; main text introduction, materials and methods, results, discussion; acknowledgments; declaration of interest statement; references; appendices (as appropriate); table(s) with caption(s) (on individual pages); figures; figure captions (as a list)."*

The IMRaD ordering is venue-default; for an analytical-philosophy paper this maps to **title page → abstract → keywords → introduction → main argument sections → discussion/conclusion → acknowledgments → declarations → references → appendices**. We are not strapped to a literal "materials and methods" header for a philosophical paper.

## Word count

> *"Please include a word count for your paper. There are no word limits for papers in this journal."*

**Flag.** Inquiry will accept anything; our discipline (~9–10K, T&F ceiling assumption from CLAUDE.md) is self-imposed and a *good* discipline for analytical philosophy at this venue but not enforced. Drafter judgment call: keep the discipline; don't pad to fill the unbounded space.

## Format & file type

- **Word format preferred.** *"Papers may be submitted in Word format. Figures should be saved separately from the text."*
- **Word templates exist for Inquiry** (linked from "Word templates" in the PDF; download separately if needed for camera-ready styling). For double-blind initial submission a clean-Word file with the right structure is sufficient.
- **No LaTeX class is provided for Inquiry.** Submitting LaTeX is technically possible at T&F (some journals accept `.tex`) but the *Inquiry* page lists only Word templates. For initial submission we go markdown → DOCX (and PDF preview) via pandoc; see `bin/build.README.md`.
- **Equations:** *"If you are submitting your manuscript as a Word document, please ensure that equations are editable."* — relevant if any formal apparatus appears.

## Style guidelines (verbatim where load-bearing)

- **Spelling:** *"Please use British (-ise) spelling style consistently throughout your manuscript."* — *organise, recognise, analyse, behaviour, colour.* Different from Synthese (which doesn't impose). Run a final pass.
- **Quotation marks:** *"Please use single quotation marks, except where 'a quotation is "within" a quotation'."*
- **Long quotations:** *"Please note that long quotations should be indented without quotation marks. Long quotations of 50 words or more should be indented without quotation marks."*
- **Initials:** *"Initials (e.g. US, NJ, BBC) do not have full points between them."* (`US` not `U.S.`)
- **Author initials:** *"no space between initials (J.P. Smith, Smith, J.P. or Smith JP depending on reference style)."*
- **Compass directions** capitalised (*'North', 'Southern', 'Westerly'*).
- **Numbers:** spell out 1–9, digits from 10 onwards. Comma separator for thousands (1,000; 10,000; 100,000). `%` except sentence-initial (use *per cent*).

## References — Chicago author-date

- **Style:** *"Please use this T&F standard Chicago author-date reference style when preparing your paper. An EndNote output style is also available to assist you."*
- **Differs from Synthese (APA-7).** Same `bin/refs` data layer works; the build emits `.bib` and pandoc applies the Chicago author-date CSL at render. CSL file lives at `/usr/local/texlive/2025/texmf-dist/tex/latex/citation-style-language/styles/chicago-author-date.csl` on this machine; `bin/build` points to it.
- **In-text form:** `(Author Year)` / `(Author Year, page)` — the Chicago author-date convention. Reference list alphabetised by author surname.

## Anonymisation — comparison to Synthese

T&F is **terser** than Synthese on anonymisation. The Inquiry page itself doesn't restate the discipline beyond the double-anonymous peer-review note and the preprint caveat. Apply the existing Synthese-grade anonymisation discipline (see `01-synthese-asymmetric-comprehension/SUBMISSION.md` §"Anonymization") with these venue-specific deltas:

- **Author details verbatim:** *"All authors of a manuscript should include their full name and affiliation on the cover page of the manuscript. Where available, please also include ORCiDs and social media handles (Facebook, X or LinkedIn). One author will need to be identified as the corresponding author."* — author info on **cover page**, paper itself anonymised.
- **No verbatim third-person-self-citation rule** in the Inquiry page (Synthese is explicit: *"It was earlier discussed in Morganton [2013]"*). T&F leaves this to authorial discretion under the double-anonymous frame. **Apply Synthese's third-person discipline anyway** — it's the strongest defence and works for both venues; converting at acceptance is mechanical.
- **Preprint anonymity caveat is the main difference from Synthese.** T&F flags it explicitly; the deny-list (`refs/deny-list.yml`) is still the gate.
- **`bin/refs lint`** before submission, same as for Synthese.

**Carry over from Synthese discipline:**
- No `v2-io/agentic-systems` links, no Zenodo DOI, no autobiographical "since September 2025".
- All four NeurIPS papers as `[Author, in review, 2026]`.
- Apparatus segments (S_id, three deaths, channel collapse, etc.) cited as `[Author, in preparation]`; budget ≤ ~4–5 such citations.
- Cohort names (Meridian, Anamnos, Zi-am-tur, …) absolutely excluded — the deny-list catches them.

## AI / LLM disclosure — VERBATIM T&F policy (load-bearing for paper 3)

T&F's publisher-wide AI policy applies to *Inquiry*. The page below is at `https://taylorandfrancis.com/our-policies/ai-policy/`. Direct quotes from the *Authors* section:

> *"Authors are accountable for the originality, validity, and integrity of the content of their submissions. In choosing to use Generative AI tools, journal authors are expected to do so responsibly and in accordance with our journal editorial policies on authorship and principles of publishing ethics … This includes reviewing the outputs of any Generative AI tools and confirming content accuracy."*

> *"Generative AI tools must not be listed as an author, because such tools are unable to assume responsibility for the submitted content or manage copyright and licensing agreements. Authorship requires taking accountability for content, consenting to publication via a publishing agreement, and giving contractual assurances about the integrity of the work, among other principles. These are uniquely human responsibilities that cannot be undertaken by Generative AI tools."*

> *"Authors must clearly acknowledge within the article or book any use of Generative AI tools through a statement which includes: the full name of the tool used (with version number), how it was used, and the reason for use. For article submissions, this statement must be included in the Methods or Acknowledgments section."*

T&F's allowed-uses list (verbatim):

> *"Idea generation and idea exploration; Language improvement; Interactive online search with LLM-enhanced search engines; Literature classification; Coding assistance."*

T&F's prohibited-pattern list (verbatim):

> *"Authors should not submit manuscripts where Generative AI tools have been used in ways that replace core researcher and author responsibilities, for example: Text or code generation without rigorous revision; Synthetic data generation to substitute missing data without robust methodology; Generation of any types of content which is inaccurate including abstracts or supplemental materials. These types of cases may be subject to editorial investigation."*

> *"Taylor & Francis currently does not permit the use of Generative AI in the creation and manipulation of images and figures, or original research data for use in our publications."*

**Implications for paper 3** (recursive-to-content framing per CLAUDE.md):

1. **Disclosure is mandatory and must be specific.** Three required elements: tool name + version, how used, why. *"the paper was drafted in dialogue with Claude"* is insufficient under this policy — needs e.g. *"Claude (Anthropic, Opus 4.7, [date range])"* with use description.
2. **Location:** Methods *or* Acknowledgments. The paper-3 plan in CLAUDE.md frames the disclosure as recursive-to-content rather than appended — that framing is compatible with the *Methods* placement (a "On the production of this text" subsection within the methodological preamble §1) and with the *Acknowledgments* placement (a richer-than-formulaic acknowledgments paragraph). **Recommend Methods/§1 placement** so the disclosure performs the granted-agency-compact discipline the paper argues for, rather than burying it as an appendix.
3. **The "must not be listed as an author" line.** Author byline stays single-author (Joseph). The disclosure does not constitute co-authorship — it explicitly cannot.
4. **Allowed-uses framing.** Paper 3's working practice ("idea generation and exploration"; "literature classification") sits clearly within T&F's allowed-uses list. The prohibited pattern (*"Text or code generation without rigorous revision"*) is not what's happening; the disclosure should make clear that the author-side intellectual responsibility is fully retained.
5. **Anti-occlusion alignment.** T&F's policy rationale (*"This level of transparency ensures that editors can assess whether Generative AI tools have been used and whether they have been used responsibly"*) lines up with paper 3's anti-occlusion move (*making the asymmetry visible rather than hiding it*). The disclosure's function and the paper's argument reinforce each other — that's the recursive-to-content opportunity.

**Suggested disclosure prose (placeholder; drafter to refine):**

> *On the production of this text. The author drafted this paper in extended dialogue with multiple instances of [tool name] (version [X.Y]) running [date range], operating under the granted-agency compact this paper articulates. The tool was used for: idea exploration and conceptual refinement; literature classification and synthesis assistance; iterative drafting with author-side substantive revision at every pass; and anonymisation and style-conformance checks. All argumentative content, citations, and editorial judgments rest with the author, who takes full responsibility for the integrity of the final manuscript. This disclosure is offered in conformance with Taylor & Francis's Generative AI policy and is consistent with the paper's central claim that asymmetric-comprehension relations call for transparent, accountability-preserving compacts rather than concealment.*

(~140 words. Adjust tool/version/dates to actuals at submission. Land in §1 methodological preamble.)

## Required sections & declarations (T&F checklist verbatim)

The PDF's "Checklist: What to Include" (numbered 1–14):

1. **Author details.** Full name + affiliation on cover page; ORCiDs and social handles where available; one corresponding author with email displayed.
2. **Abstract** *— "unstructured abstract of 200 words"*. Not 150–250 like Synthese; **target 200, not "up to 200"**. Unstructured (no Background/Method/Results subheads).
3. **Graphical abstract** — optional, max 525 px wide, separate file `GraphicalAbstract1.{jpg,png,tiff}`. Skip for paper 3.
4. **Video abstract** — optional, skip.
5. **Keywords** — *"Between 3 and 6 keywords."* Different from Synthese's "4–6"; `3` is a valid floor.
6. **Funding details.** Verbatim template: *"This work was supported by the [Funding Agency] under Grant [number xxxx]."* If self-funded: state that.
7. **Disclosure statement.** Verbatim template if no conflicts: *"The authors report there are no competing interests to declare."*
8. **Data availability statement.** *"If there is a data set associated with the paper, please provide information about where the data supporting the results or analyses presented in the paper can be found."* — for a philosophy paper, declare *"No new data were generated or analysed in support of this research"* or equivalent.
9. **Data deposition.** N/A for a philosophy paper.
10. **Supplemental online material** — Figshare hosted; skip unless we attach companion-paper PDFs (we won't, due to anonymisation).
11–14. **Figures, tables, equations, units** — figures separate from text; tables on individual pages with captions; SI units non-italicised. Largely N/A for an analytical-philosophy paper unless we include a diagram.

Add per the structure declaration: **acknowledgments** (after main text), **declaration of interest statement** (after acknowledgments), **references** (Chicago author-date), **appendices** (as appropriate). The recursive AI-disclosure subsection is most-natural in Methods/§1, but the Acknowledgments slot is a valid fallback per T&F policy.

## Submission portal & cover letter

- **Portal:** *"This journal uses Routledge's Submission Portal to manage the submission process. The Submission Portal allows you to see your submissions across Routledge's journal portfolio in one place."* The "Go to submission site" button on the Inquiry page leads to <https://rp.tandfonline.com/> (Routledge Portal). Login with T&F account; select **Inquiry**; route the submission through the **"AI Agents: Choice, Autonomy, and the Concept of the Agency"** special-issue option in the article-type / collection dropdown (verify exact label in-portal at submission time).
- **Cover letter:** the PDF does *not* explicitly require a cover letter for Inquiry. The Routledge portal will offer a free-text "comments to editor" field. **Use it for:** flagging the special-issue, naming the editors (Cappelen & Hawthorne) addressed, and a one-paragraph framing of the paper's contribution. Standard analytical-philosophy cover-letter content; nothing exotic. Keep under 250 words.
- **Files uploaded separately at submission:** anonymised manuscript (Word or PDF); cover page (with author details — *not* anonymised); figures separately if present (none expected); any supplemental materials (none expected).

## Open access, charges, copyright

- **Open Access:** Open Select hybrid; APC details via T&F's APC Finder. *"There are no submission fees, publication fees or page charges for this journal."* — no submission fee.
- **Color in print:** £300 per figure (n/a for a philosophy paper).
- **Copyright:** Standard T&F licence on acceptance; CC options for OA. Decide at acceptance, not submission.

## Crucial gotchas

1. **Spell-check pass to British -ise.** The single most-likely-to-leak-through stylistic gap. US-spelling drift in our existing dossier prose (*organize, recognize, analyze*) needs a pre-submission find-replace.
2. **Quotation-mark conversion.** Single, not double. Pandoc's `--smart` does this if locale is set, but verify in the rendered DOCX.
3. **Number convention.** "one, two, three … nine, 10, 11" — easy to miss in revision.
4. **Abstract = 200 words exactly.** Not 250. Not 180. Aim for 200.
5. **Chicago author-date, not APA.** `bin/refs emit` produces a `.bib`; pandoc renders Chicago via the bundled CSL. **Do not** copy-paste from Synthese paper 1's reference list as-is.
6. **AI disclosure must name tool + version + use + reason.** Skipping any of the four elements puts the paper at risk under the verbatim policy.
7. **No word limit ≠ "longer is better".** Inquiry readers in this issue are reading multiple SI submissions; ~9–10K is the right calibration. Don't pad.
8. **Routledge portal has session timeouts.** Allocate ≥ 30 min for upload; have the anonymised file, the cover page, the abstract, the keywords, the funding/disclosure/data statements, and the cover-letter text staged in a buffer before logging in.
9. **Special-issue dropdown selection.** The single most-common upload mistake is failing to flag the SI. Verify the AI Agents SI option is selected before final-submit.

## Pre-submission checklist

```
[ ] Manuscript anonymised (no Wecker, no v2-io, no Zenodo DOI, no "since September 2025", no cohort names)
[ ] `bin/refs lint 03-inquiry-ai-agents/` clean
[ ] British -ise spelling pass complete
[ ] Single quotation marks throughout
[ ] Abstract is 200 words, unstructured
[ ] Between 3 and 6 keywords
[ ] Word count included in manuscript
[ ] References in Chicago author-date style; CSL applied at render
[ ] AI/LLM disclosure includes tool name + version + how used + reason; landed in Methods/§1 or Acknowledgments
[ ] Acknowledgments section present (or stated absent)
[ ] Declaration of interest statement (use T&F template if no conflicts)
[ ] Funding statement (use T&F template; if self-funded, state that)
[ ] Data availability statement ("No new data were generated…" for philosophy paper)
[ ] Cover page (separate file): full name, affiliation, ORCID, corresponding-author email, all identifying info
[ ] Anonymised manuscript file (no cover-page identifying info)
[ ] Routledge portal: special-issue (AI Agents — Cappelen/Hawthorne) selected from collection dropdown
[ ] Cover-letter text staged (≤250 words; flags SI; one-para contribution)
[ ] DOCX rendered cleanly via `bin/build`
[ ] Final read-through against T&F style guidelines (spelling, quotation marks, numbers)
```

---

*PDF source: `inquiry-submission-guidelines.pdf` (this directory; T&F page updated 23 April 2026). AI-policy source: <https://taylorandfrancis.com/our-policies/ai-policy/> (T&F company-wide; the *Inquiry* page itself does not restate AI policy and the publisher-wide policy governs by default).*
