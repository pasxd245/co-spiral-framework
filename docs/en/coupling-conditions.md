---
epistemic_status: conjecture
last_reviewed: 2026-08-20
supersedes: "the CoSF 'levels' ladder (Prompt Engineering / Manual RAG / RAG System / Fine-Tuning Ethos)"
---

# Coupling conditions

## What changed and why

An earlier version of this project presented a four-rung ladder — Prompt Engineering →
Manual RAG → RAG System → Fine-Tuning Ethos — as a **skills ladder** for practitioners.

That framing is discarded. Two reasons:

1. **It measures the wrong thing.** As a skills ladder it describes practitioner
   competence, which has nothing to do with this programme's research question.
2. **It is not one dimension.** Manual RAG has *lower* automation than a RAG system but
   *higher* human epistemic involvement. Those move in opposite directions, so they cannot
   be points on a single line. The awkward "level 1.5" was a symptom of forcing two
   dimensions onto one axis.

The same material is retained here in a form that earns its place: as a set of
**experimental conditions that instantiate different degrees and kinds of coupling.** This
gives H1 a manipulation variable instead of leaving it purely theoretical.

> **This document does not prove anything.** An implementation is an existence proof of
> feasibility, not evidence of an effect. These conditions are a *means of manipulating*
> the independent variable; the outcome measures must come from elsewhere — see
> [`glossary.md`](./glossary.md) on circularity.

---

## The conditions

| Condition | Persistent context | Who performs retrieval | AI adapts to human | Human adapts to AI |
|---|---|---|---|---|
| **C0 — Human alone** | — | — | no | no |
| **C1 — Prompt only** | no | — | no | weakly |
| **C2 — Manual RAG** | yes | **human** | no | yes |
| **C3 — Automated RAG** | yes | **machine** | no | yes |
| **C4 — Adapted model** | yes | machine | **yes** | yes |

Reciprocal adaptation — the property H1 identifies as central — first appears at **C4**, and
only there. C2 and C3 have persistence but the adaptation runs one way.

This yields a directly testable prediction: **if H1 is right that reciprocity is what makes
coupling qualitatively different, then C4 should differ from C3 in a way that C3 does not
differ from C2.** If the C2→C3→C4 progression is smooth on every measure, the reciprocity
claim is in trouble.

---

## The two-dimensional structure

The conditions vary along two axes that the old ladder conflated:

```
                        human epistemic involvement
                        high                 low
                   ┌──────────────────┬──────────────────┐
      automation   │   C2             │   C1             │
      of context   │   Manual RAG     │   Prompt-only    │
      low          │                  │                  │
                   ├──────────────────┼──────────────────┤
      automation   │   ???            │   C3 / C4        │
      of context   │                  │   Automated RAG  │
      high         │   (empty cell)   │   / Adapted      │
                   └──────────────────┴──────────────────┘
```

**The empty cell is the interesting one.** High automation *with* high human epistemic
involvement is where a Co-Spiral intervention would have to live if H3 is to mean anything.
If that cell is genuinely unreachable — if automation necessarily costs epistemic
involvement — then H3 is false and the programme should say so.

This gives the research question a sharper form than the original ladder allowed:

> **Are automation of context and human epistemic involvement necessarily coupled, or can
> they be dissociated by design?**

That question is falsifiable, it does not depend on any CoSF-specific construct, and it
would be worth answering even if every other hypothesis in this programme fails.

---

## Design cautions

- **Confounds.** Moving up the conditions changes several things at once: token budget,
  latency, output quality, and human effort. Without matching on time and token budget, any
  observed effect may be an effect of *effort*, not of coupling. `research-programme.md` §7
  names this explicitly.
- **Ablation is mandatory.** If C4 differs from C3, the design must be able to say whether
  the cause was reciprocal adaptation, or simply better output quality.
- **C2 is the sleeper condition.** Manual RAG is the only condition where the human does
  the epistemic work of selecting context. It may turn out to be the best condition on
  agency measures while being the worst on performance and cost — which would be a genuinely
  useful result and directly relevant to practice.

---

## Build discipline

**None of these conditions should be built as engineering work yet.**

C1–C3 can be approximated cheaply for a study; C4 (an adapted or fine-tuned model) is
expensive and is not required for a first experiment. Building the full stack before a
protocol exists would consume the entire pre-enrolment runway and produce no research.

Build order, if and when a protocol requires it: C1, C2, C3, then C4 — and only as far as
the protocol actually needs.
