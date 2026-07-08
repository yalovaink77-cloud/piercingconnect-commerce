# Editorial Guidelines

Version: 1.0

Status: Active

Project: PiercingConnect Commercial Knowledge Core

---

## Purpose

Editorial standards for human-written and PCME-generated content derived from this repository.

---

## Source of Truth

- `data/` YAML records are canonical for facts
- `books/` explain and contextualize — they must not contradict data
- `research/` is unvalidated until promoted to data
- Published articles are outputs, never imported back as truth

---

## Workflow Compliance

Follow `docs/workflow.md`:

Research → Validation → Schema → Data → Book Content → Templates → PCME → Publishing → Review

No entity should be marked `active` without standards review.

---

## Evidence Requirements

- Safety claims require evidence per `standards/evidence-policy.md`
- Official and professional sources before marketplace or community opinion
- Manufacturer claims verified independently where possible
- Gaps marked as unknown — do not fill with assumptions

---

## Problem and Medical Content

- Never diagnose infection, allergy, or other conditions
- Distinguish irritation from infection concern without false reassurance
- Include when to seek piercer or medical help on moderate+ risk topics
- Symptom records describe observations — not diagnoses

---

## Commercial Content

- Follow `standards/affiliate-policy.md`
- Product reviews must cite trust scores and ingredients from data layer
- Comparisons must be fair and evidence-based
- Buying guides lead with selection criteria, not brand deals

---

## Review States

| Status | Meaning |
|--------|---------|
| draft | Initial entry, not publish-ready |
| needs_review | Flagged for update |
| reviewed | Editorially checked |
| active | Approved for PCME publishing |
| outdated | Source or product changed |
| deprecated | Retired, kept for ID stability |

---

## Sync Rule

When updating a product or problem in `data/`, review the matching book chapter and any linked keyword clusters.

---

## Related Documents

- `docs/style-guide.md`
- `docs/ai-developer-guide.md`
- `standards/terminology.md`
