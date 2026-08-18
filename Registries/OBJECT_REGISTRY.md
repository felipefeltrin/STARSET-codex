# Object Registry

| Field | Value |
|---|---|
| Document ID | DOC-REG-0001 |
| Category | Registry |
| Status | Active |
| Version | 1.0.1 |
| Last Updated | 2026-08-09 |

## Purpose

The Object Registry is the authoritative database of every permanent non-source identifier allocated within **The STARSET Codex**.

## Registry Rules

- Identifiers SHALL be allocated before publication.
- Identifiers SHALL be immutable and SHALL never be reused.
- A deprecated object retains its identifier and registry entry.
- New identifier types must first be added to [`../Specifications/ID_STANDARDS.md`](../Specifications/ID_STANDARDS.md).
- Status values are `Planned`, `Draft`, `Review`, `Published`, or `Deprecated`.
- `Owner` identifies the maintainer, team, or project area responsible for the object.
- `First Release` records the first public release containing the object; use `Unreleased` during development.

## Registered Objects

| ID | Type | Name | Status | Revision | Owner | First Release | Notes |
|---|---|---|---|---|---|---|---|
| DOC-GOV-0001 | Governance Document | Contributing | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-GOV-0002 | Governance Document | Architectural Decisions | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-GOV-0003 | Governance Document | Editorial Policy | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-GOV-0004 | Governance Document | Project Glossary | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-GOV-0005 | Governance Document | Project Roadmap | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-GOV-0006 | Governance Document | Review Process | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-GOV-0007 | Governance Document | Style Guide | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-SPEC-0001 | Specification | Asset Guide | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-SPEC-0002 | Specification | Canon Confidence | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-SPEC-0003 | Specification | Chapter Template | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-SPEC-0004 | Specification | Citation Guide | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-SPEC-0005 | Specification | Identifier Standards | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-SPEC-0006 | Specification | Metadata Specification | Published | 1.0.0 | Core Maintainers | Unreleased | |
| DOC-REG-0001 | Registry Document | Object Registry | Published | 1.0.1 | Core Maintainers | Unreleased | Self-registering entry. |
| DOC-REG-0002 | Registry Document | Source Registry | Published | 1.0.0 | Core Maintainers | Unreleased | |
| CH-0001 | Chapter | Introduction | Draft | 1.0.0 | Content Team | Unreleased | First lore-content package. |
| SSA-0100 | Archive Document | Chapter 1 Archive Header | Draft | 1.0.0 | Content Team | Unreleased | Public-release archival framing for CH-0001. |
| ARC-0001 | Archive Document | Archivist Note: Record and Archivist | Draft | 1.0.0 | Content Team | Unreleased | Clarifies that archival framing cannot create canon evidence. |
| CIT-0001 | Citation | The Prox Transmissions foundational-source citation | Draft | 1.0.0 | Content Team | Unreleased | Used by CH-0001. |
| CIT-0002 | Citation | A Brief History of the Future foundational-source citation | Draft | 1.0.0 | Content Team | Unreleased | Used by CH-0001. |
| CIT-0003 | Citation | Transmissions foundational-source citation | Draft | 1.0.0 | Content Team | Unreleased | Used by CH-0001. |

## Related Documents

- [`../Specifications/ID_STANDARDS.md`](../Specifications/ID_STANDARDS.md)
- [`SOURCE_REGISTRY.md`](SOURCE_REGISTRY.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.0.1 | 2026-08-09 | Registered CH-0001 and its initial archive and citation objects. |
| 1.0.0 | 2026-08-05 | Added ownership, first-release tracking, document registrations, and registry rules. |