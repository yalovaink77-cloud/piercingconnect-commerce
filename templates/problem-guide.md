# Template: Problem Guide

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for piercing problem troubleshooting guides. Safety language overrides affiliate placement.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Problem | `data/problems/{{problem.id}}.yaml` |
| Ingredient (1+) | From `problem.related_ingredients` |
| Healing Stage (1+) | From `problem.healing_stages` |
| Product (1+) | From `problem.related_products` |
| Piercing Type (1+) | From cluster or problem context cross-links |
| Keyword Cluster | `data/keywords/{{keyword_cluster.id}}.yaml` |

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

- `{{problem.name}}`
- `{{problem.summary}}`
- `{{ingredient.name}}`
- `{{healing_stage.name}}`
- `{{piercing_type.name}}`
- `{{product.name}}`
- `{{keyword_cluster.primary_keyword}}`
- `{{keyword_cluster.safety_notes}}`
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
- Apply all `{{keyword_cluster.safety_notes}}` before commercial sections

### 2. Problem Overview

- `{{problem.name}}`
- `{{problem.summary}}`
- `{{problem.description}}` — cautious framing

### 3. What It May Look Like

- `{{problem.symptoms}}` list from entity

### 4. Possible Causes

- `{{problem.possible_causes}}`
- Mechanical vs product vs jewelry factors

### 5. Affected Piercings and Stages

- `{{piercing_type.name}}` cross-links
- `{{healing_stage.name}}` from problem record

### 6. Recommended Actions

- `{{problem.recommended_actions}}`
- Professional referral language

### 7. Actions to Avoid

- `{{problem.actions_to_avoid}}`
- APP-not-recommended ingredients

### 8. Product and Ingredient Context

- `{{product.name}}` from related products
- `{{ingredient.name}}` — what may help vs what to avoid
- `{{affiliate_disclosure}}` only after safety sections

### 9. When to Seek Professional Help

- `{{problem.when_to_seek_professional_help}}`
- Piercer vs medical evaluation guidance

### 10. Risk Level Context

- `{{problem.risk_level}}` — editorial flag, not diagnosis

### 11. Safety Disclaimer

- `{{safety_disclaimer}}`
- Explicit non-diagnosis statement

### 12. CTA

- `{{cta}}` — minimal commercial pressure on urgent clusters

### 13. Sources and Review

- Problem and cluster sources
- `review.status`
