# Supporting Taxonomies

Version: 1.0

Status: Active

---

# Purpose

This document indexes supporting taxonomy entities that connect the PiercingConnect Knowledge Core to commerce, publishing, geography, and editorial tone.

Structured records live in `data/`. This chapter summarizes coverage for human editors and PC Media Engine.

**Important:** Affiliate commission rates and regional legal claims are not stored in these records. Verify externally before publishing.

---

# Taxonomy Index

| Taxonomy | Records | Status | Review |
|----------|---------|--------|--------|
| Affiliate Programs | 7 | Draft | Pending |
| Content Assets | 10 | Draft | Pending |
| Countries / Regions | 7 | Draft | Pending |
| Risk Levels | 5 | Draft | Pending |
| Search Intents | 6 | Draft | Pending |
| Symptoms | 13 | Draft | Pending |
| Template Entities | 13 | Draft | Pending |

---

# Editorial Rules

1. **Affiliate data is separate from safety** — per taxonomy Rule 5.
2. **Symptoms are not diagnoses** — use problem records for structured troubleshooting.
3. **Risk levels** drive disclaimer depth and affiliate placement limits.
4. **Search intents** map to keyword clusters in `data/keywords/`.
5. **Template entities** in `data/templates/` link to blueprints in `templates/` — not generated content.
6. **Content assets** are downstream publishable outputs.

---

## Affiliate Programs

**Schema:** `schemas/affiliate-program.schema.yaml`

**Data:** `data/affiliate-programs/`

| ID | Name | Status |
|----|------|--------|
| `amazon-associates` | Amazon Associates | Draft |
| `awin` | Awin | Draft |
| `brand-direct` | Brand Direct | Draft |
| `impact` | Impact | Draft |
| `marketplace-affiliate` | Marketplace Affiliate | Draft |
| `shareasale` | ShareASale | Draft |
| `unknown` | Unknown | Draft |

## Content Assets

**Schema:** `schemas/content-asset.schema.yaml`

**Data:** `data/content-assets/`

| ID | Name | Status |
|----|------|--------|
| `buying-guide` | Buying Guide | Draft |
| `comparison-article` | Comparison Article | Draft |
| `email-sequence` | Email Sequence | Draft |
| `facebook-post` | Facebook Post | Draft |
| `faq-page` | FAQ Page | Draft |
| `pdf-guide` | PDF Guide | Draft |
| `pinterest-pin` | Pinterest Pin | Draft |
| `product-review` | Product Review | Draft |
| `wordpress-article` | WordPress Article | Draft |
| `youtube-script` | YouTube Script | Draft |

## Countries / Regions

**Schema:** `schemas/country.schema.yaml`

**Data:** `data/countries/`

| ID | Name | Status |
|----|------|--------|
| `australia` | Australia | Draft |
| `canada` | Canada | Draft |
| `european-union` | European Union | Draft |
| `international` | International | Draft |
| `turkiye` | Türkiye | Draft |
| `united-kingdom` | United Kingdom | Draft |
| `united-states` | United States | Draft |

## Risk Levels

**Schema:** `schemas/risk-level.schema.yaml`

**Data:** `data/risk-levels/`

| ID | Name | Status |
|----|------|--------|
| `medical-attention-required` | Medical Attention Required | Draft |
| `mild-irritation` | Mild Irritation | Draft |
| `moderate-concern` | Moderate Concern | Draft |
| `normal` | Normal | Draft |
| `urgent-professional-review` | Urgent Professional Review | Draft |

## Search Intents

**Schema:** `schemas/search-intent.schema.yaml`

**Data:** `data/search-intents/`

| ID | Name | Status |
|----|------|--------|
| `commercial` | Commercial | Draft |
| `comparison` | Comparison | Draft |
| `informational` | Informational | Draft |
| `local` | Local | Draft |
| `transactional` | Transactional | Draft |
| `urgent-problem-solving` | Urgent Problem Solving | Draft |

## Symptoms

**Schema:** `schemas/symptom.schema.yaml`

**Data:** `data/symptoms/`

| ID | Name | Status |
|----|------|--------|
| `bleeding` | Bleeding | Draft |
| `bump` | Bump | Draft |
| `crust` | Crust | Draft |
| `dryness` | Dryness | Draft |
| `green-discharge` | Green Discharge | Draft |
| `heat` | Heat | Draft |
| `itching` | Itching | Draft |
| `odor` | Odor | Draft |
| `pain` | Pain | Draft |
| `redness` | Redness | Draft |
| `swelling` | Swelling | Draft |
| `tenderness` | Tenderness | Draft |
| `yellow-discharge` | Yellow Discharge | Draft |

## Template Entities

**Schema:** `schemas/template.schema.yaml`

**Data:** `data/templates/`

| ID | Name | Status |
|----|------|--------|
| `aftercare-guide` | Aftercare Guide | Draft |
| `brand-profile` | Brand Profile | Draft |
| `buying-guide` | Buying Guide | Draft |
| `category-page` | Category Page | Draft |
| `email-sequence` | Email Sequence | Draft |
| `facebook-post` | Facebook Post | Draft |
| `faq` | FAQ | Draft |
| `pillar-page` | Pillar Page | Draft |
| `pinterest-pin` | Pinterest Pin | Draft |
| `problem-guide` | Problem Guide | Draft |
| `product-comparison` | Product Comparison | Draft |
| `product-review` | Product Review | Draft |
| `youtube-script` | YouTube Script | Draft |


---

# Relationship Overview

```
Keyword Cluster → Search Intent → Content Asset → Template Entity
Problem → Risk Level + Symptoms
Product / Brand → Affiliate Program + Country
```

---

# Related Data

- `data/affiliate-programs/`
- `data/content-assets/`
- `data/countries/`
- `data/risk-levels/`
- `data/search-intents/`
- `data/symptoms/`
- `data/templates/`
- `docs/content-generation-architecture.md`
- `docs/taxonomy.md`

---

# Status

Supporting taxonomy sprint complete. All listed directories contain structured YAML records with `review.status: draft` and `last_reviewed: 2026-07-08`.
