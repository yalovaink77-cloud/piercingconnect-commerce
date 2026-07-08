# Terminology Guide

Version: 1.0

Status: Active

Project: PiercingConnect Commercial Knowledge Core

---

## Purpose

Approved terms for consistent use across data, books, and published content.

---

## Aftercare Products

| Preferred | Avoid or clarify |
|-----------|------------------|
| sterile saline spray | saline solution (vague), cleaning spray |
| sterile saline wound wash | contact lens solution |
| isotonic saline (0.9% sodium chloride) | homemade sea salt soak (as primary APP-aligned care) |
| packaged sterile saline | DIY mix (note contamination risk) |

---

## Jewelry Materials

| Preferred | Notes |
|-----------|-------|
| implant-grade titanium | Requires ASTM/ISO grade verification — not "hypoallergenic titanium" alone |
| niobium | No implant-grade designation per APP |
| solid 14k gold | Not gold-plated or gold-filled |
| internally threaded / threadless | Preferred for fresh piercings per APP |
| externally threaded | Discouraged for fresh piercings |

See `data/materials/` and `data/jewelry-types/`.

---

## Healing Language

| Preferred | Avoid |
|-----------|-------|
| may take six months or longer (cartilage) | heals in exactly X weeks |
| healing varies by individual | guaranteed recovery |
| irritation bump | keloid (unless clinically diagnosed) |
| infection concern | your piercing is infected |
| seek professional evaluation | treat at home with antiseptic |

---

## Problem Terms

Use problem record names from `data/problems/`:

- irritation bump (not "piercing pimple" in structured data)
- infection concern (not "infected piercing" as a diagnosis)
- jewelry quality issue
- migration, rejection, embedded jewelry

---

## Entity Names

- **Knowledge Core** — this repository
- **PCME** — PC Media Engine (generation layer)
- **APP** — Association of Professional Piercers
- **Keyword cluster** — SEO entity in `data/keywords/`
- **Content asset** — publishable output type in `data/content-assets/`

---

## IDs vs Prose

- YAML `id` fields: kebab-case (`neilmed-piercing-aftercare-fine-mist`)
- Prose: human-readable names (NeilMed Piercing Aftercare Fine Mist)

Never rename IDs without explicit instruction.

---

## Related Documents

- `docs/taxonomy.md`
- `docs/style-guide.md`
- `standards/evidence-policy.md`
