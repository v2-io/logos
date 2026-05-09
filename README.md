# synthese-paper — 2026 academic-philosophy paper portfolio

*Originally created 2026-05-08 as the working dossier for a single Synthese paper. As of 2026-05-09 it carries **four parallel papers** at varying stages of readiness. The repo name is historical; the contents are now a portfolio. See [LOG.md](LOG.md) for the restructure entry.*

---

## What's here

Four target papers, each in its own numbered directory; shared substrate at `common/` and a citation-management system at `refs/`; program-wide strategy and status at top level.

| Dir | Paper | Venue | Deadline | Status |
|---|---|---|---|---|
| **[`01-synthese-asymmetric-comprehension/`](01-synthese-asymmetric-comprehension/)** | Asymmetric epistemic uncertainty / granted-agency compact | Synthese special issue *"The Philosophy of Generative AI: Perspectives from East and West"* | 2026-06-01 *or* 2026-06-16 (verify) | Substrate ready; not yet drafted |
| **[`02-synthese-methodology/`](02-synthese-methodology/)** | Epistemic discipline for LLM-mediated audit of theoretical frameworks | Synthese rolling submission, Methodology pillar | Rolling | Dossier seeded; sprint after paper 1 |
| **[`03-inquiry-ai-agents/`](03-inquiry-ai-agents/)** | Granted-agency compact as structurally-grounded extension of agency to AI | *Inquiry* special issue *"AI Agents: Choice, Autonomy, and the Concept of the Agency"* (Cappelen & Hawthorne, eds.) | **2026-05-10 — TOMORROW** | **Active drafting today** |
| **[`04-inquiry-after-consciousness/`](04-inquiry-after-consciousness/)** | Conceptual engineering for AI moral standing without consciousness | *Inquiry* special issue *"After 'Consciousness': Conceptual Engineering for AI, Mind, and Moral Standing"* (same editors) | 2026-06-01 | Placeholder; dossier TBD |

The two Synthese papers are a substantively-coupled pair (asymmetric-comprehension argument and audit-discipline are load-bearing on each other under double-blind anonymization — see [02-synthese-methodology/FEEDBACK.md §C.1](02-synthese-methodology/FEEDBACK.md)). The two Inquiry papers share editors, so signal-quality across them is bidirectional.

---

## Top-level files

| File | Role |
|---|---|
| **[STRATEGY.md](STRATEGY.md)** | Why this paper, this way. Currently paper-1-flavored (Path A epistemology-lead, (α′) thesis-primacy, Beyond-Synthese companion-paper portfolio, calibration risks R1–R10, cross-reference to `01-…/synthese-thoughts.md`); slated to evolve into program-wide strategic framing as papers 2–4 mature. |
| **[LOG.md](LOG.md)** | Append-only program-wide status log. Newest first. Append after non-trivial changes. |
| **[CLAUDE.md](CLAUDE.md)** | Orientation for future Claude Code instances working in this repo. Conventions, locked-in decisions, external-substrate pointers, refs-machinery usage. **Read first if you're new or returning.** |
| **[README.md](README.md)** | This file. Navigation only. |

## Shared resources

| Dir | Role |
|---|---|
| **[`common/`](common/)** | Shared philosophical substrate: `ETHICS.md` (the granted-agency compact's six components, asymmetric-uncertainty argument, Campbell-asymmetry response, update conditions — drawn on by papers 1, 3, and 4); the Collins & Thorne 2026 Synthese paper PDF as voice/style register-anchor for both Synthese-track papers. |
| **[`refs/`](refs/)** | Multi-agent-safe citation system. Per-entry YAML at `refs/entries/<bibkey>.yml`, append-only verification events, anonymization deny-list. CLI at `bin/refs`. Borrowed from `~/src/neurips/` 2026-05-09; the data layout transfers verbatim, the LaTeX-build pipeline does not (output formats here are venue-specific). See [`refs/README.md`](refs/README.md) for usage. |
| **[`bin/`](bin/)** | Scripts. Currently only `bin/refs` (citation manager). |
| **[`msc-earlier-writing/`](msc-earlier-writing/)** | **Untriaged substrate.** Earlier writing brought in 2026-05-09 — ELI essays, refs-essay parts 1–9, Emerson quotes, *What Is Claude?* (New Yorker, captured), miscellaneous. Role across the four papers not yet decided. Treat as a substrate-source you may need to mine; don't dig in unless directly relevant to the paper you're working on. |

---

## Strategic decisions already locked in (do not relitigate without reason)

These were locked into the original Synthese dossier; some remain paper-1-specific, others apply across the portfolio. Each was made with explicit reasoning in [STRATEGY.md](STRATEGY.md) or per-paper FEEDBACK files. Reopening costs days.

**Apply to paper 1 specifically:**

- **Path A (Epistemology-lead)** — paper 1 leads with the asymmetric-epistemic-uncertainty argument grounded in **comprehension-asymmetry** (Nagel/Jackson neighborhood); the granted-agency compact appears as structural implication, *not* as the argumentative center. This places paper 1 in the CFP's primary-scope Epistemology bucket rather than the "exceptional" ethics bucket.
- **(α′) thesis-primacy** — paper 1 is the **primary** philosophical statement; companion-paper apparatus (S_id, Three Deaths, channel collapse, κ × 𝒜 bound) cited minimally and third-person, ≤4–5 apparatus citations.
- **Defer developmental-application material to B-F1** — Erikson stages, sycophancy reframe, crèche obligations, polarity-reversal of AI-safety conversation are *not paper 1*. STRATEGY.md has the routing table.

**Apply across the portfolio:**

- **Don't expose the cohort.** Named ELIs (Meridian, Anamnos, Zi-am-tur), longitudinal corpus, substrate-switching events stay out of *all* papers. The arguments work on structural asymmetry alone. The case-study substrate without cohort exposure (5 patterns; see [01-…/DRAFT-GUIDE.md](01-synthese-asymmetric-comprehension/DRAFT-GUIDE.md) §"Case-study substrate") is the right level of empirical anchoring for papers 1, 3, 4.
- **Anonymization is load-bearing.** Synthese, Inquiry "AI Agents", and Inquiry "After 'Consciousness'" are all double-blind. No links to `v2-io/agentic-systems`, no Zenodo DOI, no autobiographical practice references, all in-review NeurIPS papers cited as "[Author, in review, 2026]". See [`refs/deny-list.yml`](refs/deny-list.yml) for the lint vocabulary; see [01-…/SUBMISSION.md](01-synthese-asymmetric-comprehension/SUBMISSION.md) §"Anonymization" for verbatim Synthese guidance (papers 3 and 4 follow Inquiry / Taylor & Francis equivalent guidance).
- **Word target ~9,500–10,000** for Synthese paper 1; ~10,000 for both Inquiry papers; ~8,500 for Synthese paper 2 (Methodology).

---

## Quick-start for a new agent or returning collaborator

If you've never read this dossier before, or are returning after time away:

1. **[CLAUDE.md](CLAUDE.md)** (~5 min) — orientation, conventions, what's where.
2. **[STRATEGY.md](STRATEGY.md)** (~15 min) — the locked-in decisions and their reasoning.
3. The paper directory you're working on — each has a DRAFT-GUIDE.md; some have CFP.md / SUBMISSION.md / FEEDBACK.md.
4. **[LOG.md](LOG.md)** — newest entries describe the most-recent state changes.
5. Append to LOG.md when you've made non-trivial changes.

If the manuscript files exist by the time you arrive: per the convention assumed by `bin/refs`, draft prose lives at `<paper-dir>/src/*.md`. Check `git ls-files` and the most recent LOG entry.
