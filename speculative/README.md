---
epistemic_status: speculative
last_reviewed: 2026-08-20
---

# Speculative work

## What belongs here

Science fiction, design fiction, scenarios, thought experiments, vision documents,
imaginative sketches of systems that do not exist and may never exist.

**This material is welcome and is part of the method.** Speculative and design fiction are
recognised techniques in human–computer interaction for generating hypotheses and for
surfacing assumptions that formal writing conceals. Writing a scenario about a person and
an AI system three years from now is a legitimate way to find out what you actually believe
about coupling.

## What it is not

**Nothing in this folder is evidence.** Not weak evidence, not suggestive evidence, not
"illustrative" evidence. A vivid scenario produces the *feeling* of having demonstrated
something while demonstrating nothing, and that feeling is the single most reliable way for
a research programme to become unfalsifiable without anyone deciding to make it so.

Every file here carries `epistemic_status: speculative`, without exception.

## The rule that makes this safe

From [`../docs/en/epistemic-status.md`](../docs/en/epistemic-status.md):

> **An `operational` document may never cite a `speculative` one as support.**

A conjecture *may* be inspired by something written here. When it is, say so in prose —
"this line of thinking originated in `speculative/foo.md`" — rather than citing it as a
reference. The difference between acknowledging where an idea came from and claiming
evidential backing for it is the whole distinction this repository is built to preserve.

## How to get value out of it

The productive loop is one-directional:

```
speculative  ──generates──▶  conjecture  ──operationalises──▶  operational  ──tests──▶  evidenced
```

Nothing flows backwards. A failed experiment is never explained by returning to the
scenario that inspired it and arguing the scenario was right in spirit.

If a piece of speculative work turns out to contain a testable claim, **extract the claim
into a ledger entry** with kill criteria attached. The story stays here; the hypothesis goes
to `ledger/`. That extraction is where the value is realised.

## Suggested convention

Name files by what they explore, not by genre — `delegation-spiral-2029.md`,
`what-if-memory-were-shared.md`. Add a one-line note at the top saying what question
prompted it. Six months later, that line is the only part you will still be able to use.
