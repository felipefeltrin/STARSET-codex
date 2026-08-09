# Chapter Package Standard

| Field | Value |
|---|---|
| Document ID | DOC-SPEC-0003 |
| Category | Specification |
| Status | Accepted |
| Version | 1.0.0 |
| Last Updated | 2026-08-05 |

## Purpose

This document defines the required structure of every independently publishable lore chapter package.

## Package Structure

```text
CH-0001/
├── chapter.md
├── chapter.pdf
├── metadata.yaml
├── manifest.yaml
├── sources.yaml
└── assets/
    ├── figures/
    ├── diagrams/
    └── maps/
```

Empty asset directories MAY be omitted when a chapter contains no assets.

## Required Files

### `chapter.md`

Canonical human-readable chapter source.

### `chapter.pdf`

Standalone generated chapter release artifact.

### `metadata.yaml`

Machine-readable chapter identity, status, revision, classification, and editorial data.

### `manifest.yaml`

Inventory of every file and registered object belonging to the chapter package.

### `sources.yaml`

Chapter-specific citation and source subset referencing registered `SRC` and `CIT` identifiers.

## Required Markdown Sections

Every `chapter.md` SHALL contain:

1. Archive Header.
2. Chapter Title.
3. Abstract.
4. Main Narrative or Analysis.
5. Cross-References.
6. Source Notes.
7. Canon Confidence Summary.
8. Revision History.

Metadata SHALL NOT be embedded in the Markdown. The archive header is human-readable presentation, not machine-readable metadata.

## Optional Markdown Sections

Include only when useful:

- Archivist Notes.
- Figures.
- Diagrams.
- Maps.
- Tables.
- Contradiction Analysis.
- Historical-versus-fictional comparison.
- Unresolved Questions.
- Further Reading.

## Archive Header

The archive header SHOULD include:

- STARSET Society Archive label.
- SSA document ID.
- Classification.
- Integrity or recovery status when narratively appropriate.
- Authentication status.
- Revision.

**Example:**

```text
STARSET Society Archive
Document: SSA-0100
Classification: Public Release
Authentication: Verified
Revision: 1.0.0
```

## Abstract

The abstract SHOULD summarize the chapter's subject, scope, chronological range, and major evidence boundaries without attempting to replace the chapter.

## Main Body

The main body SHALL:

- Follow the Style Guide.
- Distinguish canon from reconstruction.
- Explain essential context without requiring another chapter.
- Cite factual claims.
- Preserve source contradictions where relevant.

## Cross-References

Cross-references SHALL use stable identifiers and descriptive titles.

**Example:** `For the organization created around these events, see CH-0009, Order of Teslonia.`

## Source Notes

Source Notes SHALL explain unusual source limitations, adaptation differences, unavailable ARG material, reconstruction methods, or citation boundaries not obvious from individual citations.

## Canon Confidence Summary

The summary SHALL identify which confidence levels appear in the chapter and call out major non-confirmed conclusions.

## Revision History

Each chapter SHALL record its version, date, and meaningful changes. Published versions are immutable.

## Publishability Test

Before publication, reviewers must be able to answer yes to each question:

- Can a reader understand the chapter's core subject without opening another chapter?
- Can the package produce a standalone PDF without manual rewriting?
- Are all required sources and assets present?
- Are all external dependencies explicitly identified?
- Can the chapter be revised without restructuring unrelated chapters?

## Related Documents

- [`../Governance/STYLE_GUIDE.md`](../Governance/STYLE_GUIDE.md)
- [`METADATA_SPEC.md`](METADATA_SPEC.md)
- [`ASSET_GUIDE.md`](ASSET_GUIDE.md)
- [`CITATION_GUIDE.md`](CITATION_GUIDE.md)
- [`CANON_CONFIDENCE.md`](CANON_CONFIDENCE.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.0.0 | 2026-08-05 | Defined complete chapter packages, required and optional sections, and standalone publishability tests. |
