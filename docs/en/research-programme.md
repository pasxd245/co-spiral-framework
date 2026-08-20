---
epistemic_status: conjecture
last_reviewed: 2026-08-20
supersedes: CoSF_v1.1_draft.md
---

# CoSF / HI×AI — Research Programme

> **Epistemic status: conjecture.** This is a provisional, bounded research-and-design
> programme. It is **not** a completed theory of cognition, an ontology of reality, or a
> universal framework. Nothing in this document is supported by data collected under this
> programme, because no data has been collected.

**Scope:** human–AI interaction, cognition, agency, and co-adaptive systems.

---

## 1. Research motivation

AI does not merely automate tasks. In extended interactions with memory, feedback, and
adaptive capability, an AI system can act back upon how a person thinks, sets goals, makes
decisions, and understands themselves.

CoSF investigates one slice of this problem:

> When does the relationship `HI + AI` become a coupled adaptive system `HI × AI`; what
> cognitive states does this produce; and how might such a system be deliberately
> orchestrated so as to preserve human agency while creating value?

---

## 2. Core hypotheses

Each hypothesis has a tracked entry in [`../../ledger/`](../../ledger/) carrying its
predictions, kill criteria, and status history. The ledger is authoritative; this section
is the summary.

### H1 — Coupling hypothesis

Not every use of AI constitutes `HI × AI`.

```text
HI + AI
  ── persistent state + reciprocal adaptation
     + feedback + goal influence
     + causal interdependence ──▶  HI × AI
```

Complexity alone is not sufficient. The `×` is conjectured to apply when human and AI both
change over the interaction history, and the behaviour of the whole cannot be adequately
described as the sum of two independent components.

> **Revision (2026-08-20).** As originally written, H1 asserted a *binary* transition. But
> every criterion above — persistence, reciprocity, goal influence, interdependence — is
> continuous. A binary claim is therefore not supported by its own definition, and would be
> the first thing a reviewer attacks.
>
> **H1 is restated: coupling is a continuous quantity to be measured.** Whether there
> exists a threshold at which system behaviour qualitatively changes is a possible
> *finding*, not a starting assumption. `HI × AI` remains as a name for the high-coupling
> region, not as a claim about a phase transition.

### H2 — Cognitive-state transition hypothesis

The primary object of observation is not the AI's output but the transition in the human's
cognitive state:

$$K_t \xrightarrow[\;M_i,\,D_j\;]{\text{HI–AI interaction}} K_{t+1}$$

What must be examined across that transition:

- the conclusions formed and the confidence attached to them;
- the warrant or evidence actually used;
- the scope of explanation and the assumptions in play;
- the decisions, actions, and responsibility taken;
- the capacity to detect error and to self-correct.

**This is the most promising hypothesis in the programme** and the one most likely to be
publishable — and also the one most likely to already exist in the literature under other
names. The literature review is the gate.

### H3 — Co-Spiral intervention hypothesis

Within a defined domain `D_j`, pattern-triggered Co-Spiral interventions may produce a
better trade-off than a generic human–LLM workflow across:

$$J = \langle \text{Performance},\ \text{Calibration},\ \text{Agency},\ \text{Transfer},\ \text{Cost} \rangle$$

CoSF is **not** assumed to win on every dimension. The target is a Pareto improvement, or a
meaningful and empirically confirmed trade-off.

---

## 3. The human anchor

The human anchor is a **normative constraint** on the system, not an empirical claim:

- dignity and human agency;
- the right to reflect, to veto, and to change the goal;
- responsibility for decisions and their consequences;
- the human is not reduced to a data source, a reward signal, or a feedback provider.

`Telic Rung` was introduced as a working construct for the human's cognitive investment and
ownership. It is currently **backlogged and undefined** — see
[`glossary.md`](./glossary.md) for why, and for the circularity problem that must be solved
before it can be activated.

---

## 4. Research modules

All modules below are `conjecture`. None is built. See
[`glossary.md`](./glossary.md) for the constraints on each.

- **Agent-Self** — a proposed experimental architecture for studying persistent coupling.
  Not a source of truth, not a subject with default personhood. Requires comparison against
  stateless LLM, generic workflow, human-alone, and AI-alone, plus ablations. **Not to be
  built before a designed study requires it.**
- **ΔU** — a non-closure marker, not a variable. Never measured, never explanatory, never a
  rescue. What is measured instead: error, surprise, contradiction, model disagreement,
  belief revision.
- **PCL / PCV** — provisional, undefined, parked.
- **TRIZ-inspired pattern layer** — a source of transformation operators, not a measurement
  theory. Every candidate pattern must be detectable, triggerable, predictive, and
  falsifiable.

---

## 5. Initial research questions

1. By what indicators can a human's **retained epistemic agency** be measured?
2. What conditions distinguish `HI + AI` from `HI × AI` — and is that distinction
   continuous or discrete?
3. How do persistent memory and reciprocal adaptation affect cognition and decision-making?
4. Can delegation spirals, cognitive capture, or goal drift be detected early?
5. Do pattern-triggered interventions improve calibration, agency, and task performance
   relative to generic reflection prompts?

---

## 6. Minimal empirical design

Select one narrow domain `D_j`. Fix task, model, tools, time/token budget, and success
criteria. Compare:

$$\text{Human alone} \quad vs \quad \text{Human} + \text{LLM}_{\text{stateless}} \quad vs \quad \text{Human} + \text{AgentSelf} \quad vs \quad \text{Human} + \text{AgentSelf}_{\text{CoSF}}$$

Minimum requirements:

- preregistered hypotheses (externally timestamped — a git commit is not credible
  preregistration, since history can be rewritten);
- behavioural measures combined with self-report;
- simple, task-matched baselines;
- ablation study;
- independent or blind evaluation;
- a versioned hypothesis ledger;
- kill criteria fixed in advance.

> **Blocking gap: `D_j` has not been chosen.** No protocol can be written until it is.
>
> **Blocking constraint: no ethics approval exists.** No human-subjects data may be
> collected before enrolment (target December 2026). Data collected without approval cannot
> be retroactively authorised and is unusable. Pilot work before that date is limited to
> N=1 self-observation.

---

## 7. Falsification discipline

CoSF is weakened whenever:

- failures are absorbed by `ΔU`, by domain mismatch, or by "not enough spiral iterations";
- the same framework generates the intervention, defines the metric, **and** scores the
  result;
- a new concept is added after each refutation;
- the effect disappears against a generic checklist, or once time/token budget is
  controlled;
- the individual contribution of each module cannot be isolated.

A failed experiment refutes an intervention or module **under the conditions tested**. It
does not automatically refute the whole research vision. But the research vision may not be
used to indefinitely shield mechanisms that keep failing.

**Operationalised as repository rules** in [`../../CLAUDE.md`](../../CLAUDE.md) §5–6, so
that this section is structural rather than aspirational.

---

## 8. Master's → PhD trajectory

**Master's scope.** One construct, one narrow domain. Target: measuring *human epistemic
agency* and *appropriate reliance* in extended interaction with an LLM or agent system.

**PhD scope.** Expanded only if the construct and the initial effect survive empirical
test: modelling the coupling, cognitive-state transition, automatic pattern detection,
triggered intervention, and longitudinal study of HI×AI systems.

**Timeline.** Enrolment targeted December 2026. Between now and then the work is:
literature review → choose `D_j` → select externally-validated instruments → write protocol
and preregistration → N=1 pilot. No participants.

---

## 9. Epistemic status

CoSF is currently a conjectural research programme with a genealogy in practical
observation, cognition, philosophy, TRIZ, and human–AI practice. It is not arbitrary. It
may nonetheless be wrong, redundant, unoriginal, or unmeasurable.

**Its novelty is unestablished.** Appropriate reliance, trust calibration, cognitive
offloading, distributed cognition, and human–AI complementarity are populated research
areas. Until the literature review is complete, any claim of originality here is a
placeholder.

> The research value of CoSF comes not from the number of concepts it retains, but from the
> distinguishing predictions it makes, the interventions whose mechanisms are specified, and
> the tests by which each module could fail.

---

*A Vietnamese version of this document can be produced on request. English is canonical;
preregistrations and protocols remain English-only to avoid version skew.*
