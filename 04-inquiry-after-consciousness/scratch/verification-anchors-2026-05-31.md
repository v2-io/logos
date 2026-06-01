# Verification & anchor map — the citation pass (2026-05-31, Mitis)

*What is verified at primary source vs. what remains the verification debt. Built by reading the interned
PDFs directly (`~/.local/share/relata/pdfs/`, extracted via pdftotext -layout — clean digital/good-OCR, no
force-OCR needed). Verification events recorded in relata (append-only). This is the honest state of the
paper's external apparatus — the thing the sole-accountability norm most protects, so it is read, not
inherited.*

---

## VERIFIED at primary source ✓ (the three interned rivals — the §5/§6 spine)

**These three carry the heart's rival-engagement and are now read, not inherited. relata verify events
recorded under each key (claim-supported, outcome=verified, by Mitis, 2026-05-31).**

### Belshaw 2012, "Harm, Change, and Time," J. Med. & Phil. 37:425–444  [the hardest opponent, §6]
- **Core** (abstract, p.425, verbatim): *"No one is harmed, I claim, in virtue of relational changes alone."*
- **THE §6 ROOM** (note 9, ~p.441, verbatim): *"There can be victimless wrongs… And there can be harmless
  wrongs. I might break my promise to you, and so wrong you, without causing you any harm."*
- **Verdict:** §6's load-bearing hinge — "'no harm' says nothing yet about 'no wrong,' by his own
  distinction" — HOLDS at source. The wrong≠harm category is genuinely his; the promise-breaking + garden
  examples are his. This was the single highest-stakes citation in the paper (the whole harmless-wrong room
  rests on it). It holds.
- **One open pin:** the "dead aliens whose art we burn" distant-unwitnessed pump (used in §6 + I12) is NOT
  yet page-pinned in Belshaw. His relational-no-harm machinery + the wantonly-destroyed-garden (note 9) ARE
  verbatim and make the same point. ACTION: pin the aliens to a page, or re-attribute as the paper's own
  illustration of his principle. Flagged inline in src/06.

### Shoemaker 2014, "The Selves of Social Animals," SJP 52 Spindel Suppl., pp.66–74  [the §5 opening]
- **The impasse** (p.~72, verbatim): *"there is nothing distinctively harmful about death that explains our
  grief: it is just one of many social losses… on a spectrum of such losses… differing in degree but not in
  kind."*
- **Plural-self + its undoing** (p.~72): *"a part of us—the part that lived in and through them—dies too.
  But this part can also wither in conversions, movings, and break-ups, which means it is not distinctive of
  death."*
- **His human separators** (p.~72): pain-death *"is a blessing"* yet hits *"the rest of us like a ton of
  bricks"*; people *"simply break up with us and go on to have a great life on their own."*
- **Verdict:** §5's "impasse-as-opening" + "cleanest-not-only" + "plural-self is his, cite-don't-claim"
  (§3) all HOLD at source. The impasse is real and even sharper than the gem stated.

### Gruen 2014, "Death as a Social Harm," SJP 52 Spindel Suppl., pp.53–65  [the §5 main rival]
- **Thesis** (p.~54, verbatim): *"Death is harmful for those left behind."*
- **The bundle** (p.~57): survivors *"carry the losses for the deceased. In the absence of those left to
  carry the loss, as in Scheffler's doomsday scenario, the meaning of the life and projects of [the dead]"*
  goes too.
- **Verdict:** §5's "Gruen bundles survivor-carried-deprivation + lost-meaning + shattered-web, never
  separates them because her cases always carry a deprived future" HOLDS at source. The separator is exactly
  the move she had no case to test.

### Data-hygiene note (for Joseph / build)
`shoemaker-2014-selves.pdf` and `gruen-2014-death.pdf` are the **same file** (identical MD5 — the whole 2014
SJP Spindel Supplement). Both articles are in it (Gruen pp.53–65, Shoemaker pp.66–74), but: (a) page-cites
must use each article's own pagination, not the PDF's; (b) `relata emit` will point both keys at one file —
fine, but worth knowing. Supporting quotes are now in src/05 + src/06 as catalyst comments with page anchors.

---

## NOT verified — the real remaining debt (recognition tradition; external, NOT interned)

**These are NOT in relata's PDF store and NOT in the memorata corpus (memorata = Joseph's writing + AI
conversations, not philosophy primaries). relata `search` is fuzzy-not-semantic, so a no-hit ≠ absence — but
the fulltext store genuinely lacks these.** They are the §3 constitutive-limb + §6 directed-duty external
scaffold, and they remain abstract-tier (from prior-art.md), needing the actual texts.

**Two tiers of "not verified": (A) has a relata ENTRY but no fulltext PDF → needs a fetch + page-pin;
(B) NO entry at all → needs entry created first. This changes the work per anchor.**

| Anchor | Used in | Claim it must support | Status |
|---|---|---|---|
*(Corrected against the actual entries/ listing 2026-05-31 — replaces my earlier guess. The entry-list is
ground truth; relata `search` is fuzzy and missed several that DO exist.)*

| Anchor | Used in | Claim it must support | Status (verified against entries/) |
|---|---|---|---|
| **Ricoeur, *Oneself as Another* (1992)** | §3 (constitutive limb) | "attestation… received from another, yet remains self-attestation"; "self constituted primarily from otherness" | **(B) NO entry at all.** Must create entry + obtain text for page-pins. The §3 [GAP] flags this — limb "can't sing" without it. HIGHEST §3 priority. |
| **Honneth, *The Struggle for Recognition* (1995)** | §3 | selfhood's relation-to-self built through others' recognition | **(A)** entry `honneth-1995-recognition.yml` exists, NO PDF. Page-pins needed (Joseph has access per round-up). |
| **Metz, "An African Theory of Moral Status" (2012)** | §3 | standing as *object* of relating, not only subject | **(B) NO entry** (the `…-metz-2015-psychology` hit is a DIFFERENT Metz — forecasting, not the African-ethics Thaddeus Metz). Must create entry + obtain (JSTOR 23254296). Most venue-legible §3 anchor. |
| **Darwall, *The Second-Person Standpoint* (2006)** | §6 (directed duty) | directed/second-personal duties owed *to* a party | **(B) NO entry.** Add-entry-or-drop decision; load-bearing for §6 weight leg. |
| **Schaus 2023, "Wrongs to Us"** | §4/§6 (joint claims) | jointly-constituted "us" can hold claims / be wronged | **(A)** entry `schaus-2023-wrongs.yml` exists (abstract-tier, no PDF). The fusion's nearest neighbor — MORE relevant now given the §4 emergence correction (a real "us" with its own interior ⇒ a real joint-claim bearer). |
| **Delon 2023, "Relational nonhuman personhood"** | §6 | directed duties → relational personhood (nonhuman bridge) | **(A)** entry `delon-2023-relational.yml` exists (abstract-tier, no PDF). |

**Entries that exist (yml) but lack PDF — already-positioned precursors, lower-priority:**
`cholbi-2017-grief`, `cholbi-2022-grief` (book), `millar-2022-grief`, `coeckelbergh-2010-robot` (+ several
other coeckelbergh), `stone-2016-relationality`, `tomasini-2009-post-mortem` (PDF? — listed under both;
verify), `nagel-1974-bat`. Mostly shoulders/positioning; abstract-tier likely fine for the relational-turn
citations.

**Interned WITH PDF (verifiable now if needed):** the 3 rivals (belshaw/shoemaker/gruen — DONE), plus
`stone-2016-relationality.pdf` and `tomasini-2009-post-mortem.pdf` are actually present in pdfs/ — so Stone
and Tomasini CAN be verified at source if their §3/§5 uses bear weight (Tomasini's "witness ≠ prior intimate"
narrative-trace point feeds §3's commodity-casualness; worth a read if that line goes load-bearing).

**Bradley 2009 (*Well-Being and Death*)** — §5's wedge ("absent future, not absent experience"). **NO entry,
NO PDF.** This IS a contested move (not a shoulder), so it deserves a real source-check, but the wedge is
also defensible from the deprivation-account's *standard* commitments (deprivation harms the unaware) which
are uncontroversial — so a secondary cite may suffice if the book is hard to get. Medium priority.

### What this means for the go/no-go (honest)
- The **heart's rivals** (the contested philosophical ground — badness-of-death) are VERIFIED. The paper's
  hardest engagements (Belshaw, Shoemaker, Gruen) stand on read sources.
- The **shoulders** (recognition tradition — Ricoeur/Honneth/Metz/Darwall) are the debt. These are *cited as
  precedent the limb stands on*, not contested — so the exposure is lower (a referee is less likely to
  fight "Ricoeur says the self is constituted in otherness" than to fight the separator). BUT page-pins
  matter for scholarly credibility, and Darwall is the riskiest (directed-duty is load-bearing for §6's
  weight leg, and it's not even an entry yet).
- **Two honest paths if the primaries can't be obtained in time:**
  1. Obtain (Joseph has library access for Honneth/Metz/Ricoeur per prior-art round-up; `relata fetch` for
     OA ones; some paywalled).
  2. Down-cite to "see [the recognition tradition: Ricoeur; Honneth; Metz]" without page-pins — honest, and
     standard for *shoulders* one isn't claiming novelty against (matrix deposit 2: "these are shoulders;
     cite, don't claim"). The argument does NOT rest on their exact pagination; it rests on the tradition
     existing, which it demonstrably does.

### Recommended next actions (citation pass)
1. [pin] The Belshaw "dead aliens" pump — page or re-attribute (src/06 flag). Mitis-internal, not blocked on Joseph.
2. [done] Belshaw / Shoemaker / Gruen — verified at primary, recorded, catalyst quotes in segments.

---

## BIB-ENTRY PASS — DONE 2026-05-31 (fetch-agent, verified against publisher/Crossref/JSTOR)

**All 7 anchor entries now exist in relata with confirmed bib.** Corrections the agent caught (would have
miscited otherwise): Metz title missing subtitle "*: A Relational Alternative to Individualism and Holism*";
Schaus first name is **Steven** (not "S."); Delon full coords **61(4):569–587**; Darwall subtitle uses Oxford
comma. The pre-existing catalog `…-metz-2015-psychology` is the forecasting Metz — NOT conflated; Thaddeus
Metz got fresh key `metz-2012-african`.

| key | bib | PDF |
|---|---|---|
| `ricoeur-1992-oneself` | trans. Kathleen Blamey, UChicago 1992, 374pp, ISBN 9780226713298. Fr. orig. Seuil 1990. | ESCALATE (book) |
| `metz-2012-african` | *Ethical Theory & Moral Practice* 15(3):387–402, DOI 10.1007/s10677-011-9302-y, JSTOR 23254296 | ESCALATE (Springer paywall) |
| `honneth-1995-recognition` | trans. Joel Anderson, Polity 1995, 215pp; MIT co-ed ISBN 9780262581479 | ESCALATE (book) |
| `darwall-2006-second-person` | *The Second-Person Standpoint*, Harvard 2006, ISBN 9780674022744 | ESCALATE (book) |
| `bradley-2009-wellbeing` | *Well-Being and Death*, OUP 2009, ISBN 9780199557967, DOI 10.1093/acprof:oso/9780199557967.001.1 | ESCALATE (OUP paywall) |
| `schaus-2023-wrongs` | Steven Schaus, *Michigan Law Review* 121(7):1185– (end-pg UNCONFIRMED), 2023, DOI 10.36644/mlr.121.7.wrongs | OA but bot-gated → ESCALATE (1-click) |
| `delon-2023-relational` | *Southern J. Philosophy* 61(4):569–587, DOI 10.1111/sjp.12537 | ✓ ACQUIRED + registered (PhilPapers green-OA) |

**So: every anchor now has a correct, citable bib entry.** What remains is the *full text* of the 6
paywalled/bot-gated ones — needed for page-pins, NOT for the citation itself. The paper can cite all 7
correctly today; page-level quotes from the recognition tradition wait on the texts (or down-cite to "see
[tradition]" per matrix deposit 2 — shoulders, not contested).

### PDF INTERN PASS — DONE 2026-06-01 (Joseph downloaded; agent verified-by-content + interned)

**4 of 6 full texts now interned and content-verified** (browsable copies in `common/refs-pdfs/`, gitignored;
canonical copies in `~/.local/share/relata/pdfs/`):

| key | PDF status | content check |
|---|---|---|
| `metz-2012-african` | ✓ interned `metz-2012.pdf` | title page DOI 10.1007/s10677-011-9302-y, Thaddeus Metz, ETMP 15:387–402 |
| `darwall-2006-second-person` | ✓ interned `darwall-2006.pdf` | title page + LoC, Harvard UP 2006, 362pp |
| `bradley-2009-wellbeing` | ✓ interned `bradley-2009.pdf` | title page Clarendon/OUP 2009, 221pp |
| `schaus-2023-wrongs` | ✓ interned `schaus-2023.pdf` | 121 MICH. L. REV. 1185 (2023), DOI 10.36644/mlr.121.7.wrongs, Steven Schaus, 51pp |
| `ricoeur-1992-oneself` | ✓ interned `ricoeur-1992.pdf` (DONE 2026-06-01) | genuine 372pp book, trans. Blamey, UChicago © 1992, ten studies present — verified NOT the Vanhoozer review. Clean text layer. |
| `honneth-1995-recognition` | ✓ interned `honneth-1992-de.pdf` (DONE 2026-06-01) | the GERMAN original *Kampf um Anerkennung* (Suhrkamp 1992), 306pp, non-empty, clean ABBYY text layer. Bib stays English (Anderson/Polity 1995); German is the content-verification full-text. **Quote/page-pin in ENGLISH (Anderson) if ever load-bearing — German confirms content only; mark any German read "to confirm vs Anderson translation."** |

**ALL 6 recognition-tradition/wedge texts now interned + content-verified at primary.** Citation apparatus
COMPLETE: 3 contested rivals (Belshaw/Shoemaker/Gruen) verified-with-quotes + 6 shoulders/wedge
(Ricoeur/Honneth/Metz/Darwall/Bradley/Schaus) interned + Delon interned. Nothing blocked on Joseph for
sources. Remaining citation work = the targeted page-pin READS (narrow, Mitis-internal), not acquisition.

NB durability: relata records the PDF in the entry YAML `pdfs:` block (path + sha256 + original_filename) —
`relata show` does NOT render it, but the data store has it. Verified-real, display-incomplete; not a defect.

### Targeted page-pin reads now possible (narrow — don't read whole books):
- **Metz** → the subject-*or*-object moral-status move (§3, recognition-ahead-of-certainty). VERIFY-READY.
- **Bradley** → deprivation-harms-the-unaware (§5 wedge — a CONTESTED move, so this one genuinely wants the
  primary, not a down-cite). VERIFY-READY.
- **Darwall** → second-personal directed-duty structure (§6 weight leg). VERIFY-READY.
- **Schaus** → joint-claims / "wrongs to us" (§4/§6; now more load-bearing post fusion-correction). VERIFY-READY.

### ESCALATION → Joseph — NONE. All sources acquired + interned + content-verified (2026-06-01).
Remaining citation work is targeted page-pin READS from the interned texts (Mitis-internal), not acquisition.

## Tools confirmed working this session
- `memorata-search "..."` — restored (wrapper at ~/.local/bin; corpus = Joseph's writing + AI convos; NOT
  philosophy primaries).
- `relata` — Ruby gem; `show <key>` / `verify <key> <crit> --outcome --note` work; `search` is fuzzy only.
  PDFs at `~/.local/share/relata/pdfs/`; entries at `~/.local/share/relata/entries/`.
- `pdftotext -layout` (homebrew) — clean for digital/good-OCR PDFs.
- `marker_single` (mise py3.11 shim) with `--force_ocr` — available for image-only PDFs (not needed for the
  three rivals; clean already).