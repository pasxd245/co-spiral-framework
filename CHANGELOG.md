# Changelog

Stage markers, not semantic versions — see [`CONTRIBUTING.md`](./CONTRIBUTING.md).

## [0.1.0-stage0] — 2026-08-20

Restructured from a practitioner-framework repository into a research programme repository.

### Added

- `CLAUDE.md` — binding working agreement for AI sessions: research-collaborator role,
  epistemic discipline, hard constraints
- `docs/en/epistemic-status.md` — five-tier status vocabulary and the cite-downward rule
- `docs/en/glossary.md` — every construct with explicit status; undefined terms marked
  UNDEFINED and backlogged
- `docs/en/research-programme.md` — the programme, translated to English and cleaned
- `docs/en/coupling-conditions.md` — conditions C0–C4 replacing the old "levels" ladder
- `ledger/` — append-only hypothesis record (H1, H2, H3) with kill criteria fixed in advance
- `lit/` — literature workspace with note template and copyright rules
- `speculative/` — quarantined folder for fiction and design fiction
- `AI-USE.md` — detailed AI-use disclosure; explicit statement that AI is not an author
- `CITATION.cff` — citation metadata
- `.gitignore` — blocks copyrighted material, human-subjects data, and private working files

### Changed

- **H1 reformulated** from a binary `HI + AI` → `HI × AI` transition to a continuous
  coupling quantity. Every criterion in the original definition was continuous, so the
  binary was unsupported by its own terms. Any threshold is now a possible finding rather
  than a premise.
- **The "levels" ladder** (Prompt Engineering / Manual RAG / RAG System / Fine-Tuning Ethos)
  reframed from a practitioner skills ladder into experimental conditions instantiating
  degrees of coupling. The awkward "level 1.5" is resolved: it was two dimensions —
  automation of context, and human epistemic involvement — forced onto one axis.
- **`Telic Rung`, `ΔU`, `PCL`, `PCV`, `Agent-Self`** moved to an explicit backlog. One
  construct (*human epistemic agency*) is targeted for operationalisation; the rest may not
  be built upon.
- **Dual licence split** into `LICENSE-DOCS` (CC BY-SA 4.0) and `LICENSE-CODE` (MIT) so both
  are machine-detectable.
- **`CONTRIBUTING.md`** rewritten for a single-author programme. The previous version
  required contributors to satisfy a "Telic note" checklist item for a term that was never
  defined anywhere in the repository.
- **`README.md`** rewritten. The previous version documented six folders while shipping two,
  and linked to `ROADMAP.md` and an issue template that did not exist.

### Removed

- Joint human–AI maintainership attribution. Superseded by `AI-USE.md`: AI involvement is
  disclosed in detail, but AI is not an author, because authorship requires accountability.

### Notes

- Novelty of the primary hypothesis (H2) remains **unestablished**. The literature review
  is the next gate and can retire it cheaply.
- Domain `D_j` remains unchosen; this blocks study design.
- No human-subjects data exists and none may be collected before ethics approval.

---

## [1.0] — 2025-10-28 *(superseded)*

Initial release as a practitioner-oriented framework. Retained here as history; the
conceptual content is superseded by `0.1.0-stage0` above. The version numbering restarted
because the repository changed purpose.
