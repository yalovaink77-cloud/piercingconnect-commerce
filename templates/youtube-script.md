# Template: YouTube Script

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for YouTube video scripts. PCME generates spoken prose from entity fields per timed section.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Keyword Cluster | `data/keywords/{{keyword_cluster.id}}.yaml` |
| Healing Stage (1+) | Timeline and stage context |
| Focal entity (by script type) | Piercing Type, Problem, Product, Brand, or Ingredient |

---

## Publishing Targets

- YouTube
- WordPress (embedded video companion post)

---

## Template Variables

- `{{keyword_cluster.primary_keyword}}`
- `{{video_title}}`
- `{{video_description}}`
- `{{piercing_type.name}}`
- `{{problem.name}}`
- `{{product.name}}`
- `{{brand.name}}`
- `{{ingredient.name}}`
- `{{healing_stage.name}}`
- `{{safety_disclaimer}}`
- `{{affiliate_disclosure}}`
- `{{cta}}`
- `{{chapter_timestamps}}`

---

## Sections

### 1. Video Metadata

- `{{video_title}}` from keyword cluster + focal entity
- `{{video_description}}` — SEO block for YouTube
- `{{keyword_cluster.primary_keyword}}`
- Target length estimate (PCME parameter — not stored as article)

### 2. Hook (0:00–0:30)

- Open with `{{keyword_cluster.user_problem}}`
- Promise what viewer will learn — from entity scope only

### 3. Introduction (0:30–1:30)

- Channel trust framing
- `{{safety_disclaimer}}` for problem or aftercare scripts
- What entities / sources inform the video

### 4. Main Content Blocks (repeat per topic)

Block structure per subtopic:

- **Section title** — from entity field group name
- **Talking points** — bullet list mapped to YAML fields (aftercare notes, symptoms, ingredients)
- **On-screen text notes** — key terms for editor
- **B-roll / visual notes** — concept keywords only

Suggested block order by script type:

- **Aftercare:** anatomy → routine → jewelry → problems → products
- **Problem:** overview → causes → actions → avoid → seek help
- **Product review:** summary → ingredients → trust → verdict

### 5. Healing Timeline Section (When Applicable)

- `{{healing_stage.name}}` sequence
- Cautious language from entity timeframes

### 6. Product or Brand Mention (Conditional)

- `{{product.name}}` or `{{brand.name}}`
- Trust and ingredient context before recommendation
- `{{affiliate_disclosure}}`

### 7. Recap

- 3-point summary from entity key lists

### 8. CTA and Outro

- `{{cta}}` — subscribe, piercer consultation, full article link
- `{{chapter_timestamps}}` for description field

### 9. Pinned Comment Structure

- Safety reminder
- Link to full problem guide or aftercare guide URL

### 10. Sources and Review

- Entity sources
- `review.status`
