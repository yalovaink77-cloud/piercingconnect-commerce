# Affiliate Policy

Version: 1.0

Status: Active

Project: PiercingConnect Commercial Knowledge Core

---

## Purpose

Define how PiercingConnect uses affiliate relationships without compromising safety, evidence, or user trust.

Affiliate value is stored separately from product quality evaluation per taxonomy Rule 5.

---

## Core Rule

**Safety and evidence always override affiliate opportunity.**

A product with affiliate availability is not automatically recommended. A product without affiliate availability may still be recommended when evidence supports it.

---

## Evaluation Order

When recommending or comparing products:

1. Safety and APP alignment
2. Ingredients and formulation evidence
3. Trust score and manufacturer documentation
4. User need and healing stage fit
5. Availability
6. Affiliate opportunity (last)

---

## Disclosure Requirements

- Clear affiliate disclosure near commercial links
- Follow FTC guidelines (US) and applicable regional rules
- Do not hide affiliate relationships in generated content
- PCME outputs must include `{{affiliate_disclosure}}` on commercial templates

---

## Data Rules

- Affiliate program records live in `data/affiliate-programs/`
- **Do not invent commission rates or cookie durations** in structured data
- Use `commission_notes: unknown` or verify from official program documentation
- Mark unverified programs as `unknown` until confirmed
- Product `affiliate.available` is a flag only — not a quality endorsement

---

## Prohibited Practices

- Ranking products by commission rate
- Recommending harsh or APP-not-recommended products because they pay well
- Using marketplace copy as primary safety evidence
- Omitting safer non-affiliate alternatives when relevant
- Problem-intent content with aggressive product CTAs (infection, bumps, etc.)

---

## Keyword Cluster Rules

- `urgent-problem-solving` intent → minimal or no affiliate placement
- Comparison clusters → present trust scores and ingredients, not payout
- Commercial clusters → disclosure required; safety criteria still first

---

## Related Documents

- `standards/evidence-policy.md`
- `standards/editorial-guidelines.md`
- `data/affiliate-programs/`
- `books/01-aftercare-bible/07-affiliate-strategy.md`
