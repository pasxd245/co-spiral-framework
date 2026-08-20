---
epistemic_status: operational
last_reviewed: 2026-08-20
---

# Literature

## Status: not started. This is the programme's blocking gate.

Until the review is done, the novelty of H2 — the primary hypothesis — is **assumed, not
established**. It is the cheapest possible test of the whole programme and it should be run
before any other work.

## What lives here

| Path | Contents | Committed? |
|---|---|---|
| `references.bib` | BibTeX metadata | **yes** |
| `notes/<citekey>.md` | Your own summary and critique, in your words | **yes** |
| `review.md` | The synthesis: what exists, where the gap is | **yes** (once written) |
| PDFs, EPUBs, scans | — | **never** |

## The copyright rule

**No copyrighted source files in this repository. Ever.** `.gitignore` blocks `*.pdf`,
`*.epub`, and similar, and those rules are not to be given exceptions.

What is safe to commit: bibliographic metadata (facts, not copyrightable), and your own
summaries and critiques written in your own words. Extended verbatim quotation is not a
summary.

Keep the PDFs in a reference manager outside the repo.

## Recommended workflow

Zotero with the Better BibTeX plugin, auto-exporting to `lit/references.bib`. Hand-managed
citations do not survive a five-year programme. Set this up before the reading starts, not
after fifty papers have accumulated.

## Note-taking convention

One file per source, named by citekey. Front-matter carries the verification state:

```markdown
---
epistemic_status: evidenced
last_reviewed: YYYY-MM-DD
citekey: author2024title
read: full | partial | abstract-only
ai_summarised: true | false
verified_against_source: true | false
---

# <Short title>

## Claim
## Method
## What it measures, and how
## Relevance to CoSF
## Objection / limitation
## Does this pre-empt H2?
```

That last heading is not optional. Every source gets asked the question directly, because
the answer is what the review is for.

**`ai_summarised: true` with `verified_against_source: false` means the note is a lead, not
a finding.** It may not be cited in any document until verified. AI-generated reference
lists are checked against primary sources without exception — a fabricated or misattributed
citation is the most damaging error available in academic work.

## Scope of the review

Areas that plausibly already contain H2, and must be checked before novelty is claimed:

- appropriate reliance / over-reliance on AI advice
- trust calibration in human–automation interaction
- cognitive offloading and its effects on retention and understanding
- distributed cognition and the extended mind
- human–AI complementarity and joint cognitive systems
- explanation, confidence, and their effect on user verification behaviour
- cognitive forcing functions and interventions against over-reliance

The review's job is to answer one question: **is there a distinguishing prediction left
for H2 to make?** If not, the programme reformulates or retires the hypothesis. That is a
success of the method, not a failure of the project.
