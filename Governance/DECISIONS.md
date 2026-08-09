# Architectural Decisions

| Field | Value |
|---|---|
| Document ID | DOC-GOV-0002 |
| Category | Governance |
| Status | Accepted |
| Version | 1.0.0 |
| Last Updated | 2026-08-05 |

## Purpose

This document records durable project decisions and the reasoning behind them. It prevents future maintainers from having to rediscover why the repository was designed in a particular way.

## Decision Format

Each decision contains a status, context, decision, consequences, and alternatives considered.

---

## DEC-0001 — Markdown Is the Source of Truth

**Status:** Accepted

### Context

The project requires a format that is portable, diff-friendly, readable without specialized software, and suitable for generating multiple outputs.

### Decision

Markdown SHALL be the canonical human-readable content source. PDFs, websites, search indexes, and similar outputs SHALL be generated artifacts.

### Consequences

- Contributors edit readable source files.
- Generated outputs may be rebuilt consistently.
- Output-specific changes must originate in source or build configuration.

### Alternatives Considered

- Word-processing documents.
- HTML as the primary source.
- LaTeX as the primary source.

---

## DEC-0002 — Metadata Lives Outside Markdown

**Status:** Accepted

### Context

Embedded front matter mixes machine-readable configuration with prose and complicates independent content reuse.

### Decision

Metadata SHALL NEVER be embedded inside Markdown files. Companion files such as `metadata.yaml`, `manifest.yaml`, and `sources.yaml` SHALL store machine-readable data.

### Consequences

- Markdown remains clean and portable.
- Automation can process metadata without parsing prose.
- Every publishable package requires companion files.

### Alternatives Considered

- YAML front matter.
- JSON front matter.
- HTML metadata comments.

---

## DEC-0003 — Single Source of Truth

**Status:** Accepted

### Context

Duplicated rules drift and eventually contradict one another.

### Decision

Every rule, schema, hierarchy, or registry SHALL have exactly one authoritative document. Other files SHALL reference that authority rather than reproduce it.

### Consequences

- Changes are made once.
- Cross-references become important and must remain valid.
- Summaries may explain a rule but must not redefine it.

### Alternatives Considered

- Repeating core rules in every contributor-facing document.

---

## DEC-0004 — Chapters Are Independently Publishable

**Status:** Accepted

### Context

Chapters must remain maintainable, exportable, and revisable without rebuilding the entire Codex.

### Decision

Every chapter SHALL be understandable and publishable as a standalone package containing its Markdown, PDF, metadata, citations, manifest, revision history, and required assets.

### Consequences

- Limited contextual repetition is acceptable when necessary for comprehension.
- Cross-references may enrich a chapter but cannot be required to understand its core subject.
- Chapter-specific source and asset subsets must travel with the package.

### Alternatives Considered

- A monolithic book source with inseparable chapters.

---

## DEC-0005 — Published Releases Are Immutable

**Status:** Accepted

### Context

Readers and researchers need stable, reproducible versions they can cite.

### Decision

A published release SHALL never be altered retroactively. Corrections and additions SHALL be published under a new semantic version.

### Consequences

- Release artifacts remain stable.
- Corrections require changelog entries and new release versions.
- Historical releases remain accessible after supersession.

### Alternatives Considered

- Silently replacing release files.
- Maintaining only a continuously updated latest edition.

---

## DEC-0006 — The Repository Must Remain Buildable

**Status:** Accepted

### Context

A broken default branch prevents reliable collaboration and release generation.

### Decision

Every commit merged into `main` SHALL preserve a valid project state capable of producing all currently supported outputs. Enforcement will be implemented when CI/CD and build tooling are created.

### Consequences

- The public repository will use branch protection and automated validation.
- Partial migrations must use feature branches until complete.
- Build requirements may expand as outputs are introduced.

### Alternatives Considered

- Allowing temporarily broken states on `main`.

## Related Documents

- [`../README.md`](../README.md)
- [`EDITORIAL_POLICY.md`](EDITORIAL_POLICY.md)
- [`../Specifications/METADATA_SPEC.md`](../Specifications/METADATA_SPEC.md)
- [`../Specifications/CHAPTER_TEMPLATE.md`](../Specifications/CHAPTER_TEMPLATE.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.0.0 | 2026-08-05 | Converted project decisions into standardized architectural decision records. |
