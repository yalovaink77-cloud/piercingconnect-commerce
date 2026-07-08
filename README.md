# PiercingConnect Commercial Knowledge Core

Version: 1.0

Status: Active

---

## What This Repository Is

This repository is the **source of truth** for PiercingConnect structured piercing commerce knowledge — brands, products, aftercare guidance, taxonomy, templates, and publishing assets.

It is **not a blog**. Published articles and social content are downstream outputs generated from this knowledge core.

---

## Quick Start

1. Read [`docs/ai-developer-guide.md`](docs/ai-developer-guide.md) before making changes.
2. Review [`docs/architecture.md`](docs/architecture.md) for layer responsibilities.
3. Structured records live in [`data/`](data/) and must conform to [`schemas/`](schemas/).
4. Human-readable summaries live in [`books/`](books/).
5. Content blueprints live in [`templates/`](templates/).

---

## Repository Layers

| Layer | Path | Role |
|-------|------|------|
| Docs | `docs/` | Architecture, workflow, roadmap, style |
| Standards | `standards/` | Evidence, editorial, SEO, affiliate, terminology |
| Schemas | `schemas/` | Entity definitions |
| Data | `data/` | Canonical YAML records |
| Books | `books/` | Human-readable knowledge bibles |
| Research | `research/` | Unvalidated source notes |
| Templates | `templates/` | PCME section blueprints |
| Scripts | `scripts/` | Validation and export automation |
| Exports | `exports/` | Generated outputs (not source of truth) |

---

## Core Workflow

```
Research → Validation → Schema → Data → Book Content → Templates → PCME → Publishing → Review
```

See [`docs/workflow.md`](docs/workflow.md).

---

## Book 1 — Aftercare Bible

Start at [`books/01-aftercare-bible/00-index.md`](books/01-aftercare-bible/00-index.md).

---

## Principles

1. Safety before revenue
2. Evidence before marketing
3. Store knowledge once, publish many times
4. Affiliate data separate from safety evaluation

See [`docs/vision.md`](docs/vision.md).

---

## License and Usage

Internal PiercingConnect commercial knowledge base. Do not commit secrets or credentials.
