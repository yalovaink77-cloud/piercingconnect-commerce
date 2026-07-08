# Ingredient Database

Version: 1.0

Status: Active

---

# Purpose

This document provides human-readable profiles for aftercare ingredients stored in the structured data layer.

The structured data (`data/ingredients/*.yaml`) is the single source of truth.

This document summarizes, explains, and contextualizes those records for editorial use.

**Important:** Ingredient content educates without making treatment claims. Distinguish evidence from marketing. Follow `standards/evidence-policy.md`.

---

# Ingredient Index

| Ingredient | Status | Evidence | APP Alignment | Review |
|-----------|--------|----------|---------------|--------|
| Alcohol | Draft | Strong | Not Recommended | Pending |
| Benzalkonium Chloride | Draft | Moderate | Not Recommended | Pending |
| Hydrogen Peroxide | Draft | Strong | Not Recommended | Pending |
| Hypochlorous Acid | Draft | Limited | Not Addressed | Pending |
| Lysozyme | Draft | Limited | Caution | Pending |
| Polyhexanide (PHMB) | Draft | Moderate | Not Addressed | Pending |
| Preservatives | Draft | Moderate | Caution | Pending |
| Purified Water | Draft | Moderate | Caution | Pending |
| Sea Salt | Draft | Limited | Caution | Pending |
| Sodium Chloride 0.9% | Draft | Strong | Recommended | Pending |
| Sterile Water | Draft | Strong | Recommended | Pending |
| Tea Tree Oil | Draft | Limited | Not Recommended | Pending |

---

# Alcohol

**Data Source**

`data/ingredients/alcohol.yaml`

**Research**

`research/ingredients/alcohol_research.md`

## Summary

Alcohol (ethanol or isopropyl) is used as a disinfectant and solvent in many consumer products. APP aftercare and troubleshooting guidance explicitly advises against cleaning healing piercings with alcohol because it can damage cells, irritate tissue, and delay healing. Alcohol a…

## Classification

| Field | Value |
|-------|-------|
| Type | `irritant` |
| Evidence | `strong` |
| APP Alignment | `not-recommended` |
| Fresh Piercings | `False` |

## Key Benefits (Documented)

- Broad use as surface disinfectant outside of open wound care
- Rapid evaporation in some antiseptic product designs

## Potential Risks

- Tissue irritation and delayed healing
- Burning sensation on broken skin
- Consumer habit of using rubbing alcohol on piercings despite professional guidance


## Cross-Links

**Products:** None linked

**Brands:** `easypiercing-care-lab`

**Problems:** `dryness`, `irritation-bump`, `delayed-healing`, `overcleaning`, `allergic-reaction`

---


# Benzalkonium Chloride

**Data Source**

`data/ingredients/benzalkonium-chloride.yaml`

**Research**

`research/ingredients/benzalkonium-chloride_research.md`

## Summary

Benzalkonium chloride is a quaternary ammonium antiseptic used in some ear care and first-aid products. Inverness Ear Care Solution lists purified water and benzalkonium chloride as ingredients. APP aftercare guidance advises avoiding Bactine and other products containing benzalk…

## Classification

| Field | Value |
|-------|-------|
| Type | `antimicrobial` |
| Evidence | `moderate` |
| APP Alignment | `not-recommended` |
| Fresh Piercings | `caution` |

## Key Benefits (Documented)

- Documented antiseptic use in consumer health products
- Official Inverness formulation for ear piercing aftercare context
- Alternative positioning to alcohol and hydrogen peroxide in some ear care products


## Potential Risks

- Contact irritation or sensitivity
- Prolonged use may irritate healing tissue per APP guidance on BZK products
- Consumer confusion between ear care antiseptic and sterile saline

## Cross-Links

**Products:** `inverness-ear-care-solution`

**Brands:** `inverness-aftercare`

**Problems:** `allergic-reaction`, `dryness`, `infection-concern`, `irritation-bump`

---


# Hydrogen Peroxide

**Data Source**

`data/ingredients/hydrogen-peroxide.yaml`

**Research**

`research/ingredients/hydrogen-peroxide_research.md`

## Summary

Hydrogen peroxide is an oxidizing agent used historically for wound cleaning but is no longer favored for routine open wound care because it may harm healthy tissue and delay healing. APP aftercare guidance advises against hydrogen peroxide on healing piercings. Inverness and oth…

## Classification

| Field | Value |
|-------|-------|
| Type | `oxidizing-agent` |
| Evidence | `strong` |
| APP Alignment | `not-recommended` |
| Fresh Piercings | `False` |

## Key Benefits (Documented)

- Antimicrobial oxidizing activity in surface disinfection contexts

## Potential Risks

- Tissue irritation and delayed healing
- False sense of cleaning while harming healing tissue
- Common DIY misuse on fresh piercings

## Cross-Links

**Products:** None linked

**Brands:** None linked

**Problems:** `dryness`, `irritation-bump`, `delayed-healing`, `overcleaning`, `redness`

---


# Hypochlorous Acid

**Data Source**

`data/ingredients/hypochlorous-acid.yaml`

**Research**

`research/ingredients/hypochlorous-acid_research.md`

## Summary

Hypochlorous acid (HOCl) is a weak acid with antimicrobial properties used in some wound and skin cleansers. Studex Advanced 2-in-1 Aftercare markets a hypochlorous formula; official product labeling lists water, sodium hypochlorite, and phosphoric acid as ingredients. HOCl produ…

## Classification

| Field | Value |
|-------|-------|
| Type | `antimicrobial` |
| Evidence | `limited` |
| APP Alignment | `not-addressed` |
| Fresh Piercings | `caution` |

## Key Benefits (Documented)

- Used in hypochlorous wound and skin cleanser category
- Studex product claims alcohol-free and benzalkonium-chloride-free formulation
- May support cleansing without some traditional harsh antiseptics

## Potential Risks

- Misclassification as equivalent to sterile saline
- Sensitivity or irritation possible in some users
- Marketing claims about healing speed require cautious editorial framing

## Cross-Links

**Products:** `studex-advanced-2-in-1-piercing-aftercare-cleanser`

**Brands:** `studex-aftercare`, `base-laboratories`

**Problems:** `infection-concern`, `dryness`, `allergic-reaction`, `delayed-healing`

---


# Lysozyme

**Data Source**

`data/ingredients/lysozyme.yaml`

**Research**

`research/ingredients/lysozyme_research.md`

## Summary

Lysozyme is a naturally occurring enzyme that breaks down bacterial cell walls and appears in some biological fluids including tears and saliva. H2Ocean piercing aftercare products list lysozyme among ingredients alongside sea salt and purified water. This is a multi-ingredient f…

## Classification

| Field | Value |
|-------|-------|
| Type | `enzyme` |
| Evidence | `limited` |
| APP Alignment | `acceptable-with-caution` |
| Fresh Piercings | `caution` |

## Key Benefits (Documented)

- Known enzymatic activity in biological systems
- Included in established commercial piercing aftercare brand formulations

## Potential Risks

- Additional ingredients beyond isotonic saline may irritate sensitive users
- Marketing may overstate enzymatic benefits for healing

## Cross-Links

**Products:** `h2ocean-piercing-aftercare-spray`

**Brands:** `h2ocean`

**Problems:** `allergic-reaction`, `irritation-bump`, `dryness`

---


# Polyhexanide (PHMB)

**Data Source**

`data/ingredients/polyhexanide-phmb.yaml`

**Research**

`research/ingredients/polyhexanide-phmb_research.md`

## Summary

Polyhexanide (polyhexamethylene biguanide, PHMB) is an antimicrobial agent used in medical device and wound-care contexts. Prontolind piercing aftercare products use a polyhexanide-betaine complex for antimicrobial cleaning. This is not isotonic sterile saline. Professional use i…

## Classification

| Field | Value |
|-------|-------|
| Type | `antimicrobial` |
| Evidence | `moderate` |
| APP Alignment | `not-addressed` |
| Fresh Piercings | `caution` |

## Key Benefits (Documented)

- Established antimicrobial use in medical and cosmetic device categories
- Used in professional piercing aftercare lines in Europe
- Manufacturer documents GMP production and medical device positioning for Prontolind


## Potential Risks

- May cause sensitivity in some individuals
- Misuse as a substitute for saline without professional guidance
- Antimicrobial products may not be appropriate for all piercing types or stages without piercer direction


## Cross-Links

**Products:** `prontolind-spray-75ml`

**Brands:** `prontolind`

**Problems:** `infection-concern`, `irritation-bump`, `allergic-reaction`

---


# Preservatives

**Data Source**

`data/ingredients/preservatives.yaml`

**Research**

`research/ingredients/preservatives_research.md`

## Summary

Preservatives are additives used to prevent microbial growth in multi-use cosmetic and pharmaceutical products. APP aftercare guidance recommends sterile saline wound wash with 0.9% sodium chloride as the primary ingredient and advises avoiding unnecessary additives such as moist…

## Classification

| Field | Value |
|-------|-------|
| Type | `preservative-class` |
| Evidence | `moderate` |
| APP Alignment | `acceptable-with-caution` |
| Fresh Piercings | `caution` |

## Key Benefits (Documented)

- May extend shelf life and reduce contamination risk in non-sterile multi-use products

- Required in many cosmetic formulation categories

## Potential Risks

- Contact sensitization or irritation in susceptible individuals
- Consumers may assume all saline-labeled products are additive-free
- Preserved cosmetic sprays are not interchangeable with sterile wound wash without verification


## Cross-Links

**Products:** `neilmed-piercing-aftercare-fine-mist`, `recovery-sterile-saline-wash-7-4oz`, `steri-wash-saline-spray`, `base-laboratories-piercing-aftercare-spray`

**Brands:** `neilmed`, `recovery-aftercare`, `steri-wash`, `base-laboratories`, `h2ocean`

**Problems:** `allergic-reaction`, `dryness`, `irritation-bump`

---


# Purified Water

**Data Source**

`data/ingredients/purified-water.yaml`

**Research**

`research/ingredients/purified-water_research.md`

## Summary

Purified water is water that has been treated to remove impurities but is not necessarily labeled or validated as sterile for wound use. It appears in cosmetic and aftercare formulations as a base solvent. APP guidance prefers packaged sterile saline for piercing aftercare; purif…

## Classification

| Field | Value |
|-------|-------|
| Type | `solvent-base` |
| Evidence | `moderate` |
| APP Alignment | `acceptable-with-caution` |
| Fresh Piercings | `caution` |

## Key Benefits (Documented)

- Common pharmaceutical and cosmetic diluent
- Allows formulation of multi-ingredient products

## Potential Risks

- Mislabeling or consumer assumption that all water-based sprays are sterile saline

- Combined with antiseptics or botanicals that may irritate fresh piercings

## Cross-Links

**Products:** `h2ocean-piercing-aftercare-spray`, `inverness-ear-care-solution`

**Brands:** `h2ocean`, `inverness-aftercare`

**Problems:** `dryness`, `allergic-reaction`, `infection-concern`

---


# Sea Salt

**Data Source**

`data/ingredients/sea-salt.yaml`

**Research**

`research/ingredients/sea-salt_research.md`

## Summary

Sea salt is sodium chloride derived from evaporated seawater and may contain trace minerals. APP previously described measured non-iodized sea salt soaks as a regional alternative when sterile saline is unavailable, but current APP guidance strongly encourages packaged sterile sa…

## Classification

| Field | Value |
|-------|-------|
| Type | `active-salt` |
| Evidence | `limited` |
| APP Alignment | `acceptable-with-caution` |
| Fresh Piercings | `caution` |

## Key Benefits (Documented)

- Measured non-iodized soaks have been described as a fallback when sterile saline is unavailable (regional APP guidance)

- Familiar consumer ingredient in aftercare discourse

## Potential Risks

- Overly strong soaks may irritate tissue and delay healing
- Not interchangeable with sterile pharmaceutical wound wash without validation

## Cross-Links

**Products:** `h2ocean-piercing-aftercare-spray`

**Brands:** `h2ocean`

**Problems:** `dryness`, `overcleaning`, `irritation-bump`, `delayed-healing`

---


# Sodium Chloride 0.9%

**Data Source**

`data/ingredients/sodium-chloride-0.9-percent.yaml`

**Research**

`research/ingredients/sodium-chloride-0.9-percent_research.md`

## Summary

Sodium chloride at 0.9% concentration produces isotonic saline (normal saline), matching the approximate salt concentration of human body fluids. APP aftercare guidance recommends packaged sterile saline labeled for wound wash with 0.9% sodium chloride as the primary ingredient f…

## Classification

| Field | Value |
|-------|-------|
| Type | `active-salt` |
| Evidence | `strong` |
| APP Alignment | `recommended` |
| Fresh Piercings | `True` |

## Key Benefits (Documented)

- Isotonic concentration may support gentle rinsing without strong osmotic irritation

- Simple two-ingredient saline aligns with APP preferred aftercare
- Widely available in pharmacy wound-wash products

## Potential Risks

- DIY salt mixes frequently exceed safe concentration per APP
- Confusion with contact lens saline, nasal spray, or eye drops which are not interchangeable


## Cross-Links

**Products:** `neilmed-piercing-aftercare-fine-mist`, `steri-wash-saline-spray`, `recovery-sterile-saline-wash-7-4oz`, `easypiercing-saline-solution-50ml`

**Brands:** `neilmed`, `steri-wash`, `recovery-aftercare`, `easypiercing-care-lab`

**Problems:** `irritation-bump`, `infection-concern`, `crusting`, `overcleaning`, `undercleaning`, …

---


# Sterile Water

**Data Source**

`data/ingredients/sterile-water.yaml`

**Research**

`research/ingredients/sterile-water_research.md`

## Summary

Sterile water is water that has been processed to meet sterility standards for medical or pharmaceutical use. In piercing aftercare products, it commonly serves as the solvent base for isotonic saline sprays. APP guidance favors packaged sterile saline wound wash rather than home…

## Classification

| Field | Value |
|-------|-------|
| Type | `solvent-base` |
| Evidence | `strong` |
| APP Alignment | `recommended` |
| Fresh Piercings | `True` |

## Key Benefits (Documented)

- Provides a sterile diluent for isotonic saline formulations
- Supports simple, additive-free wound rinsing when paired with 0.9% sodium chloride

- Widely used in pharmaceutical wound-wash products

## Potential Risks

- Using non-sterile water on fresh piercings may introduce bacteria
- Confusion with purified or tap water in DIY mixes

## Cross-Links

**Products:** `neilmed-piercing-aftercare-fine-mist`, `steri-wash-saline-spray`, `recovery-sterile-saline-wash-7-4oz`

**Brands:** `neilmed`, `steri-wash`, `recovery-aftercare`

**Problems:** `overcleaning`, `undercleaning`, `infection-concern`, `dryness`

---


# Tea Tree Oil

**Data Source**

`data/ingredients/tea-tree-oil.yaml`

**Research**

`research/ingredients/tea-tree-oil_research.md`

## Summary

Tea tree oil is an essential oil with antimicrobial properties marketed in some piercing and skincare products. Base Laboratories Piercing Aftercare Spray lists tea tree oil among multiple additives in a saline-based spray. APP troubleshooting and aftercare guidance does not reco…

## Classification

| Field | Value |
|-------|-------|
| Type | `essential-oil` |
| Evidence | `limited` |
| APP Alignment | `not-recommended` |
| Fresh Piercings | `False` |

## Key Benefits (Documented)

- Documented antimicrobial properties in laboratory contexts
- Common consumer recognition in aftercare marketing

## Potential Risks

- Contact dermatitis or sensitization
- Irritation when applied undiluted or too frequently on fresh piercings
- False reassurance for bumps that require irritation source removal or medical care


## Cross-Links

**Products:** `base-laboratories-piercing-aftercare-spray`

**Brands:** `base-laboratories`

**Problems:** `irritation-bump`, `allergic-reaction`, `dryness`, `overcleaning`

---



# Editorial Notes

Ingredient profiles summarize structured data stored in the `data/ingredients/` directory.

All factual changes should be made in the corresponding YAML record first.

The Markdown documentation should always reflect the structured data.

APP alignment reflects Association of Professional Piercers aftercare guidance reviewed during initial drafting. Individual piercer recommendations may vary by region.

---

# Related Data

- `data/ingredients/`
- `data/products/`
- `data/brands/`
- `data/problems/`
- `schemas/ingredient.schema.yaml`
- `research/ingredients/`

---

# Status

Current Coverage (12 ingredients):

- Alcohol
- Benzalkonium Chloride
- Hydrogen Peroxide
- Hypochlorous Acid
- Lysozyme
- Polyhexanide (PHMB)
- Preservatives
- Purified Water
- Sea Salt
- Sodium Chloride 0.9%
- Sterile Water
- Tea Tree Oil

Next phase:

- Individual preservative compound records
- Ingredient-to-product validation scripts
- PC Media Engine ingredient explainer templates
