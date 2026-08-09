# Style Guide

| Field | Value |
|---|---|
| Document ID | DOC-GOV-0007 |
| Category | Governance |
| Status | Accepted |
| Version | 1.0.0 |
| Last Updated | 2026-08-05 |

## Purpose

This document defines the written and visual presentation standards for **The STARSET Codex**.

## Voice

Writing SHALL be:

- Professional.
- Neutral.
- Clear.
- Evidence-conscious.
- Immersive when using the STARSET Society archival framing.

Writing SHOULD remain accessible to readers unfamiliar with the lore while retaining enough precision for experienced researchers.

## Tense

- Use past tense for chronological in-universe events.
- Use present tense when discussing what a source says, shows, or contains.
- Use future tense only for genuinely future work or in-universe predictions.

**Example:**

> Tesla constructed Wardenclyffe Tower. The novel presents the tower as part of a larger hidden conflict.

## Capitalization and Terminology

- Use official names exactly as published.
- Preserve official capitalization for albums, organizations, technologies, and named events.
- Italicize album, book, comic, and other standalone work titles.
- Use quotation marks for song titles.
- Do not create unofficial abbreviations without defining them.

When terminology differs across sources, use the preferred current term and document historical variants where relevant.

## Paragraphs

Paragraphs SHOULD focus on one claim or closely related group of claims. Dense lore summaries should be divided when source attribution, confidence, or chronology changes.

## Headings

- Use one `#` heading for the document title.
- Use `##` for major sections.
- Use `###` for subsections.
- Avoid heading levels deeper than `####` unless necessary.
- Do not skip heading levels.

## Requirement Language

Standards documents use the following terms:

- **SHALL / MUST:** mandatory.
- **SHOULD:** strongly recommended; deviations require a reason.
- **MAY:** optional.

Narrative lore chapters should avoid RFC wording unless discussing project requirements.

## Lists

Use numbered lists when order matters and bullets when it does not.

**Example:** The contradiction-resolution procedure uses a numbered sequence because the order is meaningful.

## Quotations

Direct quotations SHALL be exact, attributed, and cited. Editors should prefer concise quotations and paraphrase when full wording is unnecessary.

## Canon Confidence Labels

Confidence labels must use the names and meanings defined in [`../Specifications/CANON_CONFIDENCE.md`](../Specifications/CANON_CONFIDENCE.md). Do not invent intermediate levels.

## Archivist Notes

Archivist Notes are optional, visually distinct contextual callouts. They MAY connect evidence, explain ambiguity, or preserve the archival tone, but they must not introduce unsupported facts.

Recommended Markdown form:

> **Archivist's Note — ARC-0001**  
> The surviving records disagree on the date. See the contradiction analysis below.

## Figures, Diagrams, and Maps

Every visual asset SHALL include:

- Permanent ID.
- Title or caption.
- Source or creator attribution.
- Revision.
- Confidence level when the asset reconstructs uncertain information.

**Examples:**

- `FIG-0012 — Wardenclyffe Tower photograph.`
- `DIG-0004 — Evolution of the Everything Machine.`
- `MAP-0003 — Confirmed and inferred North American lore locations.`

## Tables

Tables SHOULD be used for concise structured comparison, not long narrative passages. Every column must have a clear purpose.

## Dates

Use ISO format (`YYYY-MM-DD`) in metadata and governance records. Narrative chapters may use reader-friendly dates when appropriate, but uncertain dates must be labeled.

## Cross-References

Cross-references SHALL use stable identifiers and descriptive link text.

**Good:** `See CH-0009, Order of Teslonia.`

**Bad:** `See the chapter above.`

## Publishable Chapter Rule

Every chapter SHALL:

- Explain its essential subject without requiring another chapter.
- Include its own citations and source subset.
- Include its own revision history.
- Include all required assets and companion files.
- Export to a standalone PDF without manual rewriting.

Cross-references may provide deeper context but cannot substitute for essential explanation.

## Related Documents

- [`EDITORIAL_POLICY.md`](EDITORIAL_POLICY.md)
- [`../Specifications/CHAPTER_TEMPLATE.md`](../Specifications/CHAPTER_TEMPLATE.md)
- [`../Specifications/ASSET_GUIDE.md`](../Specifications/ASSET_GUIDE.md)
- [`../Specifications/CITATION_GUIDE.md`](../Specifications/CITATION_GUIDE.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.0.0 | 2026-08-05 | Added complete voice, tense, terminology, formatting, RFC-language, callout, visual, cross-reference, and publishable-chapter standards. |
