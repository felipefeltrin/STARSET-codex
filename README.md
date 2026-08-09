# The STARSET Codex

> A living, open-source archive of the STARSET universe.

## Mission

The STARSET Codex documents STARSET lore through transparent editorial standards, verifiable sourcing, stable identifiers, and community maintenance. It is designed to serve both as an immersive reference and as a durable open-source knowledge project.

## Guiding Principles

### Document First. Interpret Second.

Official material is recorded before analysis is introduced. Interpretation must never replace what a source actually states.

**Example:** First summarize what *The Prox Transmissions* establishes; then identify any broader implication as interpretation.

### Canon Before Speculation

Evidence from official sources takes precedence over theories, assumptions, or preferred interpretations. Speculation may be documented only when clearly labeled under the confidence system defined in [`Specifications/CANON_CONFIDENCE.md`](Specifications/CANON_CONFIDENCE.md).

### No Lore Left Behind

Older or contradictory material is preserved rather than silently removed. When sources disagree, the Codex documents each version, explains the conflict, and applies the hierarchy defined in [`Governance/EDITORIAL_POLICY.md`](Governance/EDITORIAL_POLICY.md).

**Example:** If a demonstration presents an event differently from a later novel, both accounts remain available with an editorial note explaining precedence.

### Markdown Is the Source of Truth

Markdown files are the canonical human-readable source. PDFs, websites, indexes, and other outputs are generated artifacts.

### Every Claim Is Traceable

Factual lore claims must be supported by citations. Reconstructions must identify all supporting evidence.

### Stable Identifiers

Permanent identifiers are never renamed, reassigned, or reused. Identifier rules are defined in [`Specifications/ID_STANDARDS.md`](Specifications/ID_STANDARDS.md).

### Single Source of Truth

Every rule has one authoritative location. Other documents reference that location instead of duplicating the rule.

### The Repository Must Always Be Buildable

Every commit merged into `main` must preserve a repository state capable of producing a valid project release. This rule will later be enforced through protected branches and CI/CD validation.

### Publishable Chapters

Every chapter must be independently understandable and independently exportable with its own Markdown source, PDF, metadata, citations, manifest, revision history, and required assets.

### Immutable Releases

Published releases are never modified retroactively. Corrections and additions are delivered through new semantic versions.

## Repository Structure

- `Governance/` — how the project is managed and reviewed.
- `Specifications/` — technical and editorial implementation standards.
- `Registries/` — living databases for permanent objects and sources.
- `Content/` — lore chapters, appendices, archives, and associated packages. This directory will be introduced during content creation.
- `README.md` — repository entry point.
- `CHANGELOG.md` — project history.

The repository structure diagram is available as `folder_structure.png` and will be revised when content and infrastructure directories are introduced.

## Current Development Order

1. Finalize governance and writing standards.
2. Produce the complete lore content currently available.
3. Create the public GitHub repository.
4. Add build tooling, CI/CD, the website, and release automation.
5. Publish the first public release.

Current progress is tracked in [`Governance/PROJECT_ROADMAP.md`](Governance/PROJECT_ROADMAP.md).

## Contributing

Contribution requirements are defined in [`Governance/CONTRIBUTING.md`](Governance/CONTRIBUTING.md). Contributors must also follow the editorial, citation, metadata, asset, identifier, and review standards linked there.

## Versioning

The project uses Semantic Versioning:

- **Major:** canon or architecture changes requiring significant restructuring.
- **Minor:** new content, sources, or compatible features.
- **Patch:** corrections, citation improvements, and non-breaking editorial fixes.

## License

A repository license will be selected before the public GitHub release. Until then, no reuse license is implied.
