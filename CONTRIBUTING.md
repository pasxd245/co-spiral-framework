---
epistemic_status: operational
last_reviewed: 2026-08-20
---

# Contributing

## Current status: single-author programme, not open to contributions

This is one researcher's PhD-track research programme. It is public for transparency,
provenance, and citability — not because it is seeking collaborators. There is no review
capacity, so pull requests will not be merged.

**Corrections and objections are welcome and valuable.** Open an issue. In particular:

- a citation showing that a hypothesis here has already been tested;
- a methodological flaw in a proposed design;
- a construct that is doing no work and should be retired.

An issue that retires a hypothesis is the most useful contribution possible to this
repository.

## If you are reusing this material

Documentation is CC BY-SA 4.0; code is MIT. Cite via [`CITATION.cff`](./CITATION.cff).

Please carry the epistemic status with the material. Quoting a `conjecture` as though it
were `evidenced` misrepresents the work — and every document here states its status in the
front-matter precisely so that mistake is avoidable.

---

## Working rules for the author and for AI sessions

These are binding on all work in this repository. The full version is in
[`CLAUDE.md`](./CLAUDE.md).

### Before committing anything

- [ ] Document carries `epistemic_status` and `last_reviewed` front-matter
- [ ] No `operational` document cites a `speculative` one as support
- [ ] No new construct promoted to `operational` without measurement procedure, scale,
      failure condition, and a named rival explanation
- [ ] Backlogged constructs (`Telic Rung`, `ΔU`, `PCL`, `PCV`, `Agent-Self`) not built upon
- [ ] Every citation verified against the primary source — no unverified AI recall
- [ ] No copyrighted PDFs, EPUBs, or scans
- [ ] No human-subjects data of any kind
- [ ] Ledger entries appended, never rewritten
- [ ] No folder created without content in it
- [ ] English canonical; Vietnamese only if explicitly requested

### Hypothesis changes

A hypothesis may be reformulated at any time **before** data collection, with the
reformulation dated and the previous version retained in the ledger. After data collection
begins, the preregistered form governs.

Kill criteria may never be revised after seeing results.

## Versioning

Semantic versioning does not fit a research programme. This repository uses stage markers:

- `0.x-stage0` — scaffolding; no literature review
- `0.x-stage1` — literature review complete; constructs and instruments defined
- `0.x-stage2` — protocol written and externally preregistered
- `1.0` — first study completed and reported, whatever the result

A negative result still ships as `1.0`. That is the point.
