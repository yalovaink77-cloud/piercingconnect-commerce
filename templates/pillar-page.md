# Template: Pillar Page

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for SEO pillar / hub pages that link to spoke content across the knowledge graph.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Keyword Cluster | `data/keywords/{{keyword_cluster.id}}.yaml` |
| Product Category (1+) | Hub category records |
| Problem (1+) | Spoke problem records |
| Piercing Type (1+) | Spoke aftercare records |
| Healing Stage (1+) | Foundational healing context |
| Product (optional) | Featured products |
| Brand (optional) | Featured brands |

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

- `{{keyword_cluster.primary_keyword}}`
- `{{product_category.name}}`
- `{{problem.name}}`
- `{{piercing_type.name}}`
- `{{healing_stage.name}}`
- `{{product.name}}`
- `{{brand.name}}`
- `{{meta_title}}`
- `{{meta_description}}`
- `{{safety_disclaimer}}`
- `{{affiliate_disclosure}}`
- `{{review_status_note}}`
- `{{cta}}`

---

## Sections

### 1. Meta and SEO Block

- `{{meta_title}}` — pillar keyword
- `{{meta_description}}`
- Internal linking map metadata for PCME

### 2. Pillar Introduction

- `{{keyword_cluster.summary}}`
- `{{keyword_cluster.user_problem}}`
- Topic scope and who this hub serves

### 3. Foundational Concepts

- `{{healing_stage.name}}` overview sequence
- Core terminology from standards layer reference

### 4. Category Hub Section

- For each `{{product_category.name}}`: summary, primary use, link to category page template output

### 5. Aftercare Hub Section

- For each `{{piercing_type.name}}`: summary, link to aftercare guide output

### 6. Problem Hub Section

- For each `{{problem.name}}`: summary, risk level, link to problem guide output

### 7. Product and Brand Highlights (Optional)

- Featured `{{product.name}}` and `{{brand.name}}` with trust context

### 8. Comparison and Buying Paths

- Links to buying guide and comparison template outputs
- `{{keyword_cluster.recommended_content_types}}`

### 9. Safety and Evidence Framework

- `{{safety_disclaimer}}`
- Evidence policy summary pointer
- `{{keyword_cluster.safety_notes}}`

### 10. Affiliate Disclosure

- `{{affiliate_disclosure}}` — hub pages with product mentions

### 11. Spoke Content Index

- Structured list of child content asset IDs / URLs for PCME site architecture

### 12. CTA

- `{{cta}}`

### 13. Sources and Review

- Aggregated entity sources
- `review.status` across hub entities
