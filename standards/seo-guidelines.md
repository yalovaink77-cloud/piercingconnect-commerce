# SEO Guidelines

Version: 1.0

Status: Active

Project: PiercingConnect Commercial Knowledge Core

---

## Purpose

SEO strategy rules for keyword clusters, templates, and published content. Trust and safety precede traffic growth.

---

## Keyword Cluster Usage

- Primary keywords live in `data/keywords/` (keyword cluster entities)
- Each cluster includes `search_intent`, `funnel_stage`, and `priority` — editorial estimates only
- **Do not store or publish search volume or CPC** unless verified externally outside this repository

---

## Intent Mapping

| Intent | Content approach | Affiliate placement |
|--------|------------------|---------------------|
| informational | Educate first, soft CTA | moderate |
| commercial | Buying criteria, then products | standard with disclosure |
| comparison | Side-by-side evidence | standard with disclosure |
| transactional | Product focus after criteria | standard with disclosure |
| local | Studio/resource guidance | minimal |
| urgent-problem-solving | Safety first, referral language | minimal or none |

See `data/search-intents/` for structured intent records.

---

## Content Structure

- Match template to intent (see `docs/content-generation-architecture.md`)
- Problem guides: safety sections before product mentions
- Pillar pages: internal links to spoke records by stable IDs
- FAQs: schema-friendly Q&A from entity fields

---

## On-Page Rules

- Title and meta from entity summaries — no clickbait
- Use primary keyword naturally; avoid stuffing
- Include safety disclaimer on aftercare and problem content
- Affiliate disclosure on commercial pages

---

## Prohibited SEO Practices

- Diagnosing conditions to capture medical search intent
- Inventing statistics or healing timelines
- Thin affiliate pages without educational value
- Copying manufacturer marketing as unique content
- Publishing `draft` entities without review flag

---

## Priority Tiers (MVP)

**Critical:** infected piercing, piercing bump — safety-first publishing

**High:** aftercare guides, saline comparisons, best saline spray

See `books/01-aftercare-bible/13-seo-clusters.md`.

---

## Related Documents

- `standards/affiliate-policy.md`
- `data/keywords/`
- `books/01-aftercare-bible/13-seo-clusters.md`
