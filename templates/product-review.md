# Template: Product Review

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for an individual product review. PCME generates prose from product, brand, ingredient, and safety context.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Brand | `data/brands/{{brand.id}}.yaml` |
| Product | `data/products/{{product.id}}.yaml` |
| Ingredient (1+) | `data/ingredients/` from `product.ingredients` |
| Problem (1+) | From product / ingredient / cluster cross-links |
| Healing Stage (1+) | From `product.healing_stages` |
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

- `{{brand.name}}`
- `{{product.name}}`
- `{{product.trust.score}}`
- `{{ingredient.name}}`
- `{{ingredient.app_alignment}}`
- `{{problem.summary}}`
- `{{healing_stage.name}}`
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

- `{{meta_title}}` from `{{keyword_cluster.primary_keyword}}` + `{{product.name}}`
- `{{meta_description}}`
- `{{keyword_cluster.safety_notes}}`

### 2. Product Summary

- `{{product.name}}`
- `{{brand.name}}`
- Product category ID → `{{product_category.name}}`

### 3. Ingredients Breakdown

- For each ingredient: `{{ingredient.name}}`, type, APP alignment, risks

### 4. Intended Use and Healing Stages

- `{{healing_stage.name}}` and suitability from product record
- `{{problem.name}}` contexts where product is referenced

### 5. Trust Evaluation

- `{{product.trust.score}}` and trust level
- Editorial notes separate from affiliate availability

### 6. Pros and Limitations

- From ingredient benefits/limitations and product flags (sterile, preservative-free)
- Evidence vs marketing distinction

### 7. Safety Notes

- `{{safety_disclaimer}}`
- Cluster and problem safety requirements
- What this product does not treat or diagnose

### 8. Comparison Context

- Brief pointer to related products by category (IDs only — full comparison uses product-comparison template)

### 9. Affiliate and Disclosure

- `{{affiliate_disclosure}}`
- Product affiliate availability field

### 10. Verdict and CTA

- Editorial recommendation framed with cautious language
- `{{cta}}`

### 11. Sources and Review

- Product and ingredient `sources`
- `review.status` from required entities
