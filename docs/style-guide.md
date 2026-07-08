# Style Guide

Version: 1.0

Status: Active

Project: PiercingConnect Commercial Knowledge Core

---

## Purpose

Consistent voice and formatting across books, generated content, and structured record summaries.

---

## Voice

- Educational, calm, and precise
- Second person ("you") for aftercare instructions
- No hype, fear-mongering, or sensational medical language
- No diagnosis — use cautious framing per `standards/evidence-policy.md`

---

## Medical and Safety Language

**Use:**

- "may be a sign of"
- "could be related to"
- "consider contacting a qualified piercer or healthcare provider"
- "APP guidance recommends…"

**Avoid:**

- "This is infected"
- "Guaranteed healing in X days"
- "Miracle", "cure", "treatment" for consumer products
- Absolute claims about allergy or infection without professional evaluation

---

## Product and Affiliate Language

- Lead with ingredients, sterility, and trust scores — not commission
- Disclose affiliate relationships clearly
- Never imply a product treats or cures a medical condition
- Distinguish sterile isotonic saline from sea-salt marketing formulations

---

## Formatting

### Markdown (books and templates)

- Title as H1, then Version / Status metadata block
- Use `---` horizontal rules between major sections
- Tables for indexes and comparisons
- Code-style paths for file references: `` `data/brands/neilmed.yaml` ``

### YAML (data layer)

- Two-space indentation
- Block scalars (`>`) for multi-line text
- Stable kebab-case IDs
- Required `review` block on every entity

---

## Terminology

Use approved terms from `standards/terminology.md`. Prefer "sterile saline" over vague "cleaning solution."

---

## SEO Content

- Match search intent without keyword stuffing
- No invented search volume or CPC
- Safety sections precede commercial CTAs on problem-intent content

See `standards/seo-guidelines.md`.

---

## Capitalization

- Brand names as published (NeilMed, H2Ocean)
- Piercing type names lowercase in IDs, title case in prose (Helix, Nostril)
- APP — Association of Professional Piercers (spell out once per document)
