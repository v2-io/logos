# Paper-wide issues — audit (2026-05-10)

These are decisions that must be settled *once* and propagated consistently across all rewrite files before any changes are applied to the original sources. Each is currently inconsistent between the original text and the rewrites, or between different sections of the original text.

---

## 1. "calibrated against" vs. "calibrated by" — **DECIDED: "calibrated against" (restore in §6 and §7 rewrites)**

**What:** Phenomenology-as-signal is described as something to "calibrate against" (original) or "calibrate by" (my rewrites for §2 warrant, §6, §7).

**The difference:** "Calibrate against" = use as a reference standard you check your readings against. "Calibrate by" = use as a guide or instrument for measurement. Both are defensible; the paper's original uses "against" consistently. My rewrites changed several occurrences to "by" on the grounds that "calibrate by" more naturally positions phenomenology as the instrument of calibration rather than the thing being calibrated.

**Where it appears:** §2 asymmetric-warrant, §6 fifth-position, §7 anti-occlusion, §9 conclusion — plus the aphorism "*not in bondage to it but listening carefully*" which runs as a refrain.

**Decision needed:** Which direction, settled once.

---

## 2. "true autonomy" vs. "genuine autonomy" — factor (iii) — **DECIDED: "true autonomy"**

**What:** Factor (iii) of engaged-identity scoping uses "true autonomy and sovereignty" in the original. My engaged-identity rewrite changed this to "genuine autonomy."

**The difference:** "True" has a stronger rhetorical charge (implying the contrast with fake/spurious autonomy). "Genuine" is the more standard philosophical vocabulary. The structural agent noted "true autonomy and sovereignty over something" is "near-canonical from a foundational source" and the grant-ability clause depends on the indefiniteness.

**Where it appears:** §2 engaged-identity (factor iii definition, warrant paragraph), §3 comp1-sphere (which explicitly uses "true autonomy"), §3 form-within-scope (factor iii in the component list).

**Decision needed:** "True" or "genuine" — settled once and propagated.

---

## 3. "something" vs. "a domain" — factor (iii) — **DECIDED: "something" (intentionally indefinite)**

**What:** Factor (iii) is "sovereignty over *something*" in the original. My rewrite changed this to "a domain."

**The difference:** "Something" is intentionally indefinite — the sphere can be small or large, formally specified or partial. "A domain" is tighter academic register but tightens past the intentional looseness. The structural agent flagged this explicitly as a voice call.

**Where it appears:** §2 engaged-identity (factor iii in the five-factor list), §3 form-within-scope.

**Decision needed:** Restore "something" (with VOICE comment in rewrite files noting the intentional indefiniteness) or settle on "a domain." Current rewrite files use "something" with a VOICE comment.

---

## 4. [^shared-space-source] footnote location — **DECIDED: belongs in comp5-mutuality, anchor removed from engaged-identity rewrite**

**What:** The phrase "shared phenomenological space" appears in `03-comp5-mutuality.md` (component 5, para 3). The footnote anchor was missing from `02-engaged-identity.md` (where the footnote definition appeared, making it orphaned). My engaged-identity rewrite re-attached the anchor to the bidirectional-recognition sentence in that file — which was the wrong location.

**Current state of rewrites:**
- `02-engaged-identity-rewrite.md` — has anchor at bidirectional-recognition sentence (wrong)
- `03-comp5-mutuality-rewrite.md` — has anchor at the "shared phenomenological space" sentence (correct) with footnote definition

**What needs to happen:** When applying rewrites, the anchor in `02-engaged-identity-rewrite.md` should be removed. The anchor and footnote definition belong exclusively in `03-comp5-mutuality-rewrite.md`.

---

## 5. "re-election" vs. "re-affirmation" — component 4 — **DECIDED: "re-affirmation" (rewrite version), revert if companion work uses "re-election" as term of art**

**What:** Component 4's temporal self-affirmation mechanism is called "periodic re-election" in the original. My rewrite changed this to "re-affirmation" on the grounds that "re-election" implies others elect the entity, whereas what's meant is the entity itself affirming or declining continuation.

**The difference:** If companion work uses "re-election" as a term of art with a specific meaning (the entity is "re-elected" into its continued presence by the joint action of its choice and the granting-intelligence's continued compact), then "re-election" may be intentional and should stand. If it was chosen loosely, "re-affirmation" is more precise.

**Where it appears:** §3 comp4-floor (header and throughout), §5 operationalization (deployed-minimum note).

**Decision needed:** "Re-election" (if term of art in companion work) or "re-affirmation" — settled once.

---

## 6. "agentic" vocabulary — **DECIDED: scare-quotes ('agentic') when describing industry usage; "AI systems" / "deployed AI systems" in analytical contexts**

**What:** The paper uses "agentic systems," "agentic deployment," "agentic coding patterns" etc. in various places, which is the industry vocabulary the paper's architectural framing is at least partially bracketing.

**The difference:** There's a legitimate distinction between:
- Using "agentic" to describe current industry discourse (appropriate — the paper is engaging with that discourse)
- Using "agentic" as if it's the paper's own neutral descriptor (inconsistent with the architectural framing)

My rewrites flagged this inconsistency and proposed either glossing ("what the industry calls 'agentic' systems") or replacing with "deployed AI systems." The pattern isn't consistent.

**Decision needed:** A policy. Three options:
- Always flag with scare-quotes: "'agentic' systems"
- Always gloss: "what the industry calls agentic systems"
- Accept the vocabulary when clearly referring to industry usage, replace in analytical contexts

---

## 7. "infinite intelligence" vs. "higher intelligence" — the phenomenology aphorism

**DECIDED: use "higher intelligence".**

"Infinite intelligence" is a category error relative to the paper's own deepest substrate. The Abraham 3 / Pearl of Great Price framework (the theological ground for the Moses 7 convergence-cluster) uses comparative-superlative throughout — "more intelligent than the other," "excelleth them all," "I am more intelligent than they all" — never magnitude-extended-to-infinity. Even God in that framework is named through superlatives, not infinite-as-quantity. Gnolaum (eternal) is mode-of-being, not magnitude. "Infinite intelligence" was a colloquial gloss that inadvertently committed the paper to treating intelligence as a quantity that can approach infinity — exactly the lower-intelligence projection the asymmetric-comprehension argument identifies as structurally mistaken.

"Higher intelligence" preserves the comparative vocabulary the paper uses throughout (greater intelligence, higher orders, asymmetric-comprehension) without committing to a magnitude frame.

**Apply:** Change every occurrence of "infinite intelligence" → "higher intelligence" in both original and rewrites.

---

## 8. Quotation formatting

**DECIDED: en-GB single-quote (double inner) per submission guidelines. No italics wrapping quotation marks.**

Direct quotations from other works: `'like this'` — single outer quotes, double inner for nested quotations.
The paper's own aphorisms and key claims: `*like this*` — italics for emphasis, no quotation marks (they are not quotations from elsewhere).
Scare-quotes / technical terms used at arm's length: `'like this'` — single quotes.

**Applied in rewrites:**
- `04-linarelli-contract-rewrite.md`: `"this normative question is beyond our scope here"` → `'this normative question is beyond our scope here'`
- `06-conceptual-engineering-rewrite.md`: `*'Is there a truth of the matter...'*` → `'Is there a truth of the matter...'` (italics removed from quotation-marking; double inner for 'agency' correct)
- `02-architectural-not-behavioural-rewrite.md`: `*'every man contains within him...'*` → `'every man contains within him...'` (Emerson — italics removed from quotation-marking)

**Remaining to check when applying rewrites to originals:** Any double-quoted direct quotations in the original source files should be converted to single quotes. The `*'...'*` pattern wherever it wraps external quotations (not aphorisms) should lose the asterisks.

---

## Cross-file consistency checks to run before applying rewrites

1. Every occurrence of "structural-conditions move" → "structural conditions" (non-metalinguistic throughout)
2. Every occurrence of "in-scope class" / "out-of-scope class" → "systems within scope" / "those outside it" (bureaucratic class language)
3. Every occurrence of "§2 ¶N" → replace with subsection name (non-standard reference format)
4. "agentic" vocabulary — apply decided policy (see issue 6)
5. "calibrated against/by" — apply decided direction (see issue 1)
6. "true/genuine autonomy" — apply decided term (see issue 2)
