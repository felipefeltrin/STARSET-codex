# Review Process

| Field | Value |
|---|---|
| Document ID | DOC-GOV-0006 |
| Category | Governance |
| Status | Accepted |
| Version | 1.0.0 |
| Last Updated | 2026-08-05 |

## Purpose

This document defines the mandatory review stages and objective acceptance criteria for contributions.

## Workflow

`Draft -> Technical Review -> Lore Review -> Citation Review -> Asset Review, when applicable -> Editorial Approval -> Published`

A reviewer MAY return a contribution to any earlier stage when revisions affect previously completed checks.

## Technical Review

Reviewers SHALL verify:

- Markdown is valid and readable.
- Companion YAML is valid and external to Markdown.
- Identifiers follow the registered format and are unique.
- Required companion files exist.
- File and directory names follow project conventions.
- Cross-references resolve.

## Lore Review

Reviewers SHALL verify:

- The canon hierarchy in [`EDITORIAL_POLICY.md`](EDITORIAL_POLICY.md) is respected.
- Source material is represented accurately.
- Contradictions and superseded lore are preserved and explained.
- Historical facts and fictional additions are distinguished when applicable.
- Confidence levels match the evidence.

## Citation Review

Reviewers SHALL verify:

- Factual lore claims are traceable.
- Direct quotations include precise references.
- Reconstructions cite all relevant supporting sources.
- Registered source identifiers are used consistently.

## Asset Review

When assets are included, reviewers SHALL verify:

- Identifiers, filenames, formats, and directories follow the Asset Guide.
- Companion metadata exists.
- Captions and source information are complete.
- Licensing and attribution requirements are satisfied.
- The asset remains legible in standalone chapter and compiled contexts.

## Editorial Review

Reviewers SHALL verify:

- The Style Guide is followed.
- The document maintains a professional, neutral, and readable voice.
- Mandatory and optional sections are used correctly.
- The contribution is independently understandable where required.
- The changelog and registries are updated when applicable.

## Automatic Rejection Criteria

A contribution SHALL NOT be approved while any of the following remain:

- Duplicate or reused identifiers.
- Metadata embedded in Markdown.
- Missing required citations.
- Speculation presented as canon.
- Silent deletion of contradictory or superseded lore.
- Missing required package files.
- Broken cross-references.
- Unresolved licensing problems.
- Direct changes to a published immutable release.

## Review Outcomes

- **Approved:** All applicable checks pass.
- **Changes Requested:** Correctable problems remain.
- **Rejected:** The contribution conflicts with project scope, evidence standards, or foundational policy.
- **Deferred:** The contribution may be valid but depends on unresolved work or unavailable evidence.

## Related Documents

- [`CONTRIBUTING.md`](CONTRIBUTING.md)
- [`EDITORIAL_POLICY.md`](EDITORIAL_POLICY.md)
- [`STYLE_GUIDE.md`](STYLE_GUIDE.md)
- [`../Specifications/CITATION_GUIDE.md`](../Specifications/CITATION_GUIDE.md)
- [`../Specifications/CANON_CONFIDENCE.md`](../Specifications/CANON_CONFIDENCE.md)
- [`../Specifications/ASSET_GUIDE.md`](../Specifications/ASSET_GUIDE.md)
- [`../Specifications/METADATA_SPEC.md`](../Specifications/METADATA_SPEC.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.0.0 | 2026-08-05 | Standardized the review workflow and added objective rejection criteria. |
