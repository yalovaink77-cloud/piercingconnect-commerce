# Information Architecture

Version: 1.0

Status: Active

---

# Purpose

This chapter defines how Book 1 — Aftercare Bible is organized and how it connects to the Knowledge Core in `data/`.

---

# Layer Model

| Layer | Location | Role |
|-------|----------|------|
| Structured truth | `data/*.yaml` | Canonical records for PCME |
| Human summary | `books/01-aftercare-bible/` | Editor and strategist reference |
| Blueprints | `templates/` | Section structures for generation |
| Strategy | `standards/`, `docs/` | Rules and architecture |

**Rule:** If book and data disagree, reconcile both — data is machine source of truth.

---

# Book 1 Chapter Map

Book 1 uses two chapter number ranges:

1. **Foundation chapters (01–08)** — architecture, medical context, strategy, publishing
2. **Knowledge chapters (04–14)** — populated database summaries synced to `data/`

Some foundation slot numbers overlap with knowledge chapters added during MVP sprints. Legacy empty slots were converted to navigation chapters. Populated knowledge was **not** renumbered to avoid breaking references.

---

# Foundation Chapters

| File | Title | Status |
|------|-------|--------|
| `00-index.md` | Book index | Active |
| `01-information-architecture.md` | This document | Active |
| `02-medical-foundation.md` | Medical reference outline | Draft |
| `03-product-categories.md` | → Navigation to ch. 12 | Redirect |
| `07-affiliate-strategy.md` | Affiliate strategy overview | Active |
| `08-pcme-publishing.md` | → PCME architecture link | Redirect |

---

# Knowledge Chapters (synced to data/)

| File | Data path | Entity |
|------|-----------|--------|
| `04-brand-database.md` | `data/brands/`, `data/products/` | Brands, products |
| `05-problem-database.md` | `data/problems/` | Problems |
| `06-ingredient-database.md` | `data/ingredients/` | Ingredients |
| `07-healing-stages.md` | `data/healing-stages/` | Healing stages |
| `08-piercing-types.md` | `data/piercing-types/` | Piercing types |
| `09-body-locations.md` | `data/body-locations/` | Body locations |
| `10-jewelry-materials.md` | `data/materials/` | Materials |
| `11-jewelry-types.md` | `data/jewelry-types/` | Jewelry types |
| `12-product-categories.md` | `data/product-categories/` | Product categories |
| `13-seo-clusters.md` | `data/keywords/` | Keyword clusters |
| `14-supporting-taxonomies.md` | Supporting `data/` dirs | Taxonomies |

---

# Legacy Navigation Slots

These files exist at original planned numbers and point to canonical chapters:

| Legacy file | Canonical content |
|-------------|-------------------|
| `03-product-categories.md` | `12-product-categories.md` |
| `06-seo-clusters.md` | `13-seo-clusters.md` |

Note: `06-ingredient-database.md` occupies the 06 slot for knowledge content. SEO clusters moved to 13.

---

# Numbering Collision Notes

| Slot | Foundation topic | Knowledge chapter (same number) |
|------|------------------|--------------------------------|
| 06 | SEO (legacy nav) | Ingredient database |
| 07 | Affiliate strategy | Healing stages |
| 08 | PCME publishing (legacy nav) | Piercing types |

Read foundation files at 07 for affiliate strategy. Read `08-pcme-publishing.md` for publishing pipeline. Knowledge content at those numbers is authoritative for entity data.

---

# Cross-References

- Architecture: `docs/architecture.md`
- Content generation: `docs/content-generation-architecture.md`
- Taxonomy: `docs/taxonomy.md`
- Workflow: `docs/workflow.md`

---

# Status

Information architecture stabilized for repository v1.0. Full Book 1 renumbering deferred to a future refactor if needed.
