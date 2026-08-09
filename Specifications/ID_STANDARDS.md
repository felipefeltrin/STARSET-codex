# Identifier Standards

| Field | Value |
|---|---|
| Document ID | DOC-SPEC-0005 |
| Category | Specification |
| Status | Accepted |
| Version | 1.0.0 |
| Last Updated | 2026-08-05 |

## Purpose

This document is the single source of truth for permanent identifier formats in **The STARSET Codex**.

## Core Rules

- Identifiers SHALL be immutable.
- Identifiers SHALL never be reused, even after deprecation.
- Existing identifiers SHALL never be renamed to improve ordering or aesthetics.
- New identifier types SHALL be added here before use.
- Every allocated identifier SHALL be recorded in the appropriate registry.

## Standard Format

Most identifiers use:

```text
PREFIX-0001
```

Document identifiers use:

```text
DOC-CATEGORY-0001
```

Numeric portions use at least four digits and increase sequentially within each prefix.

## Object Prefixes

| Prefix | Object Type | Example |
|---|---|---|
| CH | Chapter | `CH-0001` |
| EVT | Event | `EVT-0042` |
| CHR | Character | `CHR-0001` |
| ORG | Organization | `ORG-0001` |
| TEC | Technology | `TEC-0001` |
| LOC | Location | `LOC-0001` |
| MAP | Map | `MAP-0003` |
| FIG | Figure, including photographs, screenshots, and artwork | `FIG-0012` |
| DIG | Diagram, including flowcharts, relationship graphs, timelines, and schematics | `DIG-0007` |
| ARC | In-universe archive document or recreated archival insert | `ARC-0001` |
| SON | Song | `SON-0001` |
| ALB | Album | `ALB-0001` |
| DEM | Demonstration | `DEM-0001` |
| ARG | ARG entry | `ARG-0001` |
| INT | Interview | `INT-0001` |
| SRC | Registered source | `SRC-0001` |
| CIT | Citation record | `CIT-0001` |
| SSA | STARSET Society Archive presentation document | `SSA-0100` |

## Project Document Prefixes

| Prefix | Document Category | Example |
|---|---|---|
| DOC-GOV | Governance document | `DOC-GOV-0003` |
| DOC-SPEC | Specification document | `DOC-SPEC-0005` |
| DOC-REG | Registry document | `DOC-REG-0001` |

These identifiers classify project documentation and are distinct from in-universe `SSA` presentation identifiers.

## Figure, Diagram, and Map Boundaries

- Use `FIG` when the asset primarily depicts or reproduces something.
- Use `DIG` when the asset explains relationships, systems, or processes.
- Use `MAP` when spatial position is the primary information.

**Examples:**

- Wardenclyffe photograph -> `FIG`.
- Timeline branching flowchart -> `DIG`.
- Confirmed and inferred lore locations -> `MAP`.

## Allocation

The next available identifier SHALL be selected from the authoritative Object or Source Registry. Contributors must not infer availability from filenames alone.

## Deprecation

Deprecated objects retain their original ID and registry record. Their status changes to `Deprecated`, with a note identifying the replacement when one exists.

## Related Documents

- [`../Registries/OBJECT_REGISTRY.md`](../Registries/OBJECT_REGISTRY.md)
- [`../Registries/SOURCE_REGISTRY.md`](../Registries/SOURCE_REGISTRY.md)
- [`ASSET_GUIDE.md`](ASSET_GUIDE.md)
- [`../Governance/DECISIONS.md`](../Governance/DECISIONS.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.0.0 | 2026-08-05 | Added governance, specification, and registry document identifiers; clarified allocation, asset boundaries, and deprecation. |
