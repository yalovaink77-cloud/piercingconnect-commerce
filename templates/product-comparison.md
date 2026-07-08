# Template: Product Comparison

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for comparing two or more products. PCME generates prose from structured product and ingredient data — not commission rates.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Brand (2+) | `data/brands/` for each compared product |
| Product (2+) | `data/products/{{product_a.id}}.yaml`, `{{product_b.id}}.yaml`, … |
| Ingredient | Union of all compared product ingredient lists |
| Product Category | Shared or primary `data/product-categories/{{product_category.id}}.yaml` |
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

- `{{brand.name}}` (per product)
- `{{product.name}}` (per product)
- `{{product.trust.score}}` (per product)
- `{{ingredient.name}}`
- `{{product_category.name}}`
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
- `{{keyword_cluster.safety_notes}}`

### 2. Comparison Introduction

- User problem from `{{keyword_cluster.user_problem}}`
- Products being compared (names and brands only)

### 3. Quick Comparison Table

- Columns: product name, brand, category, sterile flag, trust score, key ingredients
- PCME populates from YAML — no invented specs

### 4. Ingredient Comparison

- Side-by-side: `{{ingredient.name}}`, APP alignment, evidence level per product

### 5. Formulation and Labeling

- Sterile, preservative-free, drug-free flags per product
- Category fit: `{{product_category.primary_use}}`

### 6. Healing Stage Suitability

- Overlap and differences in `healing_stages` arrays

### 7. Trust and Editorial Assessment

- Trust scores with explicit note that affiliate does not determine winner

### 8. Safety Notes

- `{{safety_disclaimer}}`
- Acknowledge equivalent simple saline options when formulations match

### 9. Best For / Not Ideal For

- Editorial segmentation from entity fields — not universal prescriptions

### 10. Affiliate Disclosure

- `{{affiliate_disclosure}}` for all products with affiliate availability

### 11. Summary and CTA

- Neutral comparison conclusion
- `{{cta}}`

### 12. Sources and Review

- Combined `sources` from compared entities
- `review.status` flags
