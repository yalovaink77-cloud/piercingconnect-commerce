# Template: Buying Guide

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for commercial buying guides by product category. Trust and safety precede affiliate recommendations.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Product Category | `data/product-categories/{{product_category.id}}.yaml` |
| Product (2+) | From `product_category.related_products` |
| Brand (1+) | From product `brand` fields |
| Ingredient (1+) | From `product_category.related_ingredients` |
| Keyword Cluster | `data/keywords/{{keyword_cluster.id}}.yaml` |

---

## Publishing Targets

- WordPress
- Facebook
- Pinterest
- Email
- PDF

---

## Template Variables

- `{{product_category.name}}`
- `{{product_category.primary_use}}`
- `{{product.name}}`
- `{{brand.name}}`
- `{{ingredient.name}}`
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

- `{{meta_title}}` from `{{keyword_cluster.primary_keyword}}`
- `{{meta_description}}`
- `{{product_category.safety_notes}}`

### 2. Category Introduction

- `{{product_category.name}}`
- `{{product_category.summary}}`
- `{{keyword_cluster.user_problem}}`

### 3. What This Category Is For

- `{{product_category.primary_use}}`
- `{{product_category.category_type}}`

### 4. How to Evaluate Products

- Criteria from category safety notes and ingredient APP alignment
- Sterility, formulation simplicity, trust scores

### 5. Featured Products

- For each product: `{{product.name}}`, `{{brand.name}}`, trust score, key ingredients

### 6. Ingredient Checklist

- `{{ingredient.name}}` and what to look for or avoid in this category

### 7. Healing Stage Fit

- `{{product_category.suitable_healing_stages}}`
- Editorial suitability flags

### 8. Common Problems This Category Addresses

- `{{problem.name}}` from `product_category.related_problems`

### 9. What to Avoid

- Category safety notes
- Products or formulations not aligned with APP guidance

### 10. Affiliate Disclosure

- `{{affiliate_disclosure}}`
- Note: affiliate potential field does not determine ranking

### 11. Summary and CTA

- `{{cta}}`
- `{{safety_disclaimer}}`

### 12. Sources and Review

- Category, product, cluster sources
- `review.status`
