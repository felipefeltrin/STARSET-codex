# Source Registry

| Field | Value |
|---|---|
| Document ID | DOC-REG-0002 |
| Category | Registry |
| Status | Active |
| Version | 1.0.0 |
| Last Updated | 2026-08-05 |

## Purpose

The Source Registry is the authoritative database of every source cited by **The STARSET Codex**.

## Registry Rules

- Every distinct source SHALL receive one permanent `SRC` identifier.
- Identifiers SHALL never be reused.
- Metadata corrections update the existing entry rather than creating a duplicate source.
- Source authority is determined by [`../Governance/EDITORIAL_POLICY.md`](../Governance/EDITORIAL_POLICY.md); this registry records the assigned tier but does not redefine it.
- `Last Verified` records the most recent date on which the source identity and availability were checked.
- A removed or inaccessible source remains registered and receives an updated status.

## Registered Sources

| ID | Type | Title | Creator or Publisher | Canon Tier | Status | Last Verified | Notes |
|---|---|---|---|---|---|---|---|
| SRC-0001 | Novel | *The Prox Transmissions* | Dustin Bates and Peter David | Tier I | Active | 2026-08-05 | Foundational primary canon. |
| SRC-0002 | Novel | *A Brief History of the Future* | Dustin Bates | Tier I | Active | 2026-08-05 | Primary canon continuation. |
| SRC-0003 | Album | *Transmissions* | STARSET | Tier II | Active | 2026-08-05 | Official narrative media. |

## Future Source Types

The registry may include novels, albums, songs, music videos, comics, demonstrations, ARG entries, official websites, interviews, social-media records, and creator statements.

## Related Documents

- [`../Governance/EDITORIAL_POLICY.md`](../Governance/EDITORIAL_POLICY.md)
- [`../Specifications/CITATION_GUIDE.md`](../Specifications/CITATION_GUIDE.md)
- [`OBJECT_REGISTRY.md`](OBJECT_REGISTRY.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.0.0 | 2026-08-05 | Added publisher, verification date, availability rules, and source-authority cross-reference. |
