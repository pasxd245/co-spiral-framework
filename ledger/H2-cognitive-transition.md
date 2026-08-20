---
epistemic_status: conjecture
last_reviewed: 2026-08-20
---

# H2 — Cognitive-state transition hypothesis

> **This is the programme's primary hypothesis.** It is the narrowest claim that still
> addresses the core question, and the one most likely to yield a defensible Master's
> thesis. It is also the one most likely to already exist in the literature.

## Claim

In extended AI-assisted work, the theoretically important object is not the AI's output but
the transition in the human's cognitive state:

$$K_t \xrightarrow[\;M_i,\,D_j\;]{\text{HI–AI interaction}} K_{t+1}$$

Specifically: extended interaction with an adaptive AI system systematically changes the
*warrant structure* of the human's beliefs — the confidence they hold, the evidence they
can cite for it, and their capacity to detect their own error — independently of whether
task performance improves.

## Why this framing matters

The independence clause is the substance. If AI assistance improved performance *and*
degraded the human's independent warrant for their conclusions, conventional
performance-based evaluation would report an unambiguous success while something important
was being lost. H2 says that is measurable and worth measuring.

## Why it might be true

- Performance and understanding are known to dissociate in other tool-use contexts.
- Confidence is easy to transfer between agents; warrant is not.
- The effect has a plausible mechanism: fluent, confident output reduces the felt need to
  independently verify.

## Why it might be false

- **It may be well-established already.** Appropriate reliance, over-reliance on AI
  advice, trust calibration, and cognitive offloading are active research areas. If H2 is a
  rediscovery, the contribution is zero.
- Measured self-report of confidence is notoriously unreliable and may swamp the effect.
- The effect may be entirely explained by *time on task* — less time thinking, therefore
  less warrant — which would make it uninteresting.

## Distinguishing prediction

> Participants in higher-coupling conditions will show **increased confidence with
> unchanged or reduced independent warrant**, and reduced ability to detect deliberately
> introduced errors in AI output — *even when task performance is equal or better*.

The rival account ("AI just helps") predicts confidence and warrant move together.

**Error-detection is the key measure**, because it can be tested behaviourally rather than
by self-report: introduce known errors and observe whether they are caught.

## Kill criteria

Fixed in advance. H2 is retired if:

1. The literature review establishes that this effect is already documented, with adequate
   measures, and no distinguishing prediction remains; **or**
2. Confidence and warrant move together across all conditions; **or**
3. Any observed effect disappears when time-on-task is controlled; **or**
4. Error-detection rates show no condition difference at adequate statistical power.

Criterion 1 is live *now* and is the cheapest possible test. It should be run first.

## Dependencies

- **Literature review.** Blocking. This is the immediate next action for the programme.
- **Externally validated instruments** for confidence, reliance, and calibration — these
  must not be authored by this programme. See `docs/en/glossary.md` on circularity.
- A chosen domain `D_j`. **Not chosen.**
- Ethics approval. **Not available before Dec 2026.**
- Power analysis. A study that cannot detect the effect it hypothesises is not evidence of
  absence, and underpowered first studies are the most common way a promising question dies.

## Open problem

**Distinguishing agency loss from appropriate delegation.** A person who correctly defers
to a reliable system is not thereby less agentic. Any measure that scores correct deference
as agency loss is measuring the wrong construct. This is the most likely way a first
attempt at operationalisation fails, and it should be solved on paper before any data is
collected.

## Status history

- **2026-08-20** — created, `conjecture`. Designated primary hypothesis.
