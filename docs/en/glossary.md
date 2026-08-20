---
epistemic_status: operational
last_reviewed: 2026-08-20
---

# Glossary

Every named term used in this programme, with its current epistemic status. A term absent
from this file is not part of the programme.

**Reading rule:** `UNDEFINED` means exactly what it says. If a term below is marked
UNDEFINED, it may not be used as though it had a settled meaning — not in a study design,
not in a proposal, not in an argument.

**Governing constraint:** the programme's own falsification discipline
(`research-programme.md` §7) identifies construct inflation as a primary failure mode.
Therefore only **one** construct is targeted for operationalisation at Master's scope.
Everything else is parked in the backlog below and stays there.

---

## Active — targeted for operationalisation

### Human epistemic agency

> **Status:** `conjecture` — targeted for promotion to `operational`
> **Priority:** this is *the* construct. Everything else waits.

The degree to which a person retains the capacity to form, examine, and revise their own
beliefs and decisions during extended AI-assisted work — as opposed to accepting AI output
without independent warrant.

**Why this one.** It is the narrowest construct that still addresses the programme's core
question; it connects to an existing measurement literature (appropriate reliance, trust
calibration, cognitive offloading), which means instruments may already exist; and it is
the one whose loss would matter even if every other hypothesis here is wrong.

**Not yet specified:** measurement procedure, scale, failure condition, rival explanation.
Until those exist it remains a conjecture. See `epistemic-status.md` for the four criteria.

**Open problem.** Distinguishing *retained agency* from *appropriate delegation*. A person
who correctly defers to a reliable system is not thereby less agentic. Any measure that
scores deference as agency-loss is measuring the wrong thing, and this is the most likely
way a first attempt fails.

---

## Backlog — parked, do not build on

These terms are **not** available for use in study design, argument, or proposal text. They
are recorded because they may become useful, and because deleting them would hide the
programme's history. Each needs the full `operational` treatment before it can be activated,
and activating more than one would reintroduce exactly the construct inflation this
programme is trying to avoid.

### Telic Rung

> **Status:** `conjecture` — **UNDEFINED**, backlogged

Working construct for the degree of the human's cognitive investment and ownership of an
outcome. Provisionally sketched as a tuple:

$$R_H = \langle \text{Effort},\ \text{Ownership},\ \text{Agency},\ \text{Verification},\ \text{Commitment},\ \text{Revision} \rangle$$

**Problems to solve before activation:**

1. **It is not a truth score** and must never be read as one.
2. **It must not be compressed to a scalar** before construct validity is established.
   Six ill-defined dimensions averaged into one number produces a confident meaningless
   quantity.
3. **Circularity.** If CoSF defines both the intervention and the measure of its success,
   the result is unfalsifiable. Telic Rung must therefore be treated as a *hypothesis about
   what externally-validated instruments capture*, not as the measurement itself. This is
   the reason `instruments/` will be kept separate from `constructs/`.
4. It overlaps substantially with *Human epistemic agency* above. One of the two is
   probably redundant. Resolving that is cheaper than operationalising both.

**Note:** this term appeared four times in the previous version of this repository —
including as a mandatory item in the contributor checklist — while never being defined
anywhere. That is the failure mode this glossary exists to prevent.

### ΔU

> **Status:** `operational` *as a discipline*, not as a variable — backlogged as a construct

A **cognitive flag** / **non-closure marker**. It records that a conclusion reached within
some model $M_i$ and domain $D_j$ is not identical to the whole of what is the case.

**Binding constraints — these are the point of the term:**

- `ΔU` is **not a variable to be measured.**
- `ΔU` **does not explain failures.**
- `ΔU` **may not be used to rescue CoSF from a refutation.**

What *is* measured instead: error, surprise, contradiction, model disagreement, and belief
revision. If a discussion reaches for `ΔU` to account for a negative result, that discussion
has gone wrong.

### PCL

> **Status:** `conjecture` — **UNDEFINED**, backlogged

Provisional module. No operational definition, no metric, no scope, no failure condition.
Not part of the empirical core of any study. May not be invoked until all four exist.

### PCV

> **Status:** `conjecture` — **UNDEFINED**, backlogged

As PCL. Recorded, parked.

### Agent-Self

> **Status:** `conjecture` — experimental architecture, not yet built, **do not build yet**

A proposed experimental system with memory, goals, policies, tools, interaction history and
triggers, used to study persistent coupling.

**Explicitly not:** a source of truth, a subject with default personhood, or a product.

**Required comparisons if it is ever built:** stateless LLM, generic workflow, human-alone,
AI-alone — plus ablations isolating which mechanism produces any observed effect.

**Build warning.** The author is a full-stack developer; the temptation to implement this
before a study needs it is the largest single risk to the runway. Nothing here is built
until a designed study requires a specific capability. See `CLAUDE.md` §6.

---

## Structural terms

### HI × AI (coupling)

> **Status:** `conjecture` — see `ledger/H1-coupling.md`

Notation for a human–AI arrangement exhibiting persistent state, reciprocal adaptation,
feedback, goal influence, and causal interdependence.

**Important revision to the original formulation.** The `+` → `×` transition was originally
stated as binary. Every criterion listed for it is continuous, so the binary is not
supported by its own definition. **Coupling is therefore treated as a measured continuous
quantity**, and any threshold effect is a possible *finding*, not a premise. The `×`
survives as a name, not as a claim.

### Coupling conditions (L1 / L1.5 / L2 / L3)

> **Status:** `conjecture` — see `coupling-conditions.md`

The former "levels" ladder (Prompt Engineering → Manual RAG → RAG System → Fine-Tuning),
reframed as a set of experimental conditions that instantiate different degrees and kinds
of coupling. **No longer a skills or maturity ladder.**

### Co-Spiral intervention

> **Status:** `conjecture` — see `ledger/H3-intervention.md`

A pattern-triggered interruption of a human–AI workflow, intended to alter the trajectory
of the human's cognitive state. Requires a detectable trigger and a specified operator.

### TRIZ-inspired pattern

> **Status:** `conjecture`

TRIZ is used as a source of transformation operators, **not as a measurement theory**. Each
candidate pattern must carry:

$$\text{Pattern} = \langle \text{Context},\ \text{Tension},\ \text{Signals},\ \text{Trigger},\ \text{Operator},\ \text{Prediction},\ \text{Failure} \rangle$$

A pattern that cannot be detected, triggered, and falsified is not a pattern. It is a
metaphor.

---

## Terms deliberately not used

**"AI maturity level."** The author maintains a separate organisational AI-adoption
framework using the word *level*. The two are unrelated: that one measures organisational
adoption, this one concerns cognitive coupling in individuals. To prevent conflation, this
repository does not use "level" for its conditions — it uses **coupling conditions**.
