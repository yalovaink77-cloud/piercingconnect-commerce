# Template: Category Page

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for a product category landing page on WordPress or PDF catalog.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Product Category | `data/product-categories/{{product_category.id}}.yaml` |
| Product (1+) | From `product_category.related_products` |
| Brand (1+) | From product brand fields |
| Keyword Cluster | `data/keywords/{{keyword_cluster.id}}.yaml` |
| Ingredient (optional) | From `product_category.related_ingredients` |

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
- `{{product_category.summary}}`
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

- `{{meta_title}}` from category + keyword cluster
- `{{meta_description}}`

### 2. Category Hero

- `{{product_category.name}}`
- `{{product_category.summary}}`

### 3. Primary Use and Buyer Intent

- `{{product_category.primary_use}}`
- `{{product_category.buyer_intent}}`
- `{{keyword_cluster.search_intent}}`

### 4. Product Listing Block

- For each product: name, brand, trust score, sterile flags, sizes
- Link to product review template output

### 5. Brand Index

- Unique `{{brand.name}}` entries in category

### 6. Ingredient Context

- `{{ingredient.name}}` common to category
- APP alignment summary

### 7. Healing Stage Suitability

- `{{product_category.suitable_healing_stages}}`

### 8. Safety Notes

- `{{product_category.safety_notes}}`
- `{{safety_disclaimer}}`

### 9. Related Problems

- `{{problem.name}}` from category cross-links

### 10. Affiliate Disclosure

- `{{affiliate_disclosure}}`
- `{{product_category.affiliate_potential}}` — editorial estimate only

### 11. Related Content Links

- Buying guide, comparisons, FAQ spoke links

### 12. CTA

- `{{cta}}`

### 13. Sources and Review

- Category and product sources
- `review.status`
