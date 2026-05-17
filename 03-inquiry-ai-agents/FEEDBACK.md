# FEEDBACK.md — paper 3 (Inquiry "AI Agents")

*Post-submission. Resolved history and reviewer-facing positions are in [LOG.md](LOG.md). Compression roadmap is at [.archive/compression-pass.md](.archive/compression-pass.md).*

---

## Open items — `granted-agency` / rc1 lineage

**Ref verification (25 unverified entries).** Run `bin/refs verify <key> bib-fields --by joseph` against publisher pages. Priority: `soulier-2026-machine-agency`, `benthall-shekman-2023-fiduciary`, `aguirre-dempsey-surden-reiner-2020-ai-loyalty`, `anthropic-2025-end-conversations`, `paul-2014-transformative`.

---

## Open items — paper 3c (`asymmetric-comprehension`, the standalone ACA paper)

*Architecture, locked decisions, and the canonical substrate are in [ACA-DRAFT-GUIDE.md](ACA-DRAFT-GUIDE.md) and [snippets/aca-substrate-canonical.md](snippets/aca-substrate-canonical.md). Items numbered locally.*

- **3c.1 — Position-name decision (Joseph's call; provisional).** "asymmetric-comprehension argument / ACA" is the working handle "for now … might need refining" (Joseph, 2026-05-16). Candidate handles weighed in ACA-DRAFT-GUIDE.md §"Locked strategic decisions" #3. The prose introduces the name once (§2, where the *keystone* is also coined) and otherwise refers descriptively, so a rename is mechanical. Resolve before the portfolio canonises any handle.
- **3c.2 — Strengthening / sizing pass (deferred by methodology, not skipped).** ~12.5k words at natural length; no compression yet (no-compression-until-complete). When run: de-circle the *keystone* (stated ~6×; §3-theorem / §4-phenomenal / §5-relational instances *build* and stay, the bare restatements in §3-close and §6 do not add); reconsider §7's positioning (it is defensive/scope-guarding relative to the §2→§8 spine — make that honest rather than letting its prominence imply load-bearing); the §6 "follows … if one grants" framing oversells a restatement as a derivation — reframe. Empirically this pass produced ~32% reduction on the rc1 paper without losing substance; expect similar.
- **3c.3 — McGilchrist citation.** §6 references *The Master and His Emissary* (2009) in prose without a `[@]` key (kept clean to avoid an unresolved cite). `bin/refs add mcgilchrist-2009-master` then convert the §6 prose reference. Optional: `bostrom-2014-superintelligence`, a Bender-et-al "stochastic parrots" handle, `chalmers-2023-llm-conscious` if §7's positional references should become citations (currently deliberate in-prose, acceptable for the register).
- **3c.4 — Reconcile Synthese P1.** Decision #2: this paper is the canonical ACA development; P1 (`../01-synthese-asymmetric-comprehension/`) is to be re-scoped to lean on it (P1 keeps the welfare/Pascal's-wager application layer). Flag in `../01-synthese-asymmetric-comprehension/FEEDBACK.md` so P1's plan is updated rather than silently diverging under double-blind.
- **3c.5 — Containment relation is characterised by instance, not metric (honest open work, named in §9).** A formal account of "representational resources properly contained in another's" is not delivered; §9 concedes this and §9's strengthened vacuity rebuttal routes around it (Mary witnesses the *needed* representational kind metric-free). A formal treatment is genuine future work, not a defect to paper over.
