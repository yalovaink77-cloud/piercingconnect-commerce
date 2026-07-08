# Template: Aftercare Guide

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for piercing-type aftercare guides. PCME generates prose from piercing type, body location, and healing context.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Piercing Type | `data/piercing-types/{{piercing_type.id}}.yaml` |
| Body Location | `data/body-locations/{{body_location.id}}.yaml` |
| Healing Stage (1+) | From `piercing_type.healing_stages` |
| Keyword Cluster | `data/keywords/{{keyword_cluster.id}}.yaml` |
| Product (optional) | From `piercing_type.recommended_products` |
| Ingredient (optional) | From recommended product ingredients |
| Material (optional) | From `piercing_type.suitable_materials` |
| Jewelry Type (optional) | From `piercing_type.suitable_jewelry` |

---

## Publishing Targets

- WordPress
- Facebook
- Pinterest
- Email
- YouTube
- PDF

---

## Template Variables

- `{{piercing_type.name}}`
- `{{piercing_type.aftercare_notes}}`
- `{{body_location.name}}`
- `{{healing_stage.name}}`
- `{{healing_stage.summary}}`
- `{{material.name}}`
- `{{jewelry_type.name}}`
- `{{product.name}}`
- `{{keyword_cluster.primary_keyword}}`
- `{{meta_title}}`
- `{{meta_description}}`
- `{{safety_disclaimer}}`
- `{{affiliate_disclosure}}`
- `{{review_status_note}}`
- `{{cta}}`

---

## Sections

### 1. Meta and SEO Block

- `{{meta_title}}` from `{{keyword_cluster.primary_keyword}}`
- `{{meta_description}}`
- `{{keyword_cluster.safety_notes}}`

### 2. Guide Introduction

- `{{piercing_type.name}}` overview from `summary`
- `{{keyword_cluster.user_problem}}`

### 3. Anatomy and Placement Context

- `{{body_location.name}}` and anatomy notes
- `{{piercing_type.anatomy}}`

### 4. Healing Timeline Overview

- `{{healing_stage.name}}` progression
- `{{piercing_type.healing_time}}` — cautious language, no guarantees

### 5. Daily Aftercare Routine

- `{{piercing_type.aftercare_notes}}`
- APP-aligned steps from entity fields

### 6. Jewelry and Materials During Healing

- `{{material.name}}` from suitable materials
- `{{jewelry_type.name}}` from suitable jewelry
- Downsizing notes from `piercing_type.downsizing`

### 7. Normal vs Concerning Signs

- Normal signs from healing stage records
- Caution signs — refer to problem records, no diagnosis

### 8. Common Problems

- `{{problem.name}}` from `piercing_type.common_problems`
- Link IDs only — detail in problem-guide template

### 9. Recommended Products (Optional)

- `{{product.name}}` from recommended products
- `{{affiliate_disclosure}}` when products linked

### 10. What to Avoid

- Ingredients and practices with `app_alignment: not-recommended`

### 11. When to See Your Piercer

- `{{piercing_type.when_to_seek_help}}`

### 12. Safety Disclaimer and CTA

- `{{safety_disclaimer}}`
- `{{cta}}`

### 13. Sources and Review

- Piercing type, body location, cluster sources
- `review.status`
