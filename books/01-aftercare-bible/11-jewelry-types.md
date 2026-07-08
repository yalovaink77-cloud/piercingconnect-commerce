# Jewelry Types

Version: 1.0

Status: Active

---

# Purpose

This document provides human-readable profiles for jewelry types and construction styles in the PiercingConnect knowledge graph.

The structured data (`data/jewelry-types/*.yaml`) is the single source of truth.

**Important:** Jewelry suitability depends on placement, gauge, length, material grade, finish, and professional fit—not style alone. APP initial jewelry guidance distinguishes internally threaded and threadless construction from externally threaded posts. Follow `standards/evidence-policy.md`. No medical diagnosis.

---

# Jewelry Type Index

| Jewelry Type | Form | APP Alignment | Fresh Piercings | Status | Review |
|--------------|------|---------------|---------------|--------|--------|
| Captive Bead Ring | `ring-captive` | Caution | Caution | Draft | Pending |
| Circular Barbell | `barbell-circular` | Recommended | Yes | Draft | Pending |
| Clicker Ring | `ring-clicker` | Caution | Caution | Draft | Pending |
| Curved Barbell | `barbell-curved` | Recommended | Yes | Draft | Pending |
| Externally Threaded Jewelry | `construction-external-thread` | Not Recommended | No | Draft | Pending |
| Flat-Back Labret | `labret-post` | Recommended | Yes | Draft | Pending |
| Internally Threaded Jewelry | `construction-internal-thread` | Recommended | Yes | Draft | Pending |
| L-Bend Nose Jewelry | `nostril-l-bend` | Caution | Caution | Draft | Pending |
| Nose Stud | `nostril-stud` | Recommended | Yes | Draft | Pending |
| Nostril Screw | `nostril-screw` | Recommended | Yes | Draft | Pending |
| Seamless Ring | `ring-seamless` | Caution | Caution | Draft | Pending |
| Straight Barbell | `barbell-straight` | Recommended | Yes | Draft | Pending |
| Threadless Jewelry | `construction-threadless` | Recommended | Yes | Draft | Pending |

---

# Threading Guidance (APP Summary)

| Construction | Fresh Piercings | Notes |
|--------------|-----------------|-------|
| Internally threaded | Preferred | Smooth post passes through tissue; threads on removable end |
| Threadless (press-fit) | Acceptable | Pin coupling; no screw threads at connection |
| Externally threaded | Not recommended | Thread ridges on post may scrape tissue |

See `internally-threaded-jewelry`, `threadless-jewelry`, and `externally-threaded-jewelry` records for full cross-links.

---

# Captive Bead Ring

**Data Source**

`data/jewelry-types/captive-bead-ring.yaml`

**Research**

`research/jewelry-types/captive-bead-ring_research.md`

## Summary

A round ring that holds a captive bead or ball under tension without threads. APP initial jewelry guidance states rings are best for some areas and bars for others; captive bead rings may be selected for certain initial piercings when diameter, gauge, and quality meet professional standards. Quality rings should be annealed per APP.

## Classification

| Field | Value |
|-------|-------|
| Form | `ring-captive` |
| APP Alignment | `acceptable-with-caution` |
| Fresh Piercings | `caution` |
| Healed Piercings | `true` |

## Risks

- Bead may pop out if ring tension is incorrect, risking channel closure or swallowing in oral areas
- Opening or closing rings with pliers during healing may damage metal and tissue
- Diameter or gauge inappropriate for anatomy may contribute to migration per APP

## Aftercare Considerations

- APP notes quality rings are annealed for pliability; professional insertion and adjustment preferred
- If bead is loose, see piercer for tension adjustment or replacement per APP
- Do not open or close captive rings at home during early healing

## Cross-Links

**Piercing Types:** `septum`, `lobe`, `upper-lobe`, `helix`, `nostril`

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`, `surgical-steel`

**Problems:** `snagging`, `migration`, `jewelry-quality-issue`, `sleeping-irritation`, `irritation-bump`

---

# Circular Barbell

**Data Source**

`data/jewelry-types/circular-barbell.yaml`

**Research**

`research/jewelry-types/circular-barbell_research.md`

## Summary

A horseshoe-shaped bar with two removable ends, also called a circular barbell. APP notes rings are best for some areas and bars for others; circular barbells are commonly used for septum and smiley piercings when diameter and gauge suit anatomy.

## Classification

| Field | Value |
|-------|-------|
| Form | `barbell-circular` |
| APP Alignment | `recommended` |
| Fresh Piercings | `true` |
| Healed Piercings | `true` |

## Risks

- Diameter too small may compress tissue; too large may increase movement and snagging
- Ends that loosen may fall out or expose sharp threads
- Oral-adjacent placements may contact teeth or gums if oversized

## Aftercare Considerations

- Spray sterile saline for external cleaning per APP body aftercare
- Oral-adjacent piercings follow APP oral aftercare where applicable
- Check end tightness daily with clean hands for threaded styles

## Cross-Links

**Piercing Types:** `septum`, `smiley`

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`, `surgical-steel`

**Problems:** `snagging`, `pressure-irritation`, `jewelry-quality-issue`, `irritation-bump`, `swelling`

---

# Clicker Ring

**Data Source**

`data/jewelry-types/clicker.yaml`

**Research**

`research/jewelry-types/clicker_research.md`

## Summary

A hinged ring that closes with a click mechanism, popular for septum and ear cartilage once healed. APP initial jewelry guidance emphasizes fit, finish, and material; hinged clickers introduce a mechanical closure that must be smooth and secure. Many piercers discuss clickers after healing rather than as first jewelry.

## Classification

| Field | Value |
|-------|-------|
| Form | `ring-clicker` |
| APP Alignment | `acceptable-with-caution` |
| Fresh Piercings | `caution` |
| Healed Piercings | `true` |

## Risks

- Hinge gaps or rough closure points may irritate tissue
- Low-quality clickers may pop open and snag or fall out
- Decorative elements may add weight or catch on hair and masks

## Aftercare Considerations

- Confirm piercer approves clicker timing for your healing stage
- Keep hinge area clean with sterile saline without forcing mechanism open repeatedly
- Check closure security daily if piercer advises; seek adjustment if ring opens spontaneously

## Cross-Links

**Piercing Types:** `septum`, `helix`, `daith`, `lobe`, `conch`

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`

**Problems:** `snagging`, `jewelry-quality-issue`, `irritation-bump`, `pressure-irritation`

---

# Curved Barbell

**Data Source**

`data/jewelry-types/curved-barbell.yaml`

**Research**

`research/jewelry-types/curved-barbell_research.md`

## Summary

A curved bar with two removable ends, shaped to follow anatomy in placements such as navel, eyebrow, and some lip piercings. APP guidance requires jewelry style suited to placement; curved bars are among the forms professional piercers select when straight or ring styles are less appropriate.

## Classification

| Field | Value |
|-------|-------|
| Form | `barbell-curved` |
| APP Alignment | `recommended` |
| Fresh Piercings | `true` |
| Healed Piercings | `true` |

## Risks

- Incorrect curve radius may cause pressure or migration in surface-adjacent placements
- Snagging on waistbands or clothing common in navel piercings
- Too-tight curve may compress tissue; too-open curve may increase movement

## Aftercare Considerations

- Spray sterile saline once or twice daily per APP body aftercare
- Protect navel piercings from waistband friction and moisture buildup
- Minimize jewelry movement; piercer should assess fit early for eyebrow and bridge placements

## Cross-Links

**Piercing Types:** `navel`, `eyebrow`, `vertical-labret`, `bridge`

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`, `surgical-steel`

**Problems:** `snagging`, `migration`, `pressure-irritation`, `moisture-irritation`, `jewelry-quality-issue`

---

# Externally Threaded Jewelry

**Data Source**

`data/jewelry-types/externally-threaded-jewelry.yaml`

**Research**

`research/jewelry-types/externally-threaded-jewelry_research.md`

## Summary

Externally threaded jewelry has screw threads cut into the post itself, so the comparatively rough thread surface may pass through tissue during insertion and removal. APP initial jewelry guidance contrasts this with internally threaded jewelry, which is part of the APP standard for initial piercing jewelry.

## Classification

| Field | Value |
|-------|-------|
| Form | `construction-external-thread` |
| APP Alignment | `not-recommended` |
| Fresh Piercings | `false` |
| Healed Piercings | `caution` |

## Risks

- Thread ridges may scrape healing tissue during insertion and jewelry changes per APP
- Common in low-cost marketplace body jewelry with poor polish
- May combine with non-implant-grade metals and plated surfaces

## Aftercare Considerations

- APP favors internally threaded or threadless jewelry for fresh piercings—ask piercer to replace externally threaded jewelry if present
- Do not purchase externally threaded jewelry for unhealed piercings
- If already inserted, avoid unnecessary removal; seek professional assessment

## Cross-Links

**Piercing Types:** `helix`, `forward-helix`, `flat`, `conch`, `tragus`, `anti-tragus` (+17 more)

**Materials:** `mystery-metal`, `surgical-steel`, `plated-jewelry`, `acrylic`

**Problems:** `jewelry-quality-issue`, `irritation-bump`, `delayed-healing`, `infection-concern`, `allergic-reaction`

---

# Flat-Back Labret

**Data Source**

`data/jewelry-types/flat-back-labret.yaml`

**Research**

`research/jewelry-types/flat-back-labret_research.md`

## Summary

A labret-style post with a flat disk on the interior side and a removable decorative or plain end on the exterior. APP initial jewelry guidance favors styles suited to placement; flat-back labret posts are widely used for ear cartilage, nostril, and lip piercings when length, gauge, and threading meet professional standards.

## Classification

| Field | Value |
|-------|-------|
| Form | `labret-post` |
| APP Alignment | `recommended` |
| Fresh Piercings | `true` |
| Healed Piercings | `true` |

## Risks

- Post too short may contribute to embedding when swelling is present
- Post too long may catch on hair, masks, or bedding and cause trauma
- Externally threaded posts may scrape tissue during insertion or end changes

## Aftercare Considerations

- Spray sterile saline labeled for wound wash; avoid rotating jewelry during cleaning per APP body aftercare
- Check threaded end tightness daily with clean hands if jewelry uses screw-on ends per APP
- Return to piercer for downsizing when initial swelling subsides; timing varies individually

## Cross-Links

**Piercing Types:** `helix`, `forward-helix`, `flat`, `conch`, `tragus`, `anti-tragus` (+13 more)

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`, `surgical-steel`

**Problems:** `embedded-jewelry`, `pressure-irritation`, `snagging`, `jewelry-quality-issue`, `irritation-bump`

---

# Internally Threaded Jewelry

**Data Source**

`data/jewelry-types/internally-threaded-jewelry.yaml`

**Research**

`research/jewelry-types/internally-threaded-jewelry_research.md`

## Summary

Internally threaded jewelry places screw threads inside the removable end, leaving the post that passes through tissue smooth. APP initial jewelry guidance states internally threaded jewelry is part of the APP standard for initial piercing jewelry because it avoids scraping tissue with external thread ridges.

## Classification

| Field | Value |
|-------|-------|
| Form | `construction-internal-thread` |
| APP Alignment | `recommended` |
| Fresh Piercings | `true` |
| Healed Piercings | `true` |

## Risks

- Cross-threading during end attachment may damage threads and leave gaps for bacteria
- Loose ends may fall out if threads are defective—check tightness daily per APP
- Thread gaps where attachment does not seat fully may harbor debris

## Aftercare Considerations

- Check threaded end tightness daily with clean hands per APP
- Spray sterile saline without rotating post unnecessarily
- See piercer if end loosens repeatedly—may indicate defective piece per APP

## Cross-Links

**Piercing Types:** `helix`, `forward-helix`, `flat`, `conch`, `tragus`, `anti-tragus` (+19 more)

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`, `surgical-steel`

**Problems:** `jewelry-quality-issue`, `irritation-bump`, `infection-concern`, `embedded-jewelry`

---

# L-Bend Nose Jewelry

**Data Source**

`data/jewelry-types/l-bend.yaml`

**Research**

`research/jewelry-types/l-bend_research.md`

## Summary

L-bend nose jewelry uses a 90-degree bend on the interior tail for nostril retention. APP initial jewelry guidance highlights nostril screw as a placement-specific style; L-bend variants appear in professional studios but suitability for initial healing depends on anatomy, fit, and piercer practice. Not interchangeable with fashion nose studs.

## Classification

| Field | Value |
|-------|-------|
| Form | `nostril-l-bend` |
| APP Alignment | `acceptable-with-caution` |
| Fresh Piercings | `caution` |
| Healed Piercings | `true` |

## Risks

- Bend may rotate or slide more than screw profile in some anatomies
- Insertion may require passing bend through channel, increasing trauma if attempted at home
- Thin or low-quality wire may bend permanently and create rough surfaces

## Aftercare Considerations

- Follow piercer-specific guidance on L-bend versus flat-back or screw for initial wear
- Spray sterile saline without twisting jewelry
- Avoid blowing nose forcefully while jewelry is tender

## Cross-Links

**Piercing Types:** `nostril`, `high-nostril`

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`, `surgical-steel`

**Problems:** `irritation-bump`, `jewelry-quality-issue`, `embedded-jewelry`, `pressure-irritation`

---

# Nose Stud

**Data Source**

`data/jewelry-types/nose-stud.yaml`

**Research**

`research/jewelry-types/nose-stud_research.md`

## Summary

A nostril stud is a general term for small post-style nose jewelry with a decorative face and an interior retention mechanism. APP initial jewelry guidance references specialty jewelry such as nostril screws for specific placements; flat-back labret posts and nostril-appropriate studs are commonly used for initial nostril piercings when professionally fitted.

## Classification

| Field | Value |
|-------|-------|
| Form | `nostril-stud` |
| APP Alignment | `recommended` |
| Fresh Piercings | `true` |
| Healed Piercings | `true` |

## Risks

- Butterfly-back or improper retention may irritate nostril tissue
- Post length too short may embed during swelling
- Decorative top larger than piercing angle may shift and irritate

## Aftercare Considerations

- Spray sterile saline once or twice daily per APP body aftercare
- Avoid makeup, skin care, and nose blowing that deposits product on jewelry
- Return to piercer for downsizing when swelling subsides

## Cross-Links

**Piercing Types:** `nostril`, `high-nostril`

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`, `surgical-steel`

**Problems:** `embedded-jewelry`, `irritation-bump`, `jewelry-quality-issue`, `swelling`, `pressure-irritation`

---

# Nostril Screw

**Data Source**

`data/jewelry-types/nostril-screw.yaml`

**Research**

`research/jewelry-types/nostril-screw_research.md`

## Summary

A nostril screw is specialty nose jewelry with a curved or bent tail that rests inside the nostril without a separate backing. APP initial jewelry guidance explicitly lists specialty jewelry such as a nostril screw among styles suited to specific placements when material and finish meet professional standards.

## Classification

| Field | Value |
|-------|-------|
| Form | `nostril-screw` |
| APP Alignment | `recommended` |
| Fresh Piercings | `true` |
| Healed Piercings | `true` |

## Risks

- Incorrect bend profile may not suit individual nostril shape and may shift
- Rough screw bend or post may irritate internal nostril tissue
- Inserting or removing screw profile may traumatize channel if done during healing

## Aftercare Considerations

- Professional insertion and downsizing only during early healing
- Spray sterile saline; avoid rotating or twisting screw during cleaning
- Keep area free of makeup and harsh nose products

## Cross-Links

**Piercing Types:** `nostril`, `high-nostril`

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`, `surgical-steel`

**Problems:** `irritation-bump`, `embedded-jewelry`, `jewelry-quality-issue`, `migration`, `swelling`

---

# Seamless Ring

**Data Source**

`data/jewelry-types/seamless-ring.yaml`

**Research**

`research/jewelry-types/seamless-ring_research.md`

## Summary

A continuous ring without a captive bead, sometimes with a slight hinge or weld seam depending on design. APP discusses ring styles for appropriate placements; seamless rings are more commonly discussed for healed piercings when professional fit is confirmed. Initial use depends on piercing type and piercer selection.

## Classification

| Field | Value |
|-------|-------|
| Form | `ring-seamless` |
| APP Alignment | `acceptable-with-caution` |
| Fresh Piercings | `caution` |
| Healed Piercings | `true` |

## Risks

- Seam or hinge points may create rough areas if quality is low
- Inserting seamless rings may require twisting through tissue, increasing trauma if done improperly
- Snagging on hair, clothing, or bedding

## Aftercare Considerations

- Professional installation strongly preferred; do not self-insert during healing
- Spray sterile saline without unnecessary rotation
- See piercer if ring catches frequently or fit feels tight as swelling changes

## Cross-Links

**Piercing Types:** `lobe`, `upper-lobe`, `helix`, `septum`, `nostril`

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`, `surgical-steel`

**Problems:** `snagging`, `migration`, `jewelry-quality-issue`, `sleeping-irritation`, `pressure-irritation`

---

# Straight Barbell

**Data Source**

`data/jewelry-types/straight-barbell.yaml`

**Research**

`research/jewelry-types/straight-barbell_research.md`

## Summary

A straight bar with removable ends on both sides. APP initial jewelry guidance notes jewelry must be of a style suited to build and placement; straight barbells are commonly selected for tongue and nipple piercings when length accommodates swelling.

## Classification

| Field | Value |
|-------|-------|
| Form | `barbell-straight` |
| APP Alignment | `recommended` |
| Fresh Piercings | `true` |
| Healed Piercings | `true` |

## Risks

- Excessively long barbells in oral piercings may damage teeth and gums per APP oral guidance
- Too-short bars may embed as swelling resolves
- Externally threaded bars may pass rough threads through tissue

## Aftercare Considerations

- Oral piercings may use alcohol-free antiseptic mouthwash 4–5 times daily per APP oral guidance
- Piercer should downsize oral barbells after initial swelling; timing varies
- Check end tightness daily with clean hands per APP threading guidance

## Cross-Links

**Piercing Types:** `tongue`, `nipple`

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`, `surgical-steel`

**Problems:** `pressure-irritation`, `embedded-jewelry`, `jewelry-quality-issue`, `snagging`, `swelling`

---

# Threadless Jewelry

**Data Source**

`data/jewelry-types/threadless-jewelry.yaml`

**Research**

`research/jewelry-types/threadless-jewelry_research.md`

## Summary

Threadless or press-fit jewelry uses a pin coupling on the decorative end with no screw threads at the connection. APP initial jewelry guidance lists threadless jewelry as an acceptable alternative to internally threaded jewelry because the post passing through tissue can remain smooth.

## Classification

| Field | Value |
|-------|-------|
| Form | `construction-threadless` |
| APP Alignment | `recommended` |
| Fresh Piercings | `true` |
| Healed Piercings | `true` |

## Risks

- Improper pin bend tension may allow end to pop out
- Forcing ends on or off may scratch post or irritate tissue
- Mixing post and end brands without piercer verification may fit poorly

## Aftercare Considerations

- Do not remove or swap threadless ends during early healing without piercer guidance
- Spray sterile saline without twisting or pulling on decorative end
- See piercer if end feels loose or detaches; APP advises checking closures daily for threaded styles—follow piercer direction for threadless

## Cross-Links

**Piercing Types:** `helix`, `forward-helix`, `flat`, `conch`, `tragus`, `anti-tragus` (+13 more)

**Materials:** `implant-grade-titanium`, `niobium`, `solid-14k-gold`, `surgical-steel`

**Problems:** `jewelry-quality-issue`, `snagging`, `embedded-jewelry`, `irritation-bump`

---



# Editorial Notes

All factual changes should be made in the corresponding YAML record first.

Jewelry **form** (labret, barbell, ring) and **construction** (threading type) are separate taxonomy concepts. A flat-back labret may be internally threaded or threadless; externally threaded posts are discouraged for fresh piercings per APP.

Piercing type records in `data/piercing-types/` remain the canonical placement-specific records. Jewelry type records describe reusable forms and construction standards.

---

# Related Data

- `data/jewelry-types/`
- `data/materials/`
- `data/piercing-types/`
- `data/problems/`
- `schemas/jewelry-type.schema.yaml`
- `research/jewelry-types/`

---

# Status

Current Coverage (13 jewelry types):

- Captive Bead Ring
- Circular Barbell
- Clicker Ring
- Curved Barbell
- Externally Threaded Jewelry
- Flat-Back Labret
- Internally Threaded Jewelry
- L-Bend Nose Jewelry
- Nose Stud
- Nostril Screw
- Seamless Ring
- Straight Barbell
- Threadless Jewelry
