# Template: Facebook Post

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for Facebook feed posts. Short-form educational or commercial — PCME generates from entity fields.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Keyword Cluster | `data/keywords/{{keyword_cluster.id}}.yaml` |
| Focal entity (one required) | Product **or** Brand **or** Problem **or** Piercing Type |

---

## Publishing Targets

- Facebook

---

## Template Variables

- `{{keyword_cluster.primary_keyword}}`
- `{{product.name}}`
- `{{brand.name}}`
- `{{problem.name}}`
- `{{piercing_type.name}}`
- `{{post_hook}}`
- `{{post_body}}`
- `{{link_url}}`
- `{{safety_disclaimer}}`
- `{{affiliate_disclosure}}`
- `{{cta}}`

---

## Sections

### 1. Post Metadata

- Post type: educational | commercial | problem-alert
- Focal entity ID and type
- `{{keyword_cluster.search_intent}}`
- `{{keyword_cluster.priority}}`

### 2. Hook

- `{{post_hook}}` — first line from user problem or entity summary

### 3. Body Structure

- 2–4 short paragraphs mapped to entity fields
- Bulleted tips from aftercare notes or recommended actions when applicable

### 4. Safety Block (Conditional)

- Required for problem focal entity
- `{{keyword_cluster.safety_notes}}`
- `{{safety_disclaimer}}`

### 5. Link and CTA

- `{{link_url}}` to WordPress template output
- `{{cta}}`

### 6. Affiliate Disclosure (Conditional)

- `{{affiliate_disclosure}}` for product or brand posts

### 7. Engagement Prompt

- Question derived from `{{keyword_cluster.user_problem}}` — PCME generates one question only

### 8. Sources and Review

- Entity IDs used
- `review.status`
