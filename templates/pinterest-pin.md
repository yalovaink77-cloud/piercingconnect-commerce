# Template: Pinterest Pin

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for Pinterest pin copy and board metadata. Short-form — PCME generates concise text from entity fields.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Keyword Cluster | `data/keywords/{{keyword_cluster.id}}.yaml` |
| Focal entity (one required) | Problem **or** Piercing Type **or** Product **or** Product Category |

---

## Publishing Targets

- Pinterest

---

## Template Variables

- `{{keyword_cluster.primary_keyword}}`
- `{{problem.name}}`
- `{{piercing_type.name}}`
- `{{product.name}}`
- `{{product_category.name}}`
- `{{pin_title}}`
- `{{pin_description}}`
- `{{board_name}}`
- `{{destination_url}}`
- `{{hashtags}}`
- `{{safety_disclaimer}}`
- `{{affiliate_disclosure}}`
- `{{cta}}`

---

## Sections

### 1. Pin Metadata

- `{{pin_title}}` — from keyword cluster + focal entity name
- `{{pin_description}}` — 2–3 sentence cap; PCME from entity summary
- `{{keyword_cluster.primary_keyword}}`
- `{{destination_url}}` to full article template output

### 2. Hook Line

- Single attention line from `{{keyword_cluster.user_problem}}`

### 3. Value Bullet Points

- 3–5 bullets from entity field lists (aftercare notes, recommended actions, product criteria)
- No medical diagnosis language

### 4. Safety Micro-Disclaimer

- `{{safety_disclaimer}}` — abbreviated for pin format
- Required for problem-intent clusters

### 5. Visual Direction Notes

- Image concept for designer / AI image step (not generated prose article)
- Entity type and mood keywords only

### 6. Board and Hashtags

- `{{board_name}}`
- `{{hashtags}}` from cluster and entity IDs

### 7. Affiliate Note (Conditional)

- `{{affiliate_disclosure}}` when product focal entity

### 8. CTA

- `{{cta}}` — link to long-form template output

### 9. Sources and Review

- Focal entity and cluster IDs
- `review.status`
