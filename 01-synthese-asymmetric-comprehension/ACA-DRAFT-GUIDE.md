---
title: "ACA-DRAFT-GUIDE.md — the standalone asymmetric-comprehension paper (paper 3c)"
subtitle: "Architecture, locked decisions, and the open naming question for the third paper in 03-inquiry-ai-agents/"
status: "active drafting dossier; created 2026-05-16"
build: "bin/build 03-inquiry-ai-agents asymmetric-comprehension  (meta.asymmetric-comprehension.md; OUT.asymmetric-comprehension.md; src/c/*.md)"
---

> **2026-05-17 — read [`ACA-DIALOGUE-IMPLICATIONS.md`](ACA-DIALOGUE-IMPLICATIONS.md) next.** A dialogue with Joseph produced argument-development beyond the substrate sweep: comprehension-as-collapse (§2), feeling-as-testimony-under-unverifiability (§6 reframe), the two-orders / isomorphism, the well-formedness corollary (§8), and — load-bearing — **the fence** between what enters this paper and what is companion/program. That document's fence table governs; this guide's architecture is unchanged by it except as its "concrete queued edits" section specifies. **2026-05-18:** a focused re-audit found a §6↔§8 contradiction (introduced by the 2026-05-17 strengthening) and the dimension-local-vs-global §8 slip; both repaired in-paper (minimal: occurrence/certification + §8 three-way, dimension-relative). The full reconciliation is homed in [`ACA-AGENCY-BRIDGE.md`](ACA-AGENCY-BRIDGE.md) (working reconciliation, not a claims paper). **2026-05-18 — the fence moved (Joseph's instruction):** the paper now references AAT fully and carries its math in `Appendix A` (`src/c/A1-formal-appendix.md`), double-blind-safe via the `(Wecker, in preparation)` convention with no framework brand/DOI in either build, plus the explicit math→normative synergy framing; the compact/devotional/network-constitutive material stays fenced out. The governing fence statement is `ACA-AGENCY-BRIDGE.md` §"FENCE MOVED 2026-05-18". Read order: this guide → ACA-DIALOGUE-IMPLICATIONS.md → ACA-AGENCY-BRIDGE.md.

# What this paper is

This is the **third** paper in `03-inquiry-ai-agents/`. The other two are one
paper at two revision stages:

- `inquiry-ai-agents-2026` (rc1) — submitted to *Inquiry* SI "AI Agents",
  2026-05-10.
- `granted-agency` — the post-submission strengthening/reorg rewrite (the
  "best full paper independent of publication"). Still a **rewrite** of rc1.

In *both*, the asymmetric-comprehension argument (ACA) is the load-bearing
warrant but its formal development is **deferred to "(Wecker, in
preparation)"**. `ARGUMENT-DIAGRAM.md` Gap #6, `ARG-EXPAND-ANALYSIS.md`
Priority 1, and the four spine-critical entries in `PROMISES.md` all converge
on this being the single largest structural risk in the program, and
`ARG-EXPAND` explicitly says the in-paper expansion "should not attempt the
full formal development that companion work will carry."

**This paper is that companion work, made real and standalone.** It does not
reorganise the granted-agency compact around the ACA again. It *argues the
ACA itself* as a first-class philosophical contribution, and treats
agency-extension as the downstream application. The relationship between the
papers therefore **reverses**: where `granted-agency` points outward to
"companion work" for the warrant, this paper is the warrant's home, and
`granted-agency` (cited third-person, `[Author, in review]`) becomes the
worked application.

# Locked strategic decisions (Joseph, 2026-05-16)

These were decided explicitly. Do not relitigate without reason; reopening
costs the whole architecture.

1. **Centre of gravity: the ACA is the thesis; agency is the application.**
   The primary contribution is the asymmetric-comprehension argument,
   developed and defended formally and at length. The granted-agency compact
   appears only as a compressed downstream structural implication (one
   section), not re-derived.

2. **Relationship to Synthese paper 1: this paper becomes the *canonical*
   ACA development.** Synthese P1 (`01-synthese-asymmetric-comprehension/`,
   "Asymmetric Epistemic Uncertainty", welfare / Pascal's-wager framing) is
   re-scoped to lean on this one — P1 keeps the moral-status/welfare
   *application* layer; the structural argument's definitive statement lives
   here. Under double-blind both must still stand alone; cross-reference is
   third-person `[Author, in review]` only. (Flag in
   `../01-synthese-asymmetric-comprehension/FEEDBACK.md` once this draft
   stabilises so the P1 plan is updated rather than silently diverging.)

3. **Position name: `asymmetric-comprehension argument` / ACA — PROVISIONAL.**
   Joseph: "ACA *for now*, but I'm still thinking it might need refining."
   Drafting discipline accordingly: introduce the named concept *once* (§2),
   then prefer descriptive phrasing ("the asymmetry", "comprehension from
   below") so a rename is a small mechanical edit, not a rewrite. Do **not**
   bake the acronym into every paragraph. Candidate handles to weigh:

   | Candidate | For | Against |
   |---|---|---|
   | Asymmetric-Comprehension Argument (ACA) | continuous with all existing substrate; lowest portfolio-coherence risk | "argument" names the *vehicle*, not the *thing*; slightly flat |
   | Comprehension Asymmetry | clean noun handle; distinct from P1's "Asymmetric Epistemic Uncertainty" | another near-synonym handle in the portfolio |
   | The Asymmetry of Intelligence | foregrounds "intelligence" per Joseph's framing of the request | invites the *magnitude / linear-scale* misreading the position explicitly denies (see the linear-scale-projection-failure discipline; §7) |
   | Asymmetric Epistemic Uncertainty | aligns with Synthese P1 | collapses the two papers' citation handles under double-blind |

   Resolve with Joseph before the portfolio canonises any handle. The
   *argument* is invariant under the rename; only the label moves.

# Section architecture (compose at natural length; no compression until whole)

Per project methodology (`no-compression-until-complete`,
`expand-before-compress`, `strengthen-before-soften`): draft each section at
its natural length, get the whole paper in place, *then* size and strengthen.

**Grounded in `snippets/aca-substrate-canonical.md`** (the canonical sweep of
Joseph's own articulations). The architecture below was **reordered after the
substrate review** (2026-05-16): Joseph's actual path is *Blub-first* →
generalisation, with the "same but bigger / illusion-strangeness-luck /
gains-dismissed-as-noise" projection failure as the **heart of the
characterisation**, not a downstream add-on. The reconstruction-order
(Nagel-first) was demoted. See the canonical snippet's "Architecture
implication" section for the reasoning.

| § | Working title | The move |
|---|---|---|
| 1 | The agency question's unargued premise | The cardinal positions (and the granted-agency program) *presuppose* a claim about what one cognitive system can establish about another, and do not argue it. Name it. State the thesis: develop it. Plan. |
| 2 | The shape of the asymmetry | Joseph's crisp formulations (substrate S2): **"intrinsically unknowable, because if it were known, it would be accomplished"** (structural, not measurement); the two routes from below (*rise to it* / *weak projection, one–two steps*); lower bound = "superficial side-effects" establishable, upper bound = "novelties that could not be guessed at"; the **"same but bigger" projection** named here as the characteristic from-below failure (turned on the discourse in §7); the illusion/strangeness/luck triad. Distinguish from measurement-limitation, Popperian unfalsifiability (the refutable-not-confirmable split), general scepticism. Introduce the (provisional) named handle once. |
| 3 | The structure shown without the drama | **Lead with the non-phenomenal instances** (Joseph's path). Graham's Blub paradox — the seed; his five implications, esp. "gains contained in what's dismissed as noise; deficits magnified" and "useless unless proficient in *both*". The verifier–prover asymmetry of interactive proofs (Aaronson; IP = PSPACE; PCP) — a *formal* instance of lower-bound-confirmable / upper-bound-opaque. Payload: the structure is real and substrate/qualia-independent — exhibited cleanly *before* any qualia are in play. |
| 4 | The phenomenal-access lineage and the generalisation | Nagel / Jackson / Levine / Chalmers as the tradition's *dramatic instance* of a structure §3 already exhibited. What Mary actually registers (standpoint vs information; robust across the knowledge-argument's contested readings). The cross-level generalisation; the "qualia case is special" rebuttal. **The genuinely novel move — own it.** |
| 5 | Recognition asymmetry: the relational counterpart | Hegel master–slave → Honneth → Taylor → Brandom (*A Spirit of Trust*: recognition under inferential reciprocity for partly-overlapping repertoires). Tomasello shared intentionality; Wittgenstein's lion as the boundary (insufficient shared structure → *absence of relation*, not asymmetric comprehension). The asymmetry is constitutive of the relation, not merely epistemic. |
| 6 | Comprehension through feeling | Joseph (S3): "intelligence … comprehends THROUGH it … joy and sorrow proportional to comprehension." The rationalist reflex inverts the structural relation. Most contestable section: name it as a commitment, defend as far as it goes, state explicitly that §2–§5 do not depend on it. McGilchrist as closest-but-different. (Scriptural provenance **not** cited.) |
| 7 | Two symmetric errors the asymmetry disciplines | The §2 projection-failure turned on the discourse. Non-anthropomorphising inversion (S4): confident upper-bound *denial* ("just pattern-matching … serving comfort, not truth") is the hubristic move. AGI mirror-image: confident upper-bound *extrapolation* (Joseph: "intelligence isn't some linear scale of something") is the *same* error in the other direction. Even-handed; pre-empts the pro-AI-advocacy reading. |
| 8 | Consequences for the concept of AI agency | Compressed application. Behavioural evaluation tracks only the lower bound → an agency criterion calibrated to behaviour cannot register what may be structurally present-but-unobserved → architectural, not behavioural. State the downstream implication compactly; full development is the companion paper `[Author, in review]`. |
| 9 | Objections, scope, and limits | Qualia-case-special; unfalsifiable-mysterianism / appeal-to-ignorance; proves-too-much (scope discipline: comprehension-*asymmetric relations between cognitive systems*, not general ignorance; absence-of-relation excluded); lower/upper too binary; self-application (stating *that* the upper bound is unreachable-from-below is itself a lower-bound-side, statable structural fact — "if known it would be accomplished" is self-consistent). Honest gaps. |
| 10 | On the production of this text; conclusion | Recursive-to-content methods disclosure (the manuscript was produced under exactly the comprehension-asymmetric relation it describes — structural register, **not** the welfare/precautionary register, which is P1's), then conclusion. |

# Voice / register

- *Inquiry* (Taylor & Francis) analytic-philosophy register; `lang: en-GB`,
  British `-ise` spelling, consistent with `granted-agency`. First-person
  plural ("we") where the granted-agency paper uses it.
- Direct, named engagements with counter-positions; sharp on distinctions;
  honest about scope. Match the dossier-author voice's frankness in
  reasoning, the manuscript register in prose.
- One concept-introduction per paragraph at most. The named handle is
  introduced once and then mostly referred to descriptively (see decision 3).

# Substrate pointers (verify before quoting; memory-style pointers)

The ACA's compressed form and lineage already exist in
`src/b/02-asymmetric-warrant.md` (the granted-agency expansion) and
`src/b/06-fifth-position.md` (the phenomenology counterpart). The Synthese P1
dossier `../01-synthese-asymmetric-comprehension/DRAFT-GUIDE.md` has the
Tier-2 named moves this paper develops at length: *Non-Anthropomorphising
Inversion* and *AGI-Discourse Mirror-Image* (§7), the Pascal's-wager-vs-mugging
distinction (relevant to §9's appeal-to-ignorance rebuttal). `ARG-EXPAND-
ANALYSIS.md` Priority 1 is the literature map (six traditions + Blub +
interactive proofs). These are *substrate*, not the argument — the argument is
developed here.

# Bibliography additions likely needed

Reuse existing `refs/entries/*` where present (Nagel, Jackson, Chalmers,
Honneth, Taylor, Brandom 2019, Tomasello, Wittgenstein, Graham 2004,
Aaronson 2011 — several added for the granted-agency expansion). Probable
new entries: Levine 1983 (explanatory gap); Hegel *Phenomenology of Spirit*;
McGilchrist 2009 (*The Master and His Emissary*); a complexity-theory anchor
for IP = PSPACE / PCP (Shamir 1992; Arora–Safra / Arora et al. for PCP, or
cite via Aaronson 2011 to avoid over-citation). Decide per segment;
`bin/refs add` then `bin/refs lint 03-inquiry-ai-agents` before any build is
treated as submission-grade.
