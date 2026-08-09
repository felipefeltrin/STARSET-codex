# Metadata Specification

| Field | Value |
|---|---|
| Document ID | DOC-SPEC-0006 |
| Category | Specification |
| Status | Accepted |
| Version | 1.0.0 |
| Last Updated | 2026-08-05 |

## Purpose

This document defines how machine-readable metadata is stored and which fields are required for chapters and assets.

## Non-Negotiable Separation Rule

Metadata SHALL NEVER be embedded inside Markdown files.

Markdown contains only human-readable content. Machine-readable metadata belongs in external companion YAML files.

**Correct:**

```text
chapter.md
metadata.yaml
manifest.yaml
sources.yaml
```

**Incorrect:** YAML front matter at the beginning of `chapter.md`.

This rule applies even when a static-site generator supports front matter. Build tooling must read companion files instead.

## YAML Conventions

- Files SHALL use UTF-8.
- Indentation SHALL use spaces, not tabs.
- Dates SHALL use ISO format: `YYYY-MM-DD`.
- Versions SHOULD use Semantic Versioning.
- Enumerated values SHALL use the exact spelling defined by their specification.
- Unknown required values SHALL not be guessed. Use an explicitly allowed placeholder or leave the package in Draft status.

## Chapter Metadata

Required fields:

- `id`
- `title`
- `revision`
- `status`
- `classification`
- `ssa_document`
- `last_updated`
- `owner`
- `first_release`

Optional fields:

- `subtitle`
- `dependencies`
- `reviewed_by`
- `introduced_in`
- `chronological_scope`
- `notes`

**Example companion file:**

```yaml
id: CH-0001
title: Introduction
revision: 1.0.0
status: Draft
classification: Public Release
ssa_document: SSA-0100
last_updated: 2026-08-05
owner: Content Team
first_release: Unreleased
```

The example is a standalone YAML file, not Markdown front matter.

## Asset Metadata

Required fields:

- `id`
- `title`
- `revision`
- `asset_type`
- `creator`
- `source`
- `copyright_status`
- `confidence`
- `last_updated`

Optional fields:

- `description`
- `alt_text`
- `attribution`
- `derived_from`
- `dimensions`
- `notes`

## Manifest Metadata

A manifest SHALL list every file and registered object owned by a package.

Recommended fields:

- `package_id`
- `revision`
- `files`
- `objects`
- `generated_outputs`
- `shared_dependencies`

## Source Metadata

A chapter `sources.yaml` SHALL reference registered `SRC` and `CIT` identifiers rather than redefining source authority.

## Validation

Future build tooling will validate schemas. Until then, reviewers SHALL manually verify required fields, values, dates, identifiers, and companion-file separation.

## Related Documents

- [`CHAPTER_TEMPLATE.md`](CHAPTER_TEMPLATE.md)
- [`ASSET_GUIDE.md`](ASSET_GUIDE.md)
- [`ID_STANDARDS.md`](ID_STANDARDS.md)
- [`../Governance/DECISIONS.md`](../Governance/DECISIONS.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.0.0 | 2026-08-05 | Strengthened external metadata enforcement and added conventions, fields, manifests, source metadata, and examples. |
