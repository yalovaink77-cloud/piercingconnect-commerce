# Knowledge Architecture

Version: 1.0
Status: Active
Project: PiercingConnect Commerce Blueprint

---

## Purpose

This document defines the knowledge architecture of the PiercingConnect Commerce Blueprint.

The goal is to separate human-readable knowledge from machine-readable data so that the same source can support:

* editorial content
* SEO strategy
* affiliate publishing
* product databases
* brand comparisons
* PC Media Engine automation
* future AI workflows

---

## Core Architecture Principle

Knowledge must be stored once and reused many times.

Published articles are outputs.

The repository is the source of truth.

---

## Repository Layers

### 1. Books Layer

Path:

`books/`

Purpose:

Human-readable commercial knowledge.

This layer contains structured explanations, strategy documents, guides, taxonomies, and editorial knowledge.

Examples:

* Aftercare Bible
* Jewelry Bible
* Professional Studio Bible
* Healing & Lifestyle Bible
* Affiliate & Revenue Bible

The books layer is written for humans first.

---

### 2. Data Layer

Path:

`data/`

Purpose:

Machine-readable structured information.

This layer will contain YAML, JSON, or CSV files that can be consumed by PC Media Engine and future automation tools.

Examples:

* brand profiles
* product records
* keyword clusters
* affiliate programs
* country availability
* comparison data

The data layer is written for software first.

---

### 3. Docs Layer

Path:

`docs/`

Purpose:

Project architecture and operating rules.

This layer explains how the knowledge system should be built, maintained, expanded, and used.

Examples:

* vision
* architecture
* roadmap
* taxonomy
* workflow
* style guide

---

### 4. Standards Layer

Path:

`standards/`

Purpose:

Editorial, ethical, medical, SEO, affiliate, and terminology rules.

This layer protects quality and trust.

Examples:

* evidence policy
* affiliate policy
* SEO guidelines
* terminology guide
* editorial guidelines

---

### 5. Research Layer

Path:

`research/`

Purpose:

Raw research notes.

This layer may include unprocessed findings, early investigation, source summaries, competitor notes, and market research.

Research is not automatically trusted.

Research must be validated before it becomes part of `books/` or `data/`.

---

### 6. References Layer

Path:

`references/`

Purpose:

Source materials and citation notes.

This layer supports trust, evidence, and editorial review.

Examples:

* APP references
* wound care references
* product documentation
* brand documentation
* affiliate program notes

---

### 7. Templates Layer

Path:

`templates/`

Purpose:

Reusable content structures.

Examples:

* product review template
* brand profile template
* buyer guide template
* comparison article template
* FAQ template
* Pinterest pin template
* YouTube script template

---

### 8. Scripts Layer

Path:

`scripts/`

Purpose:

Automation tools.

Future scripts may support:

* Markdown validation
* YAML validation
* broken link checking
* affiliate link checks
* export generation
* PC Media Engine ingestion
* content packaging

---

### 9. Exports Layer

Path:

`exports/`

Purpose:

Generated outputs.

Examples:

* PDF exports
* CSV exports
* JSON exports
* AI datasets
* publishing packages

Exports are generated artifacts.

They are not the source of truth.

---

## Human vs Machine Knowledge

The repository must maintain a clear distinction:

### Human-readable knowledge

Stored in:

`books/`

Used for:

* strategy
* editorial planning
* education
* explanations
* long-form knowledge

### Machine-readable knowledge

Stored in:

`data/`

Used for:

* automation
* publishing
* filtering
* comparison
* AI generation
* PC Media Engine workflows

---

## Example

A brand such as NeilMed may appear in two places:

### Human-readable version

`books/01-aftercare-bible/04-brand-database.md`

This explains:

* brand reputation
* product positioning
* safety considerations
* comparison opportunities
* editorial strategy

### Machine-readable version

`data/brands/neilmed.yaml`

This stores:

* brand name
* country
* product list
* affiliate programs
* availability
* trust score
* related keywords
* content opportunities

Both layers must agree.

If they conflict, the structured data and book content must be reviewed together.

---

## Source of Truth Rule

The repository is the source of truth.

WordPress posts, Pinterest posts, videos, PDFs, and emails are downstream outputs.

Content should be generated from the repository.

The repository should not be reconstructed from published content.

---

## PC Media Engine Relationship

PC Media Engine is the publishing engine.

This repository is the commercial knowledge core.

PC Media Engine should eventually consume:

* Markdown files from `books/`
* structured files from `data/`
* templates from `templates/`
* standards from `standards/`

and generate publishable content for multiple platforms.

---

## Knowledge Lifecycle

Each knowledge asset should follow this lifecycle:

1. Research
2. Validation
3. Structuring
4. Editorial writing
5. Review
6. Publishing
7. Monitoring
8. Updating

No important knowledge should skip validation.

---

## Trust Rule

Any content that affects user safety must be treated as high-risk knowledge.

High-risk knowledge requires:

* careful wording
* evidence support
* medical disclaimers where appropriate
* avoidance of diagnosis
* clear referral to qualified professionals when necessary

---

## Commercial Rule

Affiliate opportunity is allowed only after safety, quality, and trust have been evaluated.

Commercial value must never override health or safety.

---

## Expansion Rule

New categories, books, data types, and templates should be added only when they support a real publishing, SEO, affiliate, or educational need.

The system should grow deliberately, not randomly.

---

## Final Principle

PiercingConnect is not a blog that stores articles.

PiercingConnect is a knowledge system that generates articles.
