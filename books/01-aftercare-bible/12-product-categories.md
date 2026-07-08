# Product Categories

Version: 1.0

Status: Active

---

# Purpose

This document provides human-readable profiles for aftercare and piercing-related product categories in the PiercingConnect knowledge graph.

The structured data (`data/product-categories/*.yaml`) is the single source of truth.

**Important:** Category records organize commerce knowledge—they do not replace individual product trust scores or APP-aligned ingredient review. Safety before affiliate opportunity per `standards/evidence-policy.md` and taxonomy Rule 5. No medical diagnosis.

---

# Category Index

| Category | Type | Affiliate Potential | Buyer Intent | Status | Review |
|----------|------|---------------------|--------------|--------|--------|
| Compress | `accessory` | Low | Problem Solving | Draft | Pending |
| Foam Soap | `cleaning-product` | Moderate | Routine Aftercare | Draft | Pending |
| Healing Soak | `aftercare-solution` | Moderate | Problem Solving | Draft | Pending |
| Jewelry Storage | `storage` | Moderate | Organization | Draft | Pending |
| Mirror | `tool` | Low | Organization | Draft | Pending |
| Piercing Aftercare Kit | `kit-bundle` | High | Post-Piercing Setup | Draft | Pending |
| Piercing Pillow | `comfort-aid` | Moderate | Comfort Support | Draft | Pending |
| Saline Spray | `aftercare-solution` | High | Comparison Research | Draft | Pending |
| Sterile Gauze | `wound-care` | Moderate | Routine Aftercare | Draft | Pending |
| Sterile Saline Spray | `aftercare-solution` | High | Routine Aftercare | Draft | Pending |
| Travel Aftercare Kit | `kit-bundle` | Moderate | Travel Convenience | Draft | Pending |
| Wound Wash | `wound-care` | High | Comparison Research | Draft | Pending |

---

# Editorial Rule: Safety vs Affiliate

Affiliate potential estimates commercial opportunity for content strategy. It is stored separately from safety evaluation.

High affiliate potential categories such as sterile saline spray still require per-product ingredient, sterility, and trust review before recommendation.

---

# Compress

**Data Source**

`data/product-categories/compress.yaml`

**Research**

`research/product-categories/compress_research.md`

## Summary

Compress products—including gel packs, warm compress pads, or DIY cloth compresses—may sometimes be discussed for comfort around swollen or irritated tissue near a piercing. APP troubleshooting focuses on removing mechanical causes of irritation; compresses are supportive comfort measures, not primary piercing aftercare and not infection treatment.

## Classification

| Field | Value |
|-------|-------|
| Type | `accessory` |
| Primary Use | Apply cold or warm compress externally to support comfort during swelling or irritation. |
| Affiliate Potential | `low` |
| Buyer Intent | `problem-solving` |

## Safety Notes

- Do not use compresses as a substitute for sterile saline aftercare or piercer assessment
- Avoid excessive heat that may increase inflammation; follow clinician or piercer guidance when unsure
- Keep compress materials clean; do not apply unclean cloths directly to a fresh piercing

## Cross-Links

**Products:** None mapped yet

**Ingredients:** None

**Healing Stages:** `fresh-piercing`, `early-healing`, `irritated-piercing`

**Problems:** `swelling`, `irritation-bump`, `pressure-irritation`, `bleeding`

---

# Foam Soap

**Data Source**

`data/product-categories/foam-soap.yaml`

**Research**

`research/product-categories/foam-soap_research.md`

## Summary

Foam soap products are mild cleansers sometimes used in shower routines around healed or healing external piercings. APP body aftercare notes a brief rinse with mild soap during normal bathing may be acceptable for some piercings; foam formats are a commercial variant of gentle cleansing—not a replacement for sterile saline rinsing and not a primary antiseptic treatment.

## Classification

| Field | Value |
|-------|-------|
| Type | `cleaning-product` |
| Primary Use | Support gentle external cleansing around piercings during normal bathing when approved by piercer. |
| Affiliate Potential | `moderate` |
| Buyer Intent | `routine-aftercare` |

## Safety Notes

- Fragrance, dye, and harsh surfactants may irritate healing piercings
- Foam soap is supplementary; sterile saline remains the primary APP-recommended rinse for many piercings
- Discontinue if rash or increased irritation appears and consult your piercer

## Cross-Links

**Products:** None mapped yet

**Ingredients:** `preservatives`, `purified-water`

**Healing Stages:** `early-healing`, `active-healing`, `late-healing`, `mature-piercing`

**Problems:** `overcleaning`, `allergic-reaction`, `dryness`, `moisture-irritation`

---

# Healing Soak

**Data Source**

`data/product-categories/healing-soak.yaml`

**Research**

`research/product-categories/healing-soak_research.md`

## Summary

Healing soaks refer to immersing a piercing in warm salt water or commercial soak products. APP aftercare favors packaged sterile saline over home sea-salt soaks because mixing strength, sterility, and contamination are difficult to control. This category documents the commercial and community soak concept for comparison without endorsing uncontrolled home mixing as primary aftercare.

## Classification

| Field | Value |
|-------|-------|
| Type | `aftercare-solution` |
| Primary Use | Salt-water soaks discussed historically in piercing aftercare; requires caution versus packaged saline. |
| Affiliate Potential | `moderate` |
| Buyer Intent | `problem-solving` |

## Safety Notes

- APP recommends packaged sterile saline rather than homemade sea-salt soaks
- Excessive soaking may trap moisture and contribute to irritation in some piercings
- Non-sterile water or incorrect salt concentration introduces contamination risk

## Cross-Links

**Products:** None mapped yet

**Ingredients:** `sea-salt`, `sodium-chloride-0.9-percent`

**Healing Stages:** `irritated-piercing`, `active-healing`

**Problems:** `overcleaning`, `moisture-irritation`, `infection-concern`, `irritation-bump`

---

# Jewelry Storage

**Data Source**

`data/product-categories/jewelry-storage.yaml`

**Research**

`research/product-categories/jewelry-storage_research.md`

## Summary

Jewelry storage includes cases, boxes, and organizers for body jewelry collections. Storage supports jewelry quality by reducing scratches, tangling, and exposure to moisture or debris. It does not replace implant-grade materials or professional fit but may reduce mechanical damage to healed jewelry between wears.

## Classification

| Field | Value |
|-------|-------|
| Type | `storage` |
| Primary Use | Organize and protect body jewelry when not worn to reduce damage and contamination. |
| Affiliate Potential | `moderate` |
| Buyer Intent | `organization` |

## Safety Notes

- Store clean, dry jewelry; wet or contaminated storage may harbor bacteria
- Do not store healing jewelry removed prematurely in shared containers without cleaning protocol
- Storage accessories do not upgrade low-quality jewelry materials

## Cross-Links

**Products:** None mapped yet

**Ingredients:** None

**Healing Stages:** `mature-piercing`, `retired-piercing`

**Problems:** `jewelry-quality-issue`, `snagging`, `allergic-reaction`

---

# Mirror

**Data Source**

`data/product-categories/mirror.yaml`

**Research**

`research/product-categories/mirror_research.md`

## Summary

Mirrors—including handheld, magnifying, and wearable styles—help clients inspect piercings or assist with jewelry changes when a piercer has cleared timing. Mirrors are inspection tools, not aftercare treatments. PiercingConnect discourages unsupervised early jewelry changes even when mirrors improve visibility.

## Classification

| Field | Value |
|-------|-------|
| Type | `tool` |
| Primary Use | Visual inspection and jewelry installation assistance for healed or professionally managed piercings. |
| Affiliate Potential | `low` |
| Buyer Intent | `organization` |

## Safety Notes

- Visibility tools do not replace professional jewelry changes during healing
- Magnification may highlight normal crusting and cause unnecessary anxiety—context matters
- Sanitize tools and hands; mirrors themselves do not sterilize jewelry or tissue

## Cross-Links

**Products:** None mapped yet

**Ingredients:** None

**Healing Stages:** `late-healing`, `mature-piercing`, `late-healing`

**Problems:** `jewelry-quality-issue`, `embedded-jewelry`, `snagging`

---

# Piercing Aftercare Kit

**Data Source**

`data/product-categories/piercing-aftercare-kit.yaml`

**Research**

`research/product-categories/piercing-aftercare-kit_research.md`

## Summary

Piercing aftercare kits combine multiple products—often saline spray, gauze, and instructions—into one retail package. Kits vary widely in quality; bundled items may include additives or tools not aligned with APP guidance. PiercingConnect evaluates kit components individually rather than assuming bundle safety from packaging.

## Classification

| Field | Value |
|-------|-------|
| Type | `kit-bundle` |
| Primary Use | Bundle aftercare supplies for new piercing clients or retail gifting. |
| Affiliate Potential | `high` |
| Buyer Intent | `post-piercing-setup` |

## Safety Notes

- Review every item inside a kit; bundled antiseptics or oils may conflict with APP aftercare
- Kits from piercing studios selected by a piercer differ from unverified marketplace bundles
- Instructions in kits are not a substitute for in-person piercer aftercare guidance

## Cross-Links

**Products:** `neilmed-piercing-aftercare-fine-mist`, `easypiercing-saline-solution-50ml`, `recovery-sterile-saline-wash-7-4oz`

**Ingredients:** `sterile-water`, `sodium-chloride-0.9-percent`, `sea-salt`

**Healing Stages:** `fresh-piercing`, `early-healing`, `active-healing`

**Problems:** `undercleaning`, `overcleaning`, `allergic-reaction`, `jewelry-quality-issue`

---

# Piercing Pillow

**Data Source**

`data/product-categories/piercing-pillow.yaml`

**Research**

`research/product-categories/piercing-pillow_research.md`

## Summary

Piercing pillows and travel pillows with ear cutouts are comfort accessories marketed to reduce pressure on healing ear piercings during sleep. APP aftercare advises avoiding sleeping on piercings; pressure-reduction pillows may support that goal but do not replace proper jewelry, aftercare, or professional assessment of persistent irritation.

## Classification

| Field | Value |
|-------|-------|
| Type | `comfort-aid` |
| Primary Use | Reduce sleeping pressure on ear piercings using a donut or cutout pillow design. |
| Affiliate Potential | `moderate` |
| Buyer Intent | `comfort-support` |

## Safety Notes

- Comfort accessory only; does not heal piercings or prevent all irritation
- Continue sterile saline aftercare and avoid pressure when possible
- Persistent bumps or pain require piercer evaluation, not only pillow changes

## Cross-Links

**Products:** None mapped yet

**Ingredients:** None

**Healing Stages:** `fresh-piercing`, `early-healing`, `active-healing`, `irritated-piercing`

**Problems:** `sleeping-irritation`, `pressure-irritation`, `irritation-bump`, `migration`

---

# Saline Spray

**Data Source**

`data/product-categories/saline-spray.yaml`

**Research**

`research/product-categories/saline-spray_research.md`

## Summary

Saline spray is the parent commercial category for salt-water-based piercing aftercare mists and sprays. It includes APP-aligned sterile isotonic products and formulations with sea salt, enzymes, or other additives that require separate ingredient review. PiercingConnect treats sterile isotonic saline as the professional baseline while cataloging broader saline sprays for comparison content.

## Classification

| Field | Value |
|-------|-------|
| Type | `aftercare-solution` |
| Primary Use | Broad category for saline-based piercing aftercare sprays including sterile and non-sterile formulations. |
| Affiliate Potential | `high` |
| Buyer Intent | `comparison-research` |

## Safety Notes

- Not all saline sprays are equivalent—review sterility, additives, and APP alignment per product
- Sea-salt or enzyme formulas may differ from packaged sterile isotonic saline recommendations
- Comparison content must lead with safety and evidence, not affiliate commission

## Cross-Links

**Products:** `neilmed-piercing-aftercare-fine-mist`, `recovery-sterile-saline-wash-7-4oz`, `steri-wash-saline-spray`, `h2ocean-piercing-aftercare-spray`

**Ingredients:** `sterile-water`, `sodium-chloride-0.9-percent`, `sea-salt`, `purified-water`

**Healing Stages:** `fresh-piercing`, `early-healing`, `active-healing`, `late-healing`

**Problems:** `undercleaning`, `overcleaning`, `allergic-reaction`, `dryness`, `infection-concern`

---

# Sterile Gauze

**Data Source**

`data/product-categories/sterile-gauze.yaml`

**Research**

`research/product-categories/sterile-gauze_research.md`

## Summary

Sterile gauze and non-woven sterile pads are disposable materials used to gently pat dry piercings or absorb fluid. APP troubleshooting references clean gauze or paper products for gentle pressure when bleeding occurs. Gauze supports hygiene but is not itself an active aftercare treatment.

## Classification

| Field | Value |
|-------|-------|
| Type | `wound-care` |
| Primary Use | Pat dry or protect piercing area with clean disposable material after rinsing. |
| Affiliate Potential | `moderate` |
| Buyer Intent | `routine-aftercare` |

## Safety Notes

- Use sterile single-use products when possible; do not reuse gauze on healing piercings
- Pat dry gently; avoid fiber snagging on jewelry
- Gauze does not replace saline rinsing or professional evaluation

## Cross-Links

**Products:** None mapped yet

**Ingredients:** None

**Healing Stages:** `fresh-piercing`, `early-healing`, `active-healing`, `late-healing`

**Problems:** `bleeding`, `crusting`, `moisture-irritation`, `infection-concern`

---

# Sterile Saline Spray

**Data Source**

`data/product-categories/sterile-saline-spray.yaml`

**Research**

`research/product-categories/sterile-saline-spray_research.md`

## Summary

Sterile saline sprays deliver 0.9% sodium chloride in sterile water for wound rinsing. APP aftercare guidance recommends packaged sterile saline labeled for wound washing rather than home-mixed solutions. This category covers piercing-branded and pharmacy-style sterile saline sprays when formulation and labeling meet professional aftercare standards.

## Classification

| Field | Value |
|-------|-------|
| Type | `aftercare-solution` |
| Primary Use | Rinse healing piercings with packaged sterile isotonic saline without harsh additives. |
| Affiliate Potential | `high` |
| Buyer Intent | `routine-aftercare` |

## Safety Notes

- Prefer products labeled sterile with simple isotonic saline ingredients when aligned with APP guidance
- Saline rinsing supports cleaning but does not diagnose or treat infection
- Avoid substituting contact lens solution, homemade mixes, or harsh antiseptics

## Cross-Links

**Products:** `neilmed-piercing-aftercare-fine-mist`, `recovery-sterile-saline-wash-7-4oz`, `steri-wash-saline-spray`

**Ingredients:** `sterile-water`, `sodium-chloride-0.9-percent`

**Healing Stages:** `fresh-piercing`, `early-healing`, `active-healing`, `late-healing`

**Problems:** `undercleaning`, `overcleaning`, `infection-concern`, `dryness`, `crusting`

---

# Travel Aftercare Kit

**Data Source**

`data/product-categories/travel-aftercare-kit.yaml`

**Research**

`research/product-categories/travel-aftercare-kit_research.md`

## Summary

Travel aftercare kits package TSA-friendly or small-format aftercare items for clients away from home. Professional aftercare consistency during travel typically centers on portable sterile saline options. Kit quality depends on included products; travel size alone does not establish safety.

## Classification

| Field | Value |
|-------|-------|
| Type | `kit-bundle` |
| Primary Use | Portable aftercare supplies for travel while maintaining saline rinsing routine. |
| Affiliate Potential | `moderate` |
| Buyer Intent | `travel-convenience` |

## Safety Notes

- Confirm travel containers meet airline liquid rules without sacrificing sterility after opening
- Do not skip rinsing routine during travel; small sterile saline formats may help maintain consistency
- Avoid swapping to unfamiliar harsh products simply because they are travel-sized

## Cross-Links

**Products:** `easypiercing-saline-solution-50ml`, `neilmed-piercing-aftercare-fine-mist`

**Ingredients:** `sterile-water`, `sodium-chloride-0.9-percent`

**Healing Stages:** `fresh-piercing`, `early-healing`, `active-healing`, `late-healing`

**Problems:** `undercleaning`, `snagging`, `sleeping-irritation`

---

# Wound Wash

**Data Source**

`data/product-categories/wound-wash.yaml`

**Research**

`research/product-categories/wound-wash_research.md`

## Summary

Wound wash is a retail and pharmacy labeling category for sterile saline products intended to rinse wounds. APP aftercare guidance specifically references sterile saline wound wash for piercing aftercare. In PiercingConnect taxonomy, wound wash overlaps sterile saline spray but emphasizes wound-care shelf positioning and USP-style labeling rather than piercing-branded marketing alone.

## Classification

| Field | Value |
|-------|-------|
| Type | `wound-care` |
| Primary Use | Provide pharmacy-category sterile saline rinsing labeled for wound washing. |
| Affiliate Potential | `high` |
| Buyer Intent | `comparison-research` |

## Safety Notes

- Confirm product is sterile isotonic saline; wound wash labeling alone does not guarantee suitability
- Some wound washes include additives—review individual product ingredients before recommending
- Does not replace professional evaluation when infection concern signs appear

## Cross-Links

**Products:** `neilmed-piercing-aftercare-fine-mist`, `recovery-sterile-saline-wash-7-4oz`, `steri-wash-saline-spray`

**Ingredients:** `sterile-water`, `sodium-chloride-0.9-percent`

**Healing Stages:** `fresh-piercing`, `early-healing`, `active-healing`, `late-healing`

**Problems:** `undercleaning`, `infection-concern`, `overcleaning`, `crusting`

---



# Editorial Notes

All factual changes should be made in the corresponding YAML record first.

Product records in `data/products/` reference a `category` field that maps to these category IDs where applicable. Categories without mapped products remain valid taxonomy placeholders for future catalog expansion.

Sterile isotonic saline spray and wound wash categories overlap in practice; PiercingConnect keeps both for retail positioning and comparison content.

---

# Related Data

- `data/product-categories/`
- `data/products/`
- `data/ingredients/`
- `data/healing-stages/`
- `data/problems/`
- `schemas/product-category.schema.yaml`
- `research/product-categories/`

---

# Status

Current Coverage (12 product categories):

- Compress
- Foam Soap
- Healing Soak
- Jewelry Storage
- Mirror
- Piercing Aftercare Kit
- Piercing Pillow
- Saline Spray
- Sterile Gauze
- Sterile Saline Spray
- Travel Aftercare Kit
- Wound Wash
