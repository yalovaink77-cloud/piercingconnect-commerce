# Content Generation Architecture

Version: 1.0

Status: Active

Project: PiercingConnect Commercial Knowledge Core

---

## Purpose

This document defines how structured knowledge in the repository becomes publishable content through templates and the PC Media Engine (PCME).

The Knowledge Core is the source of truth. Templates are reusable blueprints. PCME resolves entities, fills placeholders, applies standards, and outputs channel-specific assets.

Published articles, posts, pins, emails, and scripts are **outputs** — never source knowledge.

---

## Pipeline

```
Knowledge Core (data/ + schemas/ + standards/)
        ↓
Template Engine (templates/ + entity resolution)
        ↓
PC Media Engine (generation, validation, export)
        ↓
Publishing Targets (WordPress, Facebook, Pinterest, Email, YouTube, PDF)
```

### Layer responsibilities

| Layer | Path | Role |
|-------|------|------|
| Knowledge Core | `data/`, `schemas/`, `standards/` | Canonical YAML entities, validation rules, evidence and affiliate policies |
| Template Engine | `templates/` | Section blueprints, required entity contracts, placeholder variables |
| PC Media Engine | External automation consuming exports | Resolve IDs, generate prose, enforce standards, route to channels |
| Publishing | WordPress, social, email, video, PDF | Downstream distribution — not stored as source truth |

### Generation rules

1. PCME must load all **required entities** for a template before generation.
2. Safety and evidence rules in `standards/evidence-policy.md` override affiliate or commercial fields.
3. Entity `review.status` must be checked; `draft` entities require editorial flag in output.
4. Templates define **sections only** — PCME generates prose from entity fields.
5. No search volume or CPC may be invented; keyword clusters supply editorial intent only.

---

## Knowledge Core Entity Paths

| Entity | Schema | Data path |
|--------|--------|-----------|
| Brand | `schemas/brand.schema.yaml` | `data/brands/` |
| Product | `schemas/product.schema.yaml` | `data/products/` |
| Ingredient | `schemas/ingredient.schema.yaml` | `data/ingredients/` |
| Problem | `schemas/problem.schema.yaml` | `data/problems/` |
| Healing Stage | `schemas/healing-stage.schema.yaml` | `data/healing-stages/` |
| Piercing Type | `schemas/piercing-type.schema.yaml` | `data/piercing-types/` |
| Body Location | `schemas/body-location.schema.yaml` | `data/body-locations/` |
| Material | `schemas/material.schema.yaml` | `data/materials/` |
| Jewelry Type | `schemas/jewelry-type.schema.yaml` | `data/jewelry-types/` |
| Product Category | `schemas/product-category.schema.yaml` | `data/product-categories/` |
| Keyword Cluster | `schemas/keyword-cluster.schema.yaml` | `data/keywords/` |

Cross-links between entities use stable **IDs** (kebab-case). PCME resolves IDs to records at generation time.

---

## Template Variable Convention

Placeholders use double curly braces. Nested entity fields use dot notation.

### Core entities

| Placeholder | Source field |
|-------------|--------------|
| `{{brand.name}}` | Brand human-readable name |
| `{{brand.id}}` | Brand stable ID |
| `{{product.name}}` | Product name |
| `{{product.category}}` | Product category ID |
| `{{product.trust.score}}` | Product trust score |
| `{{ingredient.name}}` | Ingredient name |
| `{{ingredient.app_alignment}}` | APP alignment flag |
| `{{problem.name}}` | Problem name |
| `{{problem.summary}}` | Problem summary |
| `{{healing_stage.name}}` | Healing stage name |
| `{{healing_stage.summary}}` | Healing stage summary |
| `{{piercing_type.name}}` | Piercing type name |
| `{{piercing_type.aftercare_notes}}` | Piercing type aftercare list |
| `{{body_location.name}}` | Body location name |
| `{{material.name}}` | Material name |
| `{{jewelry_type.name}}` | Jewelry type name |
| `{{product_category.name}}` | Product category name |
| `{{keyword_cluster.primary_keyword}}` | Target keyword phrase |
| `{{keyword_cluster.search_intent}}` | Search intent type |
| `{{keyword_cluster.safety_notes}}` | Cluster safety requirements |

### Generation and compliance

| Placeholder | Purpose |
|-------------|---------|
| `{{meta_title}}` | SEO title derived from keyword cluster + entity |
| `{{meta_description}}` | Meta description from summaries |
| `{{cta}}` | Channel-appropriate call to action |
| `{{affiliate_disclosure}}` | Required affiliate disclosure block |
| `{{safety_disclaimer}}` | Non-diagnosis / professional referral disclaimer |
| `{{review_status_note}}` | Editorial note when source entities are draft |

List fields render as repeated blocks (e.g. `{{#each problem.recommended_actions}}` in PCME — not stored in template prose).

---

## Required Entities by Template

### Brand Profile

**Template:** `templates/brand-profile.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Brand | Yes | `data/brands/{{brand.id}}.yaml` |
| Product | Yes (1+) | `data/products/*.yaml` linked via `brand` |
| Product Category | Yes (1+) | Derived from product `category` → `data/product-categories/` |
| Keyword Cluster | Yes | `data/keywords/{{keyword_cluster.id}}.yaml` |

---

### Product Review

**Template:** `templates/product-review.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Brand | Yes | `data/brands/{{brand.id}}.yaml` |
| Product | Yes | `data/products/{{product.id}}.yaml` |
| Ingredient | Yes (1+) | Resolved from `product.ingredients` |
| Problem | Yes (1+) | From product / ingredient / category cross-links |
| Healing Stage | Yes (1+) | From `product.healing_stages` |
| Keyword Cluster | Yes | `data/keywords/{{keyword_cluster.id}}.yaml` |

---

### Product Comparison

**Template:** `templates/product-comparison.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Brand | Yes (2+) | Two or more brand records |
| Product | Yes (2+) | Comparison product set |
| Ingredient | Yes | Union of product ingredient lists |
| Product Category | Yes | Shared or primary category |
| Keyword Cluster | Yes | Comparison-intent cluster |

---

### Aftercare Guide

**Template:** `templates/aftercare-guide.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Piercing Type | Yes | `data/piercing-types/{{piercing_type.id}}.yaml` |
| Body Location | Yes | From `piercing_type.body_location` |
| Healing Stage | Yes (1+) | From piercing type `healing_stages` |
| Product | Optional (1+) | From `piercing_type.recommended_products` |
| Ingredient | Optional (1+) | From recommended product ingredients |
| Material | Optional (1+) | From `piercing_type.suitable_materials` |
| Jewelry Type | Optional (1+) | From `piercing_type.suitable_jewelry` |
| Keyword Cluster | Yes | Informational aftercare cluster |

---

### Problem Guide

**Template:** `templates/problem-guide.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Problem | Yes | `data/problems/{{problem.id}}.yaml` |
| Ingredient | Yes (1+) | From `problem.related_ingredients` |
| Healing Stage | Yes (1+) | From `problem.healing_stages` |
| Product | Yes (1+) | From `problem.related_products` |
| Piercing Type | Yes (1+) | From problem context / cluster cross-links |
| Keyword Cluster | Yes | Problem-intent cluster |

---

### Buying Guide

**Template:** `templates/buying-guide.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Product Category | Yes | `data/product-categories/{{product_category.id}}.yaml` |
| Product | Yes (2+) | From `product_category.related_products` |
| Brand | Yes (1+) | From product `brand` fields |
| Ingredient | Yes (1+) | From category `related_ingredients` |
| Keyword Cluster | Yes | Commercial-intent cluster |

---

### FAQ

**Template:** `templates/faq.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Keyword Cluster | Yes | Primary question cluster |
| Problem | Conditional | When cluster maps to problem intent |
| Piercing Type | Conditional | When cluster maps to aftercare intent |
| Product Category | Conditional | When cluster maps to commercial intent |
| Product | Optional | When FAQ includes product answers |
| Healing Stage | Optional | When timing questions apply |

At least one topical entity (Problem, Piercing Type, or Product Category) beyond the keyword cluster is required.

---

### Pillar Page

**Template:** `templates/pillar-page.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Keyword Cluster | Yes | Primary pillar keyword |
| Product Category | Yes (1+) | Hub category links |
| Problem | Yes (1+) | Spoke problem links |
| Piercing Type | Yes (1+) | Spoke aftercare links |
| Healing Stage | Yes (1+) | Foundational healing context |
| Product | Optional | Featured products |
| Brand | Optional | Featured brands |

---

### Category Page

**Template:** `templates/category-page.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Product Category | Yes | Primary category record |
| Product | Yes (1+) | `product_category.related_products` |
| Brand | Yes (1+) | Brands of listed products |
| Ingredient | Optional | `product_category.related_ingredients` |
| Keyword Cluster | Yes | Category or commercial cluster |

---

### Email Sequence

**Template:** `templates/email-sequence.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Keyword Cluster | Yes | Sequence theme / intent |
| Product | Conditional | Product-focused sequences |
| Brand | Conditional | Brand onboarding sequences |
| Problem | Conditional | Problem-education sequences |
| Piercing Type | Conditional | Aftercare onboarding sequences |
| Healing Stage | Yes (1+) | Timing for sequence steps |

Primary topical entity (Product, Brand, Problem, or Piercing Type) plus keyword cluster required.

---

### Pinterest Pin

**Template:** `templates/pinterest-pin.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Keyword Cluster | Yes | Pin SEO keyword |
| Problem | Conditional | Problem pin |
| Piercing Type | Conditional | Aftercare pin |
| Product | Conditional | Product pin |
| Product Category | Optional | Category pin |

One focal entity (Problem, Piercing Type, or Product) plus keyword cluster required.

---

### Facebook Post

**Template:** `templates/facebook-post.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Keyword Cluster | Yes | Post angle / hook keyword |
| Product | Conditional | Product post |
| Brand | Conditional | Brand post |
| Problem | Conditional | Education post |
| Piercing Type | Conditional | Aftercare tip post |

One focal entity plus keyword cluster required.

---

### YouTube Script

**Template:** `templates/youtube-script.md`

| Entity | Required | Data path |
|--------|----------|-----------|
| Keyword Cluster | Yes | Video target keyword |
| Piercing Type | Conditional | Aftercare video |
| Problem | Conditional | Troubleshooting video |
| Product | Conditional | Review video |
| Brand | Conditional | Brand profile video |
| Ingredient | Conditional | Ingredient explainer |
| Healing Stage | Yes (1+) | Timeline context |

Script type determines focal entities; keyword cluster always required.

---

## Template Matrix

Publishing target key: **Y** = supported output, **—** = not primary target

| Template | Required Knowledge Entities | WordPress | Facebook | Pinterest | Email | YouTube | PDF |
|----------|----------------------------|-----------|----------|-----------|-------|---------|-----|
| Brand Profile | Brand, Product, Product Category, Keyword Cluster | Y | Y | — | Y | — | Y |
| Product Review | Brand, Product, Ingredient, Problem, Healing Stage, Keyword Cluster | Y | Y | Y | Y | — | Y |
| Product Comparison | Brand, Product, Ingredient, Product Category, Keyword Cluster | Y | Y | Y | Y | — | Y |
| Aftercare Guide | Piercing Type, Body Location, Healing Stage, Keyword Cluster; optional Product, Ingredient, Material, Jewelry Type | Y | Y | Y | Y | Y | Y |
| Problem Guide | Problem, Ingredient, Healing Stage, Product, Piercing Type, Keyword Cluster | Y | Y | Y | Y | Y | Y |
| Buying Guide | Product Category, Product, Brand, Ingredient, Keyword Cluster | Y | Y | Y | Y | — | Y |
| FAQ | Keyword Cluster + topical entity (Problem, Piercing Type, or Product Category) | Y | Y | Y | Y | — | Y |
| Pillar Page | Keyword Cluster, Product Category, Problem, Piercing Type, Healing Stage | Y | Y | Y | Y | Y | Y |
| Category Page | Product Category, Product, Brand, Keyword Cluster | Y | Y | Y | Y | — | Y |
| Email Sequence | Keyword Cluster, Healing Stage, topical entity | — | — | — | Y | — | — |
| Pinterest Pin | Keyword Cluster, focal entity | — | — | Y | — | — | — |
| Facebook Post | Keyword Cluster, focal entity | — | Y | — | — | — | — |
| YouTube Script | Keyword Cluster, Healing Stage, focal entity | Y | — | — | — | Y | — |

---

## PCME Generation Checklist

Before generating content from any template:

1. Resolve all required entity IDs and confirm records exist in `data/`.
2. Load applicable standards (`standards/evidence-policy.md`, affiliate policy).
3. Apply `keyword_cluster.safety_notes` when present — overrides affiliate placement.
4. Insert `{{affiliate_disclosure}}` when `product.affiliate.available` or commercial template.
5. Insert `{{safety_disclaimer}}` on all problem and aftercare templates.
6. Block generation or flag output when high-risk problem clusters lack safety sections.
7. Set `{{review_status_note}}` when any required entity has `review.status: draft`.

---

## Related Documents

- [ai-developer-guide.md](ai-developer-guide.md)
- [architecture.md](architecture.md)
- [taxonomy.md](taxonomy.md)
- [workflow.md](workflow.md)
- `standards/evidence-policy.md`
- `templates/` — section blueprints

---

## Status

MVP Content Templates Core active. Thirteen templates ship with this architecture. PCME integration and export scripts are downstream work.
