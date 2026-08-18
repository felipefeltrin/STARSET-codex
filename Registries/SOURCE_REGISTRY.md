# Source Registry

| Field | Value |
|---|---|
| Document ID | DOC-REG-0002 |
| Category | Registry |
| Status | Active |
| Version | 1.1.0 |
| Last Updated | 2026-08-18 |

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
| SRC-0001 | Novel | *The Prox Transmissions* | Dustin Bates and Peter David | Tier I | Active | 2026-08-18 | Foundational primary canon. Primary-text locators should be verified before final publication. |
| SRC-0002 | Novel | *A Brief History of the Future* | Dustin Bates | Tier I | Active | 2026-08-18 | Primary canon continuation. Primary-text locators should be verified before final publication. |
| SRC-0003 | Album | *Transmissions* | STARSET | Tier II | Active | 2026-08-18 | Official narrative media. |
| SRC-0004 | Album | *Vessels* | STARSET | Tier II | Active | 2026-08-18 | Official narrative media; chronology is less explicit than in the novels. |
| SRC-0005 | Album | *DIVISIONS* | STARSET | Tier II | Active | 2026-08-18 | Official narrative media centered on the BMI/New East dystopian setting. |
| SRC-0006 | Album | *HORIZONS* | STARSET | Tier II | Active | 2026-08-18 | Official narrative media connected to the BMI-era storyline; exact placement relative to all DIVISIONS events remains partly unresolved. |
| SRC-0007 | Graphic Novel | *The Prox Transmissions* | Marvel Entertainment; Dustin Bates; Peter David | Tier III | Active | 2026-08-18 | Official adaptation of the first novel; authoritative where compatible with Tier I. |
| SRC-0008 | Demonstration Series | *IMMERSION: THE FINAL CHAPTER* | STARSET | Tier II | Active | 2026-08-18 | 2024 demonstrations framed as conclusions to existing dystopian narrative threads. |
| SRC-0009 | Album | *SILOS* | STARSET | Tier II | Active | 2026-08-18 | Fifth studio album, released 2026-01-09; contains explicit Order/PROX-facing titles as well as continuation-era material. |
| SRC-0010 | Music Video | “WHERE THE SKIES END” | STARSET | Tier II | Active | 2026-08-18 | Official DIVISIONS-era visual narrative featuring New East propaganda, BMI control, and supplication imagery. |
| SRC-0011 | Music Video | “THE BREACH” | STARSET | Tier II | Active | 2026-08-18 | Official HORIZONS-era visual narrative involving BMI-era social control and escape imagery. |

## Future Source Types

The registry may include novels, albums, songs, music videos, comics, demonstrations, ARG entries, official websites, interviews, social-media records, and creator statements.

## Related Documents

- [`../Governance/EDITORIAL_POLICY.md`](../Governance/EDITORIAL_POLICY.md)
- [`../Specifications/CITATION_GUIDE.md`](../Specifications/CITATION_GUIDE.md)
- [`OBJECT_REGISTRY.md`](OBJECT_REGISTRY.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.1.0 | 2026-08-18 | Added Vessels, DIVISIONS, HORIZONS, the Marvel adaptation, IMMERSION: THE FINAL CHAPTER, SILOS, and two official BMI-era music videos for CH-0002. |
| 1.0.0 | 2026-08-05 | Added publisher, verification date, availability rules, and source-authority cross-reference. |