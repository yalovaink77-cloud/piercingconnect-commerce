# Template: FAQ

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for FAQ pages. Each Q&A block maps to knowledge entity fields — PCME generates answers from structured data.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Keyword Cluster | `data/keywords/{{keyword_cluster.id}}.yaml` |
| Topical entity (one required) | Problem **or** Piercing Type **or** Product Category |
| Product (optional) | When answers reference specific products |
| Healing Stage (optional) | When timing questions apply |
| Ingredient (optional) | When formulation questions apply |

---

## Publishing Targets

- WordPress
- Facebook
- Pinterest
- Email
- PDF

---

## Template Variables

- `{{keyword_cluster.primary_keyword}}`
- `{{problem.summary}}`
- `{{piercing_type.name}}`
- `{{product_category.name}}`
- `{{product.name}}`
- `{{healing_stage.name}}`
- `{{ingredient.name}}`
- `{{meta_title}}`
- `{{meta_description}}`
- `{{safety_disclaimer}}`
- `{{affiliate_disclosure}}`
- `{{review_status_note}}`
- `{{cta}}`

---

## Sections

### 1. Meta and SEO Block

- `{{meta_title}}`
- `{{meta_description}}`
- FAQ schema hints for PCME structured data export

### 2. FAQ Introduction

- `{{keyword_cluster.user_problem}}`
- Scope statement — what this FAQ covers

### 3. Question Blocks (repeat per FAQ item)

Each block structure:

- **Question heading** — derived from cluster or entity field
- **Answer section** — populated from entity summaries, lists, safety notes
- **Entity source ID** — for traceability in PCME output metadata

Suggested question categories (PCME selects based on loaded entities):

- Overview / definition
- Normal healing vs concern
- Aftercare routine
- Product suitability
- Timing and jewelry changes
- When to seek help

### 4. Safety-Critical Questions

- Pulled from `{{keyword_cluster.safety_notes}}`
- `{{problem.when_to_seek_professional_help}}` when problem entity loaded

### 5. Product Questions (Optional)

- `{{product.name}}` answers with trust and ingredient context
- `{{affiliate_disclosure}}`

### 6. Related Topics

- Cross-link IDs to problem guides, aftercare guides, buying guides

### 7. Safety Disclaimer

- `{{safety_disclaimer}}`

### 8. CTA

- `{{cta}}`

### 9. Sources and Review

- Entity sources used in FAQ generation
- `review.status`
