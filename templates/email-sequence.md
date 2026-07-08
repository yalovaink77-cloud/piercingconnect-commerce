# Template: Email Sequence

Version: 1.0

Status: Active

Type: blueprint

---

## Purpose

Reusable section structure for multi-email nurture sequences. Each email is a section block — PCME generates copy per step.

---

## Required Knowledge Entities

| Entity | Path |
|--------|------|
| Keyword Cluster | `data/keywords/{{keyword_cluster.id}}.yaml` |
| Healing Stage (1+) | Sequence timing context |
| Topical entity (one required) | Product **or** Brand **or** Problem **or** Piercing Type |

---

## Publishing Targets

- Email

---

## Template Variables

- `{{keyword_cluster.primary_keyword}}`
- `{{healing_stage.name}}`
- `{{product.name}}`
- `{{brand.name}}`
- `{{problem.name}}`
- `{{piercing_type.name}}`
- `{{subject_line}}`
- `{{preheader}}`
- `{{affiliate_disclosure}}`
- `{{safety_disclaimer}}`
- `{{cta}}`
- `{{unsubscribe}}`

---

## Sections

### 1. Sequence Metadata

- Sequence name from `{{keyword_cluster.id}}`
- Topic entity type and ID
- Target healing stages for send timing
- `{{keyword_cluster.funnel_stage}}`

### 2. Email 1 — Welcome / Problem Acknowledgment

- `{{subject_line}}`
- `{{preheader}}`
- Hook from `{{keyword_cluster.user_problem}}`
- `{{safety_disclaimer}}` on problem sequences
- Soft `{{cta}}` — no hard sell on email 1 for urgent clusters

### 3. Email 2 — Education Block

- Core entity teaching: aftercare notes, problem actions, or product criteria
- Entity field lists only — PCME expands

### 4. Email 3 — Practical Steps

- Step list from piercing type aftercare or problem recommended actions
- Ingredient/product context if loaded

### 5. Email 4 — Product or Brand Introduction (Conditional)

- `{{product.name}}` or `{{brand.name}}`
- Trust score and safety notes before CTA
- `{{affiliate_disclosure}}`

### 6. Email 5 — Summary and Next Steps

- Recap key entity points
- When to see piercer / professional help
- Primary `{{cta}}`

### 7. Sequence Compliance Footer

- `{{affiliate_disclosure}}`
- `{{safety_disclaimer}}`
- `{{unsubscribe}}`

### 8. Sources and Review

- Entity sources per email
- `review.status`
