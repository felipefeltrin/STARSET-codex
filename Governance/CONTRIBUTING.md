# Contributing

| Field | Value |
|---|---|
| Document ID | DOC-GOV-0001 |
| Category | Governance |
| Status | Accepted |
| Version | 1.0.0 |
| Last Updated | 2026-08-05 |

## Purpose

This document defines how contributors propose, prepare, and submit changes to **The STARSET Codex**.

## Scope

These requirements apply to lore content, governance documents, specifications, registries, citations, metadata, and assets.

## Contributor Workflow

`Fork or branch -> Make focused changes -> Validate content and structure -> Update required companion files -> Open pull request -> Complete review -> Merge`

Direct commits to `main` will be disabled when the public GitHub repository is created.

## Editorial Expectations

### Never Present Speculation as Fact

**Good:**

> The novel explicitly states that the transmission originated from the future. A possible implication is that the sender understood temporal causality well enough to exploit it.

**Bad:**

> The sender definitely created a multiverse.

Interpretation must be separated from documented canon and assigned a confidence level under [`../Specifications/CANON_CONFIDENCE.md`](../Specifications/CANON_CONFIDENCE.md).

### Preserve Superseded Lore

**Good:** Document both versions, identify their sources, explain the conflict, and apply the editorial hierarchy.

**Bad:** Delete the older version because newer material exists.

The Codex functions as both a current reference and a historical archive of how the lore developed.

## Mandatory Requirements

Every contributor SHALL:

- Cite factual lore paragraphs according to [`../Specifications/CITATION_GUIDE.md`](../Specifications/CITATION_GUIDE.md).
- Follow the applicable content structure, including [`../Specifications/CHAPTER_TEMPLATE.md`](../Specifications/CHAPTER_TEMPLATE.md) for chapters.
- Allocate permanent identifiers according to [`../Specifications/ID_STANDARDS.md`](../Specifications/ID_STANDARDS.md).
- Register new objects and sources before publication.
- Never rename, reuse, or silently replace an existing identifier.
- Follow [`STYLE_GUIDE.md`](STYLE_GUIDE.md) and [`EDITORIAL_POLICY.md`](EDITORIAL_POLICY.md).
- Store metadata only in companion YAML files as required by [`../Specifications/METADATA_SPEC.md`](../Specifications/METADATA_SPEC.md).
- Update `CHANGELOG.md` when a change is notable to readers or contributors.

## Pull Request Contents

A pull request SHOULD include, when applicable:

- Updated Markdown.
- Updated companion metadata.
- Updated source references.
- Updated manifests.
- New or revised assets and their metadata.
- Object and source registry updates.
- A changelog entry.
- A clear explanation of the change and its evidence.

**Example:** A new organization article should include the article Markdown, metadata, source list, manifest, any diagrams, registry entries, and citations supporting the article.

## Pull Request Scope

Pull requests SHOULD remain focused. Unrelated changes should be separated unless they are inseparable parts of one migration.

**Good:** Correct one chapter and its citations.

**Bad:** Correct one chapter, rename unrelated assets, rewrite the roadmap, and change the editorial hierarchy in the same request.

## Before Requesting Review

Contributors SHOULD verify:

- Markdown renders correctly.
- Companion YAML is valid and external to Markdown.
- Identifiers are unique and registered.
- Cross-references resolve.
- Factual claims have citations.
- Confidence labels match the evidence.
- Assets follow the asset specification.
- The contribution can pass the workflow in [`REVIEW_PROCESS.md`](REVIEW_PROCESS.md).

## Related Documents

- [`STYLE_GUIDE.md`](STYLE_GUIDE.md)
- [`EDITORIAL_POLICY.md`](EDITORIAL_POLICY.md)
- [`REVIEW_PROCESS.md`](REVIEW_PROCESS.md)
- [`../Specifications/CANON_CONFIDENCE.md`](../Specifications/CANON_CONFIDENCE.md)
- [`../Specifications/METADATA_SPEC.md`](../Specifications/METADATA_SPEC.md)
- [`../Specifications/ID_STANDARDS.md`](../Specifications/ID_STANDARDS.md)
- [`../Specifications/CITATION_GUIDE.md`](../Specifications/CITATION_GUIDE.md)
- [`../Specifications/ASSET_GUIDE.md`](../Specifications/ASSET_GUIDE.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.0.0 | 2026-08-05 | Standardized contributor workflow, mandatory rules, examples, and review requirements. |
