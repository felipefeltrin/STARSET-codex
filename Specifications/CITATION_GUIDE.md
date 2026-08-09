# Citation Guide

| Field | Value |
|---|---|
| Document ID | DOC-SPEC-0004 |
| Category | Specification |
| Status | Accepted |
| Version | 1.0.0 |
| Last Updated | 2026-08-05 |

## Purpose

This document defines how claims in **The STARSET Codex** are connected to registered evidence.

## Core Rule

Every factual lore claim SHALL be traceable to one or more registered sources.

## Identifiers

- Sources use permanent `SRC` identifiers.
- Individual citation records use permanent `CIT` identifiers.
- Source registration occurs in [`../Registries/SOURCE_REGISTRY.md`](../Registries/SOURCE_REGISTRY.md).

## Citation Record

A citation record SHOULD identify:

- Citation ID.
- Source ID.
- Precise locator, such as page, chapter, timestamp, URL snapshot, demonstration date, or ARG record.
- Claim or paragraph supported.
- Access or verification date when applicable.
- Notes about source limitations.

**Example:**

```text
Citation: CIT-0042
Source: SRC-0001
Locator: Chapter 8, pages 112–115
Supports: Description of the transmission experiment
```

The machine-readable record belongs in the appropriate companion source file, not in Markdown front matter.

## What Requires Citation

Citations are required for:

- Factual lore claims.
- Dates, locations, identities, and sequence of events.
- Direct quotations.
- Claims about creator intent.
- Historical facts used to compare reality with fiction.
- Reconstructions and theories, including all supporting evidence.
- Statements that one source contradicts or supersedes another.

Common project instructions and original analysis methods do not require lore citations unless they depend on external facts.

## Citation Placement

Citations SHOULD appear as close as practical to the supported claim. A single citation may support several adjacent sentences only when the scope is unambiguous.

**Good:** The citation follows the paragraph describing one event from one source.

**Bad:** A single citation appears at the end of a page containing unrelated claims from several works.

## Direct Quotations

Quotations SHALL:

- Preserve the original wording.
- Identify the speaker or source context when known.
- Include a precise locator.
- Remain no longer than necessary for analysis.

## Reconstructions

A reconstruction SHALL cite every material source used to reach the conclusion and explain the inference.

**Example:** A map reconstructing a location from three separate travel descriptions cites all three passages, not only the passage that best matches the final result.

## Community Sources

Community research MAY be cited as evidence of discovery history, interpretation, or archival recovery. It SHALL NOT replace available official evidence for canon claims.

## Unavailable or Ephemeral Sources

When an official source is no longer publicly available:

- Preserve its registry entry.
- Record the last verified status.
- Cite authenticated archives or captures when lawful and available.
- Clearly state limitations.
- Do not present unverified recollections as confirmed evidence.

## Citation Quality

Prefer the most direct and authoritative source available. A novel should be cited for a novel event rather than a fan summary of the novel.

## Related Documents

- [`../Registries/SOURCE_REGISTRY.md`](../Registries/SOURCE_REGISTRY.md)
- [`CANON_CONFIDENCE.md`](CANON_CONFIDENCE.md)
- [`../Governance/EDITORIAL_POLICY.md`](../Governance/EDITORIAL_POLICY.md)
- [`METADATA_SPEC.md`](METADATA_SPEC.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.0.0 | 2026-08-05 | Expanded claim coverage, placement, quotations, reconstruction, ephemeral-source, and source-quality standards. |
