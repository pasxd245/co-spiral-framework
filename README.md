# Co-Spiral Framework (CoSF)

**A bounded research programme on human–AI cognitive coupling.**

> **Epistemic status: conjecture.** This is a provisional research-and-design programme, not
> a completed theory, not an ontology, and not a universal framework. No data has been
> collected. Its novelty is unestablished pending a literature review. Read
> [`docs/en/epistemic-status.md`](./docs/en/epistemic-status.md) before reading anything
> else here.

---

## The question

AI does not merely automate tasks. In extended interactions with memory, feedback, and
adaptive capability, an AI system can act back on how a person thinks, sets goals, decides,
and understands themselves.

This programme investigates one slice of that:

> When does a human–AI working relationship become a **coupled adaptive system**; what
> cognitive-state transitions does it produce in the human; and can such a system be
> designed so as to preserve human epistemic agency?

The primary hypothesis is **H2**: extended AI-assisted work changes the *warrant structure*
of a person's beliefs — their confidence, the evidence they can cite for it, and their
ability to catch their own errors — independently of whether task performance improves.

---

## What is here

| Path | Contents |
|---|---|
| [`docs/en/research-programme.md`](./docs/en/research-programme.md) | The programme: motivation, hypotheses, empirical design, falsification discipline |
| [`docs/en/epistemic-status.md`](./docs/en/epistemic-status.md) | The labelling system and the cite-downward rule |
| [`docs/en/glossary.md`](./docs/en/glossary.md) | Every construct, with status. Undefined terms are marked UNDEFINED |
| [`docs/en/coupling-conditions.md`](./docs/en/coupling-conditions.md) | Experimental conditions C0–C4, and the 2×2 that replaced the old "levels" ladder |
| [`ledger/`](./ledger/) | Append-only hypothesis record: claims, predictions, kill criteria |
| [`lit/`](./lit/) | Literature workspace. **Not started — this is the blocking gate** |
| [`speculative/`](./speculative/) | Fiction and design fiction. Quarantined. Never evidence |
| [`CLAUDE.md`](./CLAUDE.md) | Working agreement for AI sessions in this repo |
| [`AI-USE.md`](./AI-USE.md) | Disclosure of how AI was used in producing this work |

Folders are created when they have content, never in advance. `constructs/` and
`instruments/` open once the literature review survives; `studies/` once a protocol exists.

---

## How this repository is disciplined

The programme's own stated failure modes are construct inflation and unfalsifiability. Four
mechanisms make the discipline structural rather than aspirational:

1. **Epistemic status on every document.** `speculative` / `conjecture` / `operational` /
   `evidenced` / `retired`.
2. **The cite-downward rule.** An `operational` document may never cite a `speculative` one
   as support. Imagination can suggest a hypothesis; it can never justify one.
3. **Kill criteria fixed in advance,** recorded in an append-only ledger, never revised
   after seeing results.
4. **Outcome measures authored elsewhere.** A framework that supplies both the intervention
   and the metric cannot be refuted. Instruments will be borrowed from validated
   literature, kept separate from this programme's own constructs.

One construct — *human epistemic agency* — is targeted for operationalisation. Everything
else (`Telic Rung`, `ΔU`, `PCL`, `PCV`, `Agent-Self`) is backlogged in the glossary and may
not be built on.

---

## Current state

- **Stage 0.** Scaffolding complete. Literature review not started.
- **Domain `D_j`: not chosen.** This blocks all study design.
- **No human-subjects data exists, and none may be collected.** There is no ethics approval
  and none is available before enrolment (targeted December 2026). Pre-enrolment work is
  limited to N=1 self-observation.
- **Next action:** literature review. It is the cheapest possible test of the programme, and
  it can retire the primary hypothesis before anything expensive is built.

---

## Language

English is canonical. Vietnamese versions are produced on request. Preregistrations and
protocols remain English-only to avoid version skew between two records of the same
hypothesis.

---

## Licence

- **Documentation and written content:** [CC BY-SA 4.0](./LICENSE-DOCS)
- **Code, scripts, configuration:** [MIT](./LICENSE-CODE)

Referenced works are cited; no copyrighted source files are redistributed here.

---

## Author

Maintained by a single human author. **AI systems are not authors of this work** —
authorship requires accountability for the claims made. AI involvement is substantial and is
disclosed in detail in [`AI-USE.md`](./AI-USE.md).

Citation metadata: [`CITATION.cff`](./CITATION.cff).
