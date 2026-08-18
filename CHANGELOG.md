# Changelog

All notable changes to **The STARSET Codex** are documented in this file.

The project follows Semantic Versioning. During pre-release development, versions may use the `-dev` suffix.

## [Unreleased]

### Added

- Initial `CH-0001 — Introduction` publishable chapter package.
- Chapter 1 companion metadata, manifest, and citation records.
- Initial archival objects `SSA-0100` and `ARC-0001`.
- Initial citation objects `CIT-0001` through `CIT-0003`.
- Initial `CH-0002 — Master Chronology` publishable chapter package through *SILOS*.
- Chapter 2 companion metadata, manifest, and citation records.
- Chronology events `EVT-0001` through `EVT-0018`.
- Archive notes `ARC-0002` through `ARC-0004` and archive header `SSA-0101`.
- Citation objects `CIT-0004` through `CIT-0026`.
- Registered source set expanded through `SRC-0011`, adding *Vessels*, *DIVISIONS*, *HORIZONS*, the Marvel adaptation, *IMMERSION: THE FINAL CHAPTER*, *SILOS*, and two official BMI-era music videos.

### Changed

- Project roadmap advanced from governance finalization to content creation.
- Object Registry updated for the first two lore-content chapters.
- Source Registry expanded for the Master Chronology research set.
- The Master Chronology explicitly leaves universal *DIVISIONS*/*HORIZONS* ordering unresolved instead of treating release or fan ordering as settled canon.

## [1.0.0-dev] — 2026-08-05

### Added

- Initial governance, specification, and registry structure.
- Permanent document identifiers for governance, specification, and registry documents.
- Repository-wide contribution, editorial, style, review, asset, metadata, citation, confidence, chapter, and identifier standards.
- Object and source registries.
- Architectural decision record.
- Project roadmap.
- Changelog established from the beginning of the project.

### Changed

- Standardized document structure, RFC requirement language, examples, cross-references, and revision histories.
- Replaced vertical workflow notation with inline right-arrow notation.
- Clarified that YAML metadata must remain in companion files and must never be embedded in Markdown.
- Formalized publishable chapters, immutable releases, single-source-of-truth rules, and buildable repository requirements.

### Removed

- Duplicate canon hierarchy definitions outside `Governance/EDITORIAL_POLICY.md`.
- Temporary comparison copies of `CONTRIBUTING.md` from the packaged repository.