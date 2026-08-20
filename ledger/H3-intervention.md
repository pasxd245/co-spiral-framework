---
epistemic_status: conjecture
last_reviewed: 2026-08-20
---

# H3 — Co-Spiral intervention hypothesis

> **Depends on H2.** If H2 is refuted there is nothing for an intervention to intervene on.
> Do not invest in H3 before H2 clears the literature review.

## Claim

Within a defined domain `D_j`, **pattern-triggered** interventions in a human–AI workflow
produce a better trade-off than a generic human–LLM workflow across:

$$J = \langle \text{Performance},\ \text{Calibration},\ \text{Agency},\ \text{Transfer},\ \text{Cost} \rangle$$

CoSF is **not** claimed to win on every dimension. The target is a Pareto improvement, or a
meaningful and empirically confirmed trade-off.

## The word that carries the weight

**Pattern-triggered.** An intervention that fires on a schedule, or at every step, is a
generic reflection prompt — and generic reflection prompts are a well-studied baseline that
this hypothesis must beat. The claim only has content if:

1. a detectable **signal** identifies when intervention is warranted; and
2. the **targeted** intervention outperforms the same intervention applied
   indiscriminately.

Without both, H3 reduces to "interrupting people sometimes helps," which is neither novel
nor CoSF-specific.

## Why it might be true

- Timing effects are real in related domains: an intervention at the moment of a decision
  plausibly differs from one delivered before or after.
- If H2 holds, there should be observable precursors to warrant-erosion, and precursors are
  what triggers detect.

## Why it might be false

- **The signal may not exist.** If erosion has no detectable precursor, there is nothing to
  trigger on.
- **Generic beats targeted.** Entirely possible, and would be a clean refutation.
- **Cost dominates.** Interventions consume time and attention. If the same time spent
  simply thinking produces the same benefit, the mechanism is irrelevant.
- **Self-scoring circularity.** If CoSF supplies the intervention *and* the success metric,
  the result is unfalsifiable. This is the single largest threat to H3's credibility, and it
  is structural, not incidental.

## Distinguishing prediction

> Pattern-triggered intervention will outperform time-matched, frequency-matched **generic**
> reflection prompts on calibration and error-detection.

The matching is essential. An unmatched comparison measures only "more prompts."

## Kill criteria

Fixed in advance. H3 is retired if:

1. No detectable trigger signal can be defined; **or**
2. Targeted intervention does not beat frequency-matched generic intervention; **or**
3. Any advantage disappears once time and token budget are controlled; **or**
4. Ablation cannot isolate which component produced the effect; **or**
5. H2 is retired.

## Dependencies

- **H2 must survive first.**
- A pattern library where each entry carries the full structure
  $\langle$Context, Tension, Signals, Trigger, Operator, Prediction, Failure$\rangle$.
  **Does not exist.**
- **Outcome measures authored outside this programme.** Non-negotiable — this is what
  answers the circularity objection.
- A chosen domain `D_j`. **Not chosen.**
- Independent or blind evaluation of outcomes.

## Note on the pattern layer

TRIZ supplies transformation operators. It does **not** supply a measurement theory, and
using it as one would be a category error. A pattern that cannot be detected, triggered,
and falsified is a metaphor, not a research object.

## Status history

- **2026-08-20** — created, `conjecture`. Marked dependent on H2.
