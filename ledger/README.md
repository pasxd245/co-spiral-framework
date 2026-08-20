---
epistemic_status: operational
last_reviewed: 2026-08-20
---

# Hypothesis ledger

## Purpose

The ledger is the programme's memory of what it claimed, when, and what happened. It exists
so that hypotheses cannot be quietly reshaped after results arrive — the most common way a
research programme becomes unfalsifiable without anyone deciding to make it so.

## Rules

1. **Append-only.** A ledger entry's history is never rewritten. Status changes are added
   as dated lines beneath the existing record. If a hypothesis is reformulated, the old
   formulation stays visible above the new one.
2. **Kill criteria are fixed in advance.** An entry without a kill criterion is not a
   hypothesis; it is a hope. Write the kill criterion before running anything.
3. **Kill criteria may not be revised after seeing results.** They may be revised *before*
   data collection, with the revision dated and the reason stated.
4. **One file per hypothesis**, named `H<n>-<slug>.md`.
5. **Refutation is recorded, not deleted.** A refuted hypothesis moves to
   `epistemic_status: retired` and states what killed it. It stays in the folder.

## Entry template

```markdown
---
epistemic_status: conjecture
last_reviewed: YYYY-MM-DD
---

# H<n> — <name>

## Claim
<One paragraph. Precise enough to be wrong.>

## Why it might be true
## Why it might be false
## Distinguishing prediction
<What this predicts that a rival account does not.>

## Kill criteria
<Fixed in advance. What observation retires this hypothesis?>

## Dependencies
<What must be true or in place for this to be testable at all.>

## Status history
- YYYY-MM-DD — created, `conjecture`.
```

## A note on preregistration

**This ledger is not a preregistration.** Git history can be rewritten, so a commit date is
not credible evidence to a reviewer that a hypothesis predated its results.

When a study is designed, register it externally with a service that provides an
independent timestamp (OSF, AsPredicted, or similar), and record the registration ID in the
relevant ledger entry. The ledger remains the working record; the external registration is
the evidence.

## Current entries

| Entry | Status | Blocking issue |
|---|---|---|
| [H1 — Coupling](./H1-coupling.md) | `conjecture` | No measure of coupling strength exists |
| [H2 — Cognitive-state transition](./H2-cognitive-transition.md) | `conjecture` | Novelty unestablished; literature review pending |
| [H3 — Intervention](./H3-intervention.md) | `conjecture` | Depends on H2; no domain chosen |
