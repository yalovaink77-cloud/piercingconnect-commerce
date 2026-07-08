# PCME Publishing (Navigation)

Version: 1.0

Status: Navigation chapter

---

# Notice

This file occupies the **original Book 1 chapter 08 slot** for PC Media Engine publishing strategy.

The populated piercing types knowledge chapter is at **`08-piercing-types.md`**.

---

# Canonical Documentation

**Read:** [`docs/content-generation-architecture.md`](../../docs/content-generation-architecture.md)

**Templates:** `templates/` (section blueprints)

**Template entities:** `data/templates/`

**Content asset types:** `data/content-assets/`

---

# Pipeline Summary

```
Knowledge Core (data/) → Template Engine (templates/) → PCME → Publishing channels
```

Publishing targets: WordPress, Facebook, Pinterest, Email, YouTube, PDF

---

# Generation Rules

1. Resolve all required entities before generation
2. Apply `standards/evidence-policy.md` and affiliate policy
3. Safety notes from keyword clusters override commercial placement
4. Templates define sections only — PCME generates prose
5. Flag outputs when source entities are `review.status: draft`

---

# Why This File Exists

Preserves the original index reference to chapter 08 without renumbering `08-piercing-types.md`.

See `01-information-architecture.md` for the full chapter map.

---

# Related

- `docs/workflow.md`
- `books/01-aftercare-bible/13-seo-clusters.md`
- `books/01-aftercare-bible/14-supporting-taxonomies.md`
