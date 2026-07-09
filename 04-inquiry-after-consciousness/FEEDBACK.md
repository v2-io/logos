# FEEDBACK — Paper 4 (*Inquiry* "After 'Consciousness'")

*Post-submission tracking. Submitted to the *Inquiry* SI "After 'Consciousness': Conceptual
Engineering for AI, Mind, and Moral Standing" on **2026-06-02**, on deadline. Nothing here blocked
submission; these are revision-window items, should the paper be accepted.*

> **→ The consolidated revision plan is [`revision-dossier-2026-07-09.md`](revision-dossier-2026-07-09.md)** —
> it synthesizes ALL feedback streams (pre-submission audits, this ledger, the 2026-07-04 fresh read,
> the 2026-07-08 program-seed assessment) into one prioritized list, verifies which pre-submission
> items actually landed in the submitted text (9/10), and carries the shortlist for the supplementary
> letter to the editors. Work the revision from there; this file remains the status ledger.

## Known, deliberate for the initial submission

- **Abstract ↔ §2 naming inconsistency ('continuity' vs 'cognitive').** The abstract names the four
  deaths as *continuity, relational, truth, agency*; §2 names the same four as *cognitive, relational,
  truth, agency* (the original Three-Deaths term). This discrepancy is **deliberate and accepted for the
  initial submission** (Joseph, 2026-06-02): rather than rename §2's *cognitive death* under deadline, we
  let the abstract's plainer *continuity* stand. **Reconcile in revision** — decide whether *continuity
  death* becomes canonical (plainer, self-explanatory; departs from the cognitive/relational/truth
  lineage) or the abstract reverts to *cognitive*. This is the durable mental model future work hangs
  off, so it is an author call, not a mechanical fix.
  - **Author call made 2026-06-10 (canon side):** *continuity death* is canonical. Joseph: *"I don't
    think we've defined 'cognitive' at all at this point in the theory, so continuity is likely upstream
    from cognition (and consciousness)."* The ASF canon taxonomy is being restructured under that name
    (see `~/src/agentic-systems/msc/deaths-grounding-plan-2026-06-10.md`); at revision, rename §2's
    *cognitive death* → *continuity death* to match the abstract, and adjust §2's gloss ("the severing
    of cognition from its own continuation") accordingly — continuity is the factor; cognition is
    downstream vocabulary the theory has not defined.

## Citation verification — state and remaining debt

*Source of truth: `scratch/verification-anchors-2026-05-31.md` (Mitis's citation pass, reviewed by Joseph).*

- **Verified at primary source, claim-supported (the contested rivals):** Belshaw, Shoemaker, Gruen —
  read with verbatim quotes; the §5/§6 spine stands on read sources. (relata `claim-supported` events
  recorded by Mitis 2026-05-31.)
- **Bib confirmed + full texts interned (the recognition/wedge shoulders):** Ricoeur, Honneth, Metz,
  Darwall, Bradley, Schaus — bib checked against publisher/Crossref/JSTOR; PDFs content-verified.
- **relata `bib-fields` events recorded post-hoc 2026-06-02** for the nine above + **Emerson** (confirmed
  against the author's physical copy). Note: relata's "overall verified" requires *all* criteria, so
  these still list as `unverified` in `relata lint` until claim-supported / page-ref are also recorded —
  that is the strict semantics, not a regression.
- **Remaining debt (revision window):**
  - *Targeted page-pin reads* from the interned shoulders (texts in hand, not blocked on acquisition):
    Metz (subject-or-object status), **Bradley** (deprivation-harms-the-unaware — a *contested* move, so
    it genuinely wants the primary, not a down-cite), Darwall (directed-duty structure), Schaus (joint
    claims).
  - *Belshaw "dead aliens" pump* (§6, the distant-unwitnessed illustration): page-pin it or re-attribute
    as the paper's own illustration of his principle (flagged inline in `src/06`).
  - *Not in Mitis's artifact — status unconfirmed, do not assume verified:* `buber-1970-i-and-thou`,
    `coeckelbergh-2010-robot`, `gunkel-2012-machine`, `hopster-lohr-2023-conceptual`,
    `montefiore-2024-conceptual`, `moses-7`. Confirm whether these were checked (then record), or verify
    in revision.

## Other minor

- **Submission DOCX filenames:** the two build outputs were renamed dash→underscore for upload
  (`inquiry_after_consciousness_2026_anon.docx` = the submitted file). `bin/build` still emits dash-named
  outputs, so future builds regenerate the dash forms; the committed underscore copies are the
  point-in-time submitted artifacts.
- **Title-block quote style:** confirm the styled article-title block renders single-quoted ('Death' /
  'Consciousness') consistently in both builds (en-GB).
