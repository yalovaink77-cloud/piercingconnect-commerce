# Jewelry Materials

Version: 1.0

Status: Active

---

# Purpose

This document provides human-readable profiles for jewelry materials in the PiercingConnect knowledge graph.

The structured data (`data/materials/*.yaml`) is the single source of truth.

**Important:** Material suitability depends on verified grade, fit, finish, and professional selection—not marketing labels alone. Follow `standards/evidence-policy.md`. Distinguish implant-grade standards from terms like "surgical steel" or "hypoallergenic." No medical diagnosis.

---

# Material Index

| Material | Type | APP Alignment | Fresh Piercings | Status | Review |
|----------|------|---------------|---------------|--------|--------|
| Acrylic | `polymer` | Not Recommended | No | Draft | Pending |
| Glass | `glass` | Recommended | Yes | Draft | Pending |
| Implant-Grade Titanium | `biocompatible-metal` | Recommended | Yes | Draft | Pending |
| Mystery Metal | `unknown-unspecified` | Not Recommended | No | Draft | Pending |
| Niobium | `biocompatible-metal` | Recommended | Yes | Draft | Pending |
| Plated Jewelry | `coated-metal` | Not Recommended | No | Draft | Pending |
| PTFE | `polymer` | Not Addressed | No | Draft | Pending |
| Silicone | `polymer` | Not Recommended | No | Draft | Pending |
| Solid 14k Gold | `precious-metal` | Caution | Caution | Draft | Pending |
| Solid 18k Gold | `precious-metal` | Not Recommended | No | Draft | Pending |
| Surgical Steel | `metal-alloy` | Caution | Caution | Draft | Pending |

---

# Acrylic

**Data Source**

`data/materials/acrylic.yaml`

**Research**

`research/materials/acrylic_research.md`

## Summary

Acrylic is a plastic polymer common in fashion jewelry and some low-cost body jewelry. APP initial jewelry guidance does not list acrylic among materials proven appropriate for fresh body piercings. Acrylic is not inert like implant metals or APP-approved glass types and is generally unsuitable for initial healing channels.

## Classification

| Field | Value |
|-------|-------|
| Type | `polymer` |
| APP Alignment | `not-recommended` |
| Fresh Piercings | `false` |
| Healed Piercings | `caution` |
| Allergy Risk | `moderate` |

## Biocompatibility Notes

APP-approved initial materials include specific metals, niobium, solid biocompatible gold, platinum, and defined glass types—not acrylic polymers. Acrylic may release chemicals, harbor bacteria on porous or scratched surfaces, and cannot withstand autoclave conditions the way APP-required initial jewelry materials should. Some piercers may discuss …

## Common Use Cases

- Fashion plugs or decorative jewelry sometimes seen in healed stretched lobes—not initial piercing standard
- Temporary fashion accessories outside APP initial jewelry scope
- Contexts where professional piercers explicitly advise against use in unhealed piercings

## Risks

- Not listed by APP as appropriate for fresh piercings
- Porous or scratched surfaces may harbor bacteria and delay healing
- May crack, warp, or degrade with heat and cleaning products

## Cross-Links

**Piercing Types:** `lobe`, `upper-lobe`, `helix`, `nostril`, `septum`

**Problems:** `jewelry-quality-issue`, `allergic-reaction`, `delayed-healing`, `infection-concern`, `irritation-bump`

---

# Glass

**Data Source**

`data/materials/glass.yaml`

**Research**

`research/materials/glass_research.md`

## Summary

Lead-free borosilicate, lead-free soda-lime, and fused quartz glass are described by APP as inert and considered safe for initial piercings. Glass has a long history of use in piercings. It can be autoclave sterilized per APP.

## Classification

| Field | Value |
|-------|-------|
| Type | `glass` |
| APP Alignment | `recommended` |
| Fresh Piercings | `true` |
| Healed Piercings | `true` |
| Allergy Risk | `low` |

## Biocompatibility Notes

APP lists specific glass types—fused quartz, lead-free borosilicate, and lead-free soda-lime—as inert and safe for initial piercings. Glass must be free of lead and suitable for sterilization. Retainers and plugs are common contexts; breakage risk requires appropriate design and professional selection. This record does not extend APP guidance to un…

## Common Use Cases

- Glass retainers for school, work, or medical imaging when piercer approves
- Initial or healed jewelry in nostril and ear piercings from professional sources
- Situations where a non-metal inert material is preferred after professional assessment

## Risks

- Glass can break under impact; inappropriate style or fit increases trauma risk
- Non-body-jewelry glass may contain lead or unsuitable formulations
- Porous or uneven surfaces on low-quality glass may interfere with healing

## Cross-Links

**Piercing Types:** `nostril`, `septum`, `lobe`, `helix`, `conch`, `labret`, `tongue`, `smiley`

**Problems:** `jewelry-quality-issue`, `snagging`, `embedded-jewelry`

---

# Implant-Grade Titanium

**Data Source**

`data/materials/implant-grade-titanium.yaml`

**Research**

`research/materials/implant-grade-titanium_research.md`

## Summary

Implant-grade titanium is a lightweight metal commonly used for initial body jewelry when it meets recognized ASTM or ISO implant specifications. APP initial jewelry guidance lists implant-certified titanium (such as Ti6Al4V ELI ASTM F-136, ASTM F1295, ISO 5832-3, or commercially pure titanium ASTM F-67) as appropriate for fresh piercings. Marketing labels such as "hypoallergenic titanium" without documented grade do not replace mill test certificates or piercer verification.

## Classification

| Field | Value |
|-------|-------|
| Type | `biocompatible-metal` |
| APP Alignment | `recommended` |
| Fresh Piercings | `true` |
| Healed Piercings | `true` |
| Allergy Risk | `low` |

## Biocompatibility Notes

APP guidance describes titanium as ideal for people with nickel sensitivity concerns when the material meets implant-grade specifications. Anodization can create color without affecting biocompatibility per APP. Mill test certificates document ASTM or ISO grade designations; presence of documentation indicates a piercer may source from reputable su…

## Common Use Cases

- Initial flat-back labret posts for ear and facial piercings
- Curved and straight barbells for navel, nipple, and oral piercings
- Threadless and internally threaded body jewelry from professional studios

## Risks

- Low-quality titanium or undisclosed alloys may still cause irritation in sensitive individuals
- Anodized color may fade in friction-prone areas; fading is not described as harmful by APP
- Poor polish, threads, or fit can cause mechanical irritation regardless of material grade

## Cross-Links

**Piercing Types:** `helix`, `forward-helix`, `flat`, `conch`, `tragus`, `anti-tragus`, `rook`, `daith` (+17 more)

**Problems:** `allergic-reaction`, `jewelry-quality-issue`, `irritation-bump`, `delayed-healing`

---

# Mystery Metal

**Data Source**

`data/materials/mystery-metal.yaml`

**Research**

`research/materials/mystery-metal_research.md`

## Summary

Mystery metal is a PiercingConnect editorial term for body or fashion jewelry with unspecified, unverified, or undisclosed alloy composition. APP initial jewelry guidance requires materials with proven biocompatibility and documented grades where applicable; mystery metal fails that standard.

## Classification

| Field | Value |
|-------|-------|
| Type | `unknown-unspecified` |
| APP Alignment | `not-recommended` |
| Fresh Piercings | `false` |
| Healed Piercings | `false` |
| Allergy Risk | `high` |

## Biocompatibility Notes

APP notes the body jewelry industry is saturated with substandard products and emphasizes cost alone should not drive purchase decisions. Jewelry without mill certs, without piercer verification, or from unverified online sellers often falls into unknown alloy territory. Terms like "hypoallergenic," "surgical," or "premium steel" without ASTM/ISO d…

## Common Use Cases

- Inexpensive online body jewelry with unverified composition
- Mall kiosks, novelty shops, and fashion accessories not from professional studios
- Butterfly-back earrings and piercing-gun-style jewelry referenced in APP troubleshooting contexts

## Risks

- Unknown nickel or irritant content may contribute to allergic or irritant reactions
- No ASTM, ISO, or APP-recognized grade verification
- Rough machining, external threading, and poor polish common in substandard products

## Cross-Links

**Piercing Types:** `helix`, `forward-helix`, `flat`, `conch`, `tragus`, `anti-tragus`, `rook`, `daith` (+17 more)

**Problems:** `jewelry-quality-issue`, `allergic-reaction`, `irritation-bump`, `delayed-healing`, `infection-concern`, `rejection`

---

# Niobium

**Data Source**

`data/materials/niobium.yaml`

**Research**

`research/materials/niobium_research.md`

## Summary

Niobium is a metal widely used by professional piercers with good reported results. APP initial jewelry guidance notes it is very similar to titanium but does not carry an implant-grade designation. It may be anodized for color, including black anodizing unlike titanium per APP.

## Classification

| Field | Value |
|-------|-------|
| Type | `biocompatible-metal` |
| APP Alignment | `recommended` |
| Fresh Piercings | `true` |
| Healed Piercings | `true` |
| Allergy Risk | `low` |

## Biocompatibility Notes

APP describes niobium as inert and compatible for healing piercings when used as quality body jewelry. Unlike titanium, APP explicitly states niobium does not have an implant-grade designation. Anodized niobium may fade due to body chemistry or friction; APP notes this fading is not harmful. Individual sensitivity remains possible despite generally…

## Common Use Cases

- Initial jewelry for clients seeking a titanium alternative
- Anodized niobium including black anodized styles per APP
- Ear, facial, and body piercings where piercer selects appropriate gauge and finish

## Risks

- No implant-grade ASTM/ISO designation means piercer sourcing and finish quality matter
- Anodized surface color may fade with wear or body chemistry
- Rough finish or incorrect sizing can still cause healing complications

## Cross-Links

**Piercing Types:** `helix`, `forward-helix`, `flat`, `conch`, `tragus`, `anti-tragus`, `rook`, `daith` (+17 more)

**Problems:** `allergic-reaction`, `jewelry-quality-issue`, `irritation-bump`

---

# Plated Jewelry

**Data Source**

`data/materials/plated-jewelry.yaml`

**Research**

`research/materials/plated-jewelry_research.md`

## Summary

Plated jewelry—including gold plated, gold-filled, gold overlay, and vermeil—applies a thin surface layer over a base metal. APP initial jewelry guidance explicitly states these are not acceptable for fresh piercings because the coating can wear or chip, exposing underlying alloys.

## Classification

| Field | Value |
|-------|-------|
| Type | `coated-metal` |
| APP Alignment | `not-recommended` |
| Fresh Piercings | `false` |
| Healed Piercings | `caution` |
| Allergy Risk | `high` |

## Biocompatibility Notes

APP distinguishes solid biocompatible gold from gold plated, gold-filled, or gold overlay/vermeil jewelry. The gold surface is very thin and measured in millionths of an inch; it can wear or chip. Underlying base metals may include nickel or other irritants. Fashion and marketplace listings often use "gold tone" or similar marketing without meeting…

## Common Use Cases

- Fashion earrings and costume jewelry not intended for internal long-term wear
- Marketplace body jewelry where low price reflects plated construction
- Should not replace implant-grade or APP-listed initial jewelry in healing piercings

## Risks

- APP lists plated gold products as not acceptable for fresh piercings
- Coating wear exposes base metal and may cause irritation or staining
- Nickel or other allergens in base metal may contact tissue after plating failure

## Cross-Links

**Piercing Types:** `helix`, `forward-helix`, `flat`, `conch`, `tragus`, `anti-tragus`, `rook`, `daith` (+17 more)

**Problems:** `allergic-reaction`, `jewelry-quality-issue`, `irritation-bump`, `delayed-healing`, `infection-concern`

---

# PTFE

**Data Source**

`data/materials/ptfe.yaml`

**Research**

`research/materials/ptfe_research.md`

## Summary

PTFE (polytetrafluoroethylene), sometimes sold as flexible piercing retainers or temporary bars, is not listed in APP initial jewelry guidance among materials proven appropriate for fresh piercings. Professional use, if any, is typically limited to specific healed or temporary contexts determined by a piercer.

## Classification

| Field | Value |
|-------|-------|
| Type | `polymer` |
| APP Alignment | `not-addressed` |
| Fresh Piercings | `false` |
| Healed Piercings | `caution` |
| Allergy Risk | `low` |

## Biocompatibility Notes

APP initial jewelry brochure does not include PTFE in its list of materials with proven biocompatibility for fresh piercings. PTFE is flexible and may appear in retainers; flexibility can reduce certain mechanical stresses but also introduces movement and fit variables. PiercingConnect classifies APP alignment as not-addressed rather than recommend…

## Common Use Cases

- Flexible retainers sometimes discussed for healed pierings or temporary concealment
- Not an APP-listed initial jewelry material
- Professional assessment required before any use in or near a healing piercing

## Risks

- Not proven appropriate for fresh piercings under APP initial jewelry guidance
- Flexible jewelry may move excessively and cause irritation in some placements
- Low-quality PTFE products may have rough ends or poor fit

## Cross-Links

**Piercing Types:** `nostril`, `septum`, `labret`, `medusa`, `monroe`, `philtrum`, `tongue`, `smiley` (+1 more)

**Problems:** `jewelry-quality-issue`, `migration`, `pressure-irritation`, `snagging`

---

# Silicone

**Data Source**

`data/materials/silicone.yaml`

**Research**

`research/materials/silicone_research.md`

## Summary

Silicone body jewelry and o-rings appear in consumer markets but are not listed in APP initial jewelry guidance as materials proven appropriate for fresh piercings. Quality, grade, and suitability vary widely; medical-grade claims in marketing are not verified by PiercingConnect without manufacturer documentation.

## Classification

| Field | Value |
|-------|-------|
| Type | `polymer` |
| APP Alignment | `not-recommended` |
| Fresh Piercings | `false` |
| Healed Piercings | `caution` |
| Allergy Risk | `moderate` |

## Biocompatibility Notes

APP initial jewelry materials focus on specific metals, niobium, solid gold meeting criteria, platinum, and defined glass types. Silicone is not included. Some silicone products advertise medical or implant grades; PiercingConnect does not invent certifications and treats such labels as marketing until verified through piercer and manufacturer docu…

## Common Use Cases

- Silicone o-rings on barbell assemblies—compatibility depends on overall jewelry quality
- Occasional healed-piercing contexts discussed in studios; not APP initial standard
- Not recommended as primary initial jewelry material per APP scope

## Risks

- Not listed in APP initial jewelry material guidance
- Grade variability; marketing terms may not reflect actual composition
- Porous or damaged silicone may harbor bacteria

## Cross-Links

**Piercing Types:** `navel`, `nipple`, `tongue`, `lobe`, `septum`

**Problems:** `jewelry-quality-issue`, `allergic-reaction`, `moisture-irritation`, `delayed-healing`

---

# Solid 14k Gold

**Data Source**

`data/materials/solid-14k-gold.yaml`

**Research**

`research/materials/solid-14k-gold_research.md`

## Summary

Solid 14 karat gold may be appropriate for initial piercings when it is nickel- and cadmium-free and alloyed for biocompatibility per APP initial jewelry guidance. This record refers to solid gold body jewelry, not plated or gold-filled products. Alloy composition and vendor verification matter because not all gold jewelry meets APP criteria.

## Classification

| Field | Value |
|-------|-------|
| Type | `precious-metal` |
| APP Alignment | `acceptable-with-caution` |
| Fresh Piercings | `caution` |
| Healed Piercings | `true` |
| Allergy Risk | `moderate` |

## Biocompatibility Notes

APP states yellow, rose, or white gold is appropriate for initial piercings if 14k or higher, nickel- and cadmium-free, and alloyed for biocompatibility. Solid gold differs from gold plated, gold-filled, or vermeil jewelry, which APP lists as not acceptable for fresh piercings. PiercingConnect does not certify specific gold alloys; piercers should …

## Common Use Cases

- Initial or healed jewelry when piercer confirms nickel- and cadmium-free solid alloy
- Clients preferring precious metal aesthetics in ear, nose, and lip piercings
- Healed piercings where solid gold meets studio quality standards

## Risks

- Gold alloys may contain nickel or other sensitizers if not confirmed biocompatible
- Soft gold can scratch or nick, creating surfaces that may harbor bacteria if poorly maintained
- Confusion with plated or gold-filled jewelry that is not suitable for fresh piercings

## Cross-Links

**Piercing Types:** `helix`, `forward-helix`, `flat`, `conch`, `tragus`, `anti-tragus`, `rook`, `daith` (+17 more)

**Problems:** `allergic-reaction`, `jewelry-quality-issue`, `irritation-bump`, `delayed-healing`

---

# Solid 18k Gold

**Data Source**

`data/materials/solid-18k-gold.yaml`

**Research**

`research/materials/solid-18k-gold_research.md`

## Summary

Solid 18 karat gold is softer than 14k gold. APP initial jewelry guidance states gold higher than 18k is too soft for body jewelry because it can easily be scratched or nicked. This record covers solid 18k only; plated gold products are separate and not recommended for fresh piercings.

## Classification

| Field | Value |
|-------|-------|
| Type | `precious-metal` |
| APP Alignment | `not-recommended` |
| Fresh Piercings | `false` |
| Healed Piercings | `caution` |
| Allergy Risk | `moderate` |

## Biocompatibility Notes

APP allows 14k or higher gold for initial piercings when nickel- and cadmium-free and alloyed for biocompatibility, but notes gold above 18k is too soft. At 18k, APP guidance implies suitability is borderline for mechanical durability in body jewelry. Piercers may prefer 14k for initial wear and reserve higher karat for healed piercings with approp…

## Common Use Cases

- Healed piercings where client and piercer accept softer metal trade-offs
- Decorative ends or low-friction placements after professional assessment
- Not typically recommended as first choice for initial jewelry per APP softness note

## Risks

- Easier scratching and nicking than 14k gold may affect surface integrity
- Soft metal may not withstand daily trauma in active piercings
- Alloy sensitizers still possible if nickel or cadmium are present

## Cross-Links

**Piercing Types:** `lobe`, `upper-lobe`, `nostril`, `helix`, `septum`, `labret`, `medusa`, `philtrum`

**Problems:** `jewelry-quality-issue`, `allergic-reaction`, `snagging`, `irritation-bump`

---

# Surgical Steel

**Data Source**

`data/materials/surgical-steel.yaml`

**Research**

`research/materials/surgical-steel_research.md`

## Summary

Surgical steel is a marketing term covering many stainless steel alloys. APP initial jewelry guidance states only specific grades are proven biocompatible, including ASTM F-138 compliant or ISO 5832-1 compliant steel and related ISO 10993 or EEC Nickel Directive compliance. Unspecified "surgical steel" without documented grade is not equivalent to implant-grade steel.

## Classification

| Field | Value |
|-------|-------|
| Type | `metal-alloy` |
| APP Alignment | `acceptable-with-caution` |
| Fresh Piercings | `caution` |
| Healed Piercings | `caution` |
| Allergy Risk | `moderate` |

## Biocompatibility Notes

APP emphasizes that many alloys are used for body jewelry but only certain grades are proven biocompatible for fresh piercings. Mill test certificates with ASTM or ISO designations document grade; consumers need not interpret certificate numbers but should know documentation exists when piercers review supplier quality. Labeling alone—such as "316L…

## Common Use Cases

- Body jewelry when piercer confirms ASTM F-138 or ISO 5832-1 compliant grade
- Healed piercings where client tolerates steel and grade is verified
- Not interchangeable with generic mall or fashion "surgical steel" labels

## Risks

- Nickel and other alloy components may trigger sensitivity in some people
- Unverified surgical steel may not meet biocompatibility standards APP lists
- Marketing term overuse obscures actual alloy grade and nickel release

## Cross-Links

**Piercing Types:** `helix`, `forward-helix`, `flat`, `conch`, `tragus`, `anti-tragus`, `rook`, `daith` (+17 more)

**Problems:** `allergic-reaction`, `jewelry-quality-issue`, `irritation-bump`, `delayed-healing`

---



# Editorial Notes

All factual changes should be made in the corresponding YAML record first.

APP initial jewelry guidance lists specific metals, niobium, solid biocompatible gold, platinum, and defined glass types as appropriate for fresh piercings when quality and grade are verified. Plated jewelry and unspecified alloys are not equivalent.

PiercingConnect does not invent ASTM, ISO, or mill certificate claims for individual products. Piercers may review supplier documentation; consumers should rely on qualified professional selection.

---

# Related Data

- `data/materials/`
- `data/piercing-types/`
- `data/problems/`
- `schemas/material.schema.yaml`
- `research/materials/`

---

# Status

Current Coverage (11 materials):

- Acrylic
- Glass
- Implant-Grade Titanium
- Mystery Metal
- Niobium
- Plated Jewelry
- PTFE
- Silicone
- Solid 14k Gold
- Solid 18k Gold
- Surgical Steel
