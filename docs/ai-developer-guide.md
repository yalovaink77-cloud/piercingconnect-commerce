# AI Developer Guide

Version: 1.0

Status: Active

Project: PiercingConnect Commercial Knowledge Core

---

## Purpose

This document is the permanent guide for AI assistants (Composer, agents, and similar tools) working in this repository.

Read this file before making any changes.

---

## Repository Purpose

This repository is the **PiercingConnect Commercial Knowledge Core**.

It is **not a blog**.

It is the **source of truth** for structured piercing commerce knowledge — brands, products, aftercare guidance, affiliate intelligence, and publishing assets that feed PiercingConnect's educational and commercial ecosystem.

Published articles, social posts, videos, and marketplace listings are **downstream outputs**. Content is generated from this repository; the repository is never reconstructed from published content.

---

## Layer Responsibilities

| Layer | Path | Responsibility |
|-------|------|----------------|
| Docs | `docs/` | Project architecture, vision, taxonomy, workflow, and operating rules |
| Standards | `standards/` | Editorial, ethical, medical, SEO, affiliate, and terminology policies |
| Schemas | `schemas/` | Machine-readable definitions for structured data entities |
| Data | `data/` | Source-of-truth structured records (YAML) consumed by automation and PC Media Engine |
| Books | `books/` | Human-readable commercial knowledge — guides, bibles, and editorial content |
| Research | `research/` | Raw research notes; unvalidated findings that must not be treated as final truth |
| References | `references/` | Source materials, citations, and supporting documentation |
| Templates | `templates/` | Reusable content structures for articles, guides, pins, scripts, and comparisons |
| Scripts | `scripts/` | Automation tools for validation, export, and ingestion |
| Exports | `exports/` | Generated outputs (PDF, CSV, JSON, publishing packages) — not source of truth |

For full architectural detail, see [architecture.md](architecture.md).

---

## Core Rules

All AI work in this repository must follow these rules:

1. **Follow [vision.md](vision.md)** — Safety first. Trust before revenue. Scientific integrity.
2. **Follow [architecture.md](architecture.md)** — Respect the human vs. machine knowledge split. Store knowledge once, reuse many times.
3. **Follow [taxonomy.md](taxonomy.md)** — Use approved categories, entity types, and naming conventions.
4. **Follow [standards/evidence-policy.md](../standards/evidence-policy.md)** — Prioritize official and professional sources. Safety claims require evidence.
5. **Do not make unsafe medical claims** — Never diagnose, prescribe, or guarantee outcomes. Use cautious language for high-risk topics.
6. **Do not let affiliate opportunity override safety** — Commercial value must never influence medical or safety recommendations.
7. **Keep structured data and book content synchronized** — If `data/` and `books/` disagree, review and reconcile both together.

---

## Data Rules

Structured data lives in `data/` and must conform to schemas in `schemas/`.

### Schema compliance

- All brand records must follow [schemas/brand.schema.yaml](../schemas/brand.schema.yaml).
- All product records must follow [schemas/product.schema.yaml](../schemas/product.schema.yaml).
- Other entity types must follow their corresponding schema files when present.

### YAML conventions

- Use the existing YAML style in the repository (see `data/brands/h2ocean.yaml` and `data/products/` for examples).
- Use two-space indentation.
- Use block scalars (`>`) for multi-line descriptions.
- Reference related entities by stable ID (e.g., `products: [h2ocean-piercing-aftercare-spray]`).

### Required review fields

Every entity record must include a `review` block:

```yaml
review:
  status: draft          # draft | in_review | approved | needs_update
  last_reviewed: 2026-07-08
```

### Identifiers

- Use **stable IDs** — lowercase, kebab-case, never change once assigned (e.g., `neilmed`, `h2ocean-piercing-aftercare-spray`).
- Use **kebab-case slugs** for URL-safe identifiers matching the ID unless a documented exception exists.
- Do not rename IDs without explicit instruction; downstream systems depend on them.

---

## Research Rules

Research belongs in `research/`, not in `data/` or `books/` until validated.

1. **Use official sources first** — Brand websites, manufacturer documentation, recognized medical and public health sources, professional association guidance.
2. **Treat marketplaces and communities as secondary** — Amazon listings, Reddit threads, and forum posts may inform context but are not primary evidence.
3. **Do not treat affiliate pages as primary evidence** — Affiliate program descriptions and marketplace copy must never be the sole basis for safety or product claims.
4. **Mark missing information clearly** — If a field cannot be verified, leave it empty or note it as unknown in research notes. Do not fill gaps with assumptions.

Research files should include status, entity type, date started, source URLs, and a clear separation between verified facts and unverified claims.

See [standards/evidence-policy.md](../standards/evidence-policy.md) for the full evidence priority order.

---

## Book Rules

The `books/` layer is **human-readable**. The `data/` layer is the **source of structured truth**.

| Layer | Audience | Format | Role |
|-------|----------|--------|------|
| `data/` | Software, automation, PC Media Engine | YAML | Canonical structured records |
| `books/` | Humans, editors, strategists | Markdown | Explanations, strategy, editorial context |

Rules:

- Book files must **summarize and explain** structured data — not contradict it.
- When updating a brand or product, update both `data/` and the relevant book section.
- Book content may include editorial strategy, comparison opportunities, and narrative context that does not belong in YAML.
- If structured data changes, book content must be reviewed for consistency.

Example pairing:

- Machine-readable: `data/brands/neilmed.yaml`
- Human-readable: `books/01-aftercare-bible/04-brand-database.md`

---

## Workflow

Follow this sequence for all new knowledge assets:

```
Research → Validation → Schema → Data → Book Content → Templates → PCME → Publishing → Review
```

| Step | Action |
|------|--------|
| Research | Gather sources in `research/` |
| Validation | Verify claims against evidence policy; reject unverified affiliate copy |
| Schema | Confirm the entity type and required fields in `schemas/` |
| Data | Create or update structured YAML in `data/` |
| Book Content | Update relevant Markdown in `books/` to match |
| Templates | Apply or create templates in `templates/` if needed |
| PCME | Package for PC Media Engine ingestion |
| Publishing | Generate downstream content (WordPress, Pinterest, etc.) |
| Review | Set `review.status` and `review.last_reviewed`; flag `needs_update` when sources change |

See [workflow.md](workflow.md) for the full definition of done and update rules.

Knowledge is never final. Re-review when products, science, affiliate programs, or regulations change.

---

## AI Restrictions

AI assistants must **never**:

| Restriction | Reason |
|-------------|--------|
| Invent certifications | Fabricated credentials destroy trust and may create legal liability |
| Invent affiliate programs | Only document programs verified from official sources |
| Invent product ingredients | Ingredient lists must come from manufacturer documentation |
| Diagnose medical conditions | PiercingConnect educates; it does not practice medicine |
| Recommend unsafe aftercare | No alcohol, hydrogen peroxide, harsh antiseptics, or unverified home remedies as primary aftercare |
| Overwrite unrelated files | Make minimal, focused changes scoped to the task at hand |

When information is unavailable, state that it is **unknown** or **unverified** rather than generating plausible-sounding content.

High-risk topics (infection, allergic reaction, rejection, severe pain, oral/genital complications, pregnancy, minors) require extra caution, evidence support, and referral to qualified professionals where appropriate.

---

## Commit Rule

Use clear, descriptive commit messages that state what was added or changed and why.

**Good examples:**

```
Add Base Laboratories knowledge
Add NeilMed product records and research
Update H2Ocean brand trust score after review
Fix aftercare bible sync with neilmed.yaml
```

**Avoid:**

```
update
fix stuff
changes
```

One logical change per commit when possible. Do not commit secrets, credentials, or `.env` files.

---

## Quick Reference for AI Assistants

Before starting work:

1. Read this guide.
2. Read [vision.md](vision.md), [architecture.md](architecture.md), and [taxonomy.md](taxonomy.md).
3. Check [standards/evidence-policy.md](../standards/evidence-policy.md) for anything involving safety or product claims.
4. Inspect existing files in the target layer for style and conventions.
5. Follow the workflow: Research → Validation → Schema → Data → Book Content → Templates → PCME → Publishing → Review.

When in doubt, prioritize **safety**, **evidence**, and **consistency** over speed or commercial opportunity.
