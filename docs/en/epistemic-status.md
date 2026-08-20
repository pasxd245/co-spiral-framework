---
epistemic_status: operational
last_reviewed: 2026-08-20
---

# Epistemic status: the labelling system

## Why this exists

This programme deliberately keeps material of very different evidential weight in one
repository: imaginative and speculative writing, unproven conjectures, operational
definitions, and (eventually) empirical results.

That mixture is productive — speculative work is a recognised way of generating hypotheses
— but it is also the most common way a research programme quietly becomes unfalsifiable. A
vivid imagined scenario *feels* like evidence. Six months later nobody remembers which
document was fiction.

The labelling system makes the weight of every document explicit and machine-checkable, so
that mixing is safe.

## The five statuses

Every substantive Markdown file in this repository carries YAML front-matter:

```yaml
---
epistemic_status: conjecture
last_reviewed: 2026-08-20
---
```

### `speculative`

Fiction, vision, design fiction, thought experiment, imagination. Explicitly makes **no
claims about the world**.

Speculative material is welcome and is kept in `speculative/`. Its purpose is to generate
candidate hypotheses and to surface assumptions that formal writing hides. It is never
evidence.

### `conjecture`

A stated hypothesis. Clear enough to argue with, not yet operationalised — no measurement
procedure, no failure condition, or both.

Most of this repository is currently at this level. That is expected at Stage 0 and is not
a problem, so long as it is not disguised.

### `operational`

Defined and measurable. To qualify, a document must specify:

1. a **measurement procedure** — what is observed, how, under what conditions;
2. a **scale or unit** — including whether it is ordinal, interval, or categorical;
3. a **failure condition** — what observation would show the construct does not apply;
4. a **rival explanation** the measurement is designed to rule out.

A construct missing any of the four is a `conjecture` with ambitions.

### `evidenced`

Supported by data, with the study that produced it named, and the strength and limits of
that support stated. An `evidenced` claim states its scope: which domain, which population,
which task, which model.

### `retired`

Refuted, superseded, or abandoned.

**Retired documents are kept, never deleted.** A research programme's discarded branches
are part of its record and are frequently the most informative thing in it. A retired
document states, at the top, *what killed it*.

## The cite-downward rule

Documents may cite **downward only**, along this ordering:

```
evidenced  >  operational  >  conjecture  >  speculative
```

Concretely:

| A document at this level | may cite | may NOT cite |
|---|---|---|
| `evidenced` | `evidenced`, `operational` | `conjecture`, `speculative` |
| `operational` | `evidenced`, `operational`, `conjecture` | `speculative` |
| `conjecture` | anything, as *inspiration*, stated in prose | speculative material as *support* |
| `speculative` | anything | — |
| `retired` | anything, as history | — (and may not be cited as support) |

The one that matters: **an `operational` document may never cite a `speculative` one as
support.** A story can suggest a hypothesis; it can never justify one.

When a conjecture is inspired by speculative work, say so in prose — "this line of thinking
originated in `speculative/foo.md`" — rather than citing it as a reference. The distinction
is between acknowledging a source of ideas and claiming evidential backing.

## Promotion and demotion

Status changes are **events**, and they are recorded in the hypothesis ledger
(`ledger/`), not made silently.

- **Promotion** requires meeting the criteria above and updating `last_reviewed`.
- **Demotion to `retired`** requires stating what killed it.
- **A document may not be promoted by its own author's confidence.** Promotion from
  `conjecture` to `operational` is a claim that the four criteria are met, and it should be
  checkable by someone else.

## Staleness

`last_reviewed` is not decoration. A document at `operational` status that has not been
reviewed in twelve months should be treated as `conjecture` until re-checked.
