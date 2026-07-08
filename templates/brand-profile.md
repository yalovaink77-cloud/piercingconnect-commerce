# Template: Brand Profile

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for a brand overview page. PCME generates prose from brand and linked product records.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Brand | `data/brands/{{brand.id}}.yaml` |
| Product (1+) | `data/products/` where `brand == {{brand.id}}` |
| Product Category (1+) | `data/product-categories/` from product `category` fields |
| Keyword Cluster | `data/keywords/{{keyword_cluster.id}}.yaml` |

---

## Publishing Targets

- WordPress
- Facebook
- Email
- PDF

---

## Template Variables

- `{{brand.name}}`
- `{{brand.id}}`
- `{{keyword_cluster.primary_keyword}}`
- `{{meta_title}}`
- `{{meta_description}}`
- `{{affiliate_disclosure}}`
- `{{safety_disclaimer}}`
- `{{review_status_note}}`
- `{{cta}}`

---

## Sections

### 1. Meta and SEO Block

- `{{meta_title}}` from `{{keyword_cluster.primary_keyword}}` + `{{brand.name}}`
- `{{meta_description}}` from brand summary fields
- `{{review_status_note}}`

### 2. Brand Overview

- `{{brand.name}}`
- Brand positioning fields from `data/brands/{{brand.id}}.yaml`
- Trust and reputation fields

### 3. Product Line Summary

- For each linked product: `{{product.name}}`, category, trust score
- Map to `{{product_category.name}}` per product

### 4. Category Context

- `{{product_category.name}}` and `{{product_category.primary_use}}` for each category represented

### 5. Professional and Safety Context

- APP alignment notes from linked ingredients where applicable
- `{{safety_disclaimer}}`

### 6. Who This Brand Is For

- Piercing types and problems served via product cross-links
- Editorial suitability — not medical claims

### 7. Affiliate and Commercial Notes

- `{{affiliate_disclosure}}`
- Affiliate availability per product (separate from trust evaluation)

### 8. Related Products and Alternatives

- Linked product IDs and alternative brand references from knowledge graph

### 9. Call to Action

- `{{cta}}` aligned with `{{keyword_cluster.search_intent}}`

### 10. Sources and Review

- Entity `sources` slugs from brand and products
- `review.status` from required entities
