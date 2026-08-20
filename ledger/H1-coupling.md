---
epistemic_status: conjecture
last_reviewed: 2026-08-20
---

# H1 — Coupling hypothesis

## Claim

**As revised (2026-08-20):** A human–AI working arrangement can be characterised by a
*continuous* degree of coupling, determined by persistent state, reciprocal adaptation,
feedback, goal influence, and causal interdependence. Higher coupling produces system
behaviour that is progressively less well described as the sum of two independent
components.

**Original formulation (superseded, retained for the record):** There is a *transition*
from `HI + AI` to `HI × AI` when the above criteria are met.

## Why it was revised

Every criterion listed is continuous. A binary transition is therefore not supported by the
hypothesis's own definition — the criteria cannot pick out a boundary they do not contain.
Asserting a phase change without a mechanism for one would be the first thing a reviewer
attacks, and defending it would consume effort better spent elsewhere.

Whether a threshold exists is now an **empirical question**, not an assumption. If a
genuine discontinuity is found, that is a much stronger result than assuming one.

## Why it might be true

- Long-running interactions with memory plausibly produce mutual adaptation that
  short exchanges do not.
- Existing theory in distributed and extended cognition treats human + artefact systems as
  legitimate units of analysis, which at least makes the framing respectable.
- The `C4` condition (see `docs/en/coupling-conditions.md`) introduces a mechanism —
  AI adapting to the human — absent in all lower conditions, giving a concrete place for
  any discontinuity to appear.

## Why it might be false

- **Coupling may be unmeasurable in practice.** Without an operational measure, this
  hypothesis is untestable and everything downstream is blocked.
- **The distinction may make no behavioural difference.** High coupling could be real and
  yet predict nothing about outcomes, in which case it is a description, not a finding.
- **It may already exist** in the literature on distributed cognition, joint cognitive
  systems, or human–automation teaming, in more developed form.
- **Effort confound.** Higher conditions demand more human effort and more tokens. Any
  observed difference may be an effort effect wearing a coupling costume.

## Distinguishing prediction

If reciprocal adaptation is what makes coupling qualitatively different, then:

> The difference between C4 (AI adapts to human) and C3 (no AI adaptation) should be
> *larger in kind*, not merely in degree, than the difference between C3 and C2.

A rival "it's just more automation / more effort / better output" account predicts a smooth
monotonic progression across C1→C4 with no special status for C4.

## Kill criteria

Fixed in advance. H1 is retired if:

1. No measure of coupling strength can be defined that is distinguishable from a simple
   measure of interaction volume or token count; **or**
2. Measured coupling shows no relationship to any outcome in `J` once time and token budget
   are controlled; **or**
3. The C1→C4 progression is smooth on every measure, with C4 showing no distinctive
   signature.

## Dependencies

- An operational measure of coupling strength. **Does not currently exist.** This is the
  blocking issue.
- A chosen domain `D_j`. **Not chosen.**
- Ethics approval for any human-subjects test. **Not available before Dec 2026.**

## Status history

- **2026-08-20** — created, `conjecture`.
- **2026-08-20** — reformulated from binary transition to continuous quantity; original
  formulation retained above.
