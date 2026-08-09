# Canon Confidence

| Field | Value |
|---|---|
| Document ID | DOC-SPEC-0002 |
| Category | Specification |
| Status | Accepted |
| Version | 1.0.0 |
| Last Updated | 2026-08-05 |

## Purpose

Canon Confidence measures how strongly available evidence supports a specific claim. It does not replace the canon hierarchy and does not measure how personally convincing a theory feels.

## Core Rule

Editors SHALL choose the lowest confidence level that honestly fits the available evidence.

## Levels

### 🟢 Confirmed Canon

Use when an official source explicitly states or unambiguously depicts the claim and no higher-priority source contradicts it.

**Example:** Thomas Bell appears in *The Prox Transmissions*.

A claim does not become Confirmed merely because many fans accept it.

### 🟡 Strongly Supported

Use when multiple independent official sources support the same conclusion, but no source states it directly enough for Confirmed Canon.

**Example:** Two separate official narrative sources place the same organization in the same broader conflict without explicitly naming its complete role.

Sources that merely repeat the same promotional statement are not independent evidence.

### 🟠 Reasonable Reconstruction

Use when the claim is the most coherent conclusion from official evidence but requires inference, estimation, synthesis, or spatial reconstruction.

**Example:** A facility's approximate real-world location is estimated from travel times and geographical descriptions.

The claim must explain the inference and identify its limits.

### 🔴 Community Theory

Use when the interpretation lacks sufficient direct official support, depends primarily on symbolism, or represents one of several plausible readings.

**Example:** A song narrator is identified as a specific character solely from thematic similarity.

Community Theory does not mean worthless; it means unconfirmed.

## Decision Flow

- `Explicitly stated or unambiguously depicted? -> Yes -> Confirmed Canon`
- `Explicitly stated or unambiguously depicted? -> No -> Supported independently by multiple official sources? -> Yes -> Strongly Supported`
- `Supported independently by multiple official sources? -> No -> Evidence-based inference required? -> Yes -> Reasonable Reconstruction`
- `Evidence-based inference required? -> No, or evidence is insufficient -> Community Theory`

If a higher-priority source contradicts the claim, stop and resolve the contradiction under [`../Governance/EDITORIAL_POLICY.md`](../Governance/EDITORIAL_POLICY.md) before assigning confidence.

## Scoring Considerations

Editors SHOULD consider:

- **Explicitness:** Is the claim directly stated?
- **Source authority:** What tiers support or contradict it?
- **Independence:** Are supporting sources genuinely separate?
- **Specificity:** Does the evidence support the exact claim or only a broader idea?
- **Inference distance:** How many assumptions are required?
- **Alternative explanations:** Are other readings equally plausible?
- **Source integrity:** Is the material complete, authenticated, and available in context?

Confidence SHALL NOT be calculated as a simple numerical average. The system is categorical because source authority and contradiction cannot be represented honestly by raw point totals alone.

## Mixed Claims

A paragraph containing claims with different confidence levels SHOULD be divided or label each claim separately.

**Bad:** A paragraph mixes a confirmed event, an inferred date, and a fan interpretation under one green label.

**Good:** The event is marked Confirmed, the date is marked Reasonable Reconstruction, and the interpretation is marked Community Theory.

## Confidence Changes

Confidence may increase or decrease when new evidence appears. The claim retains its historical revision record, and published releases remain immutable.

## Related Documents

- [`../Governance/EDITORIAL_POLICY.md`](../Governance/EDITORIAL_POLICY.md)
- [`CITATION_GUIDE.md`](CITATION_GUIDE.md)
- [`../Governance/REVIEW_PROCESS.md`](../Governance/REVIEW_PROCESS.md)

## Revision History

| Version | Date | Change |
|---|---|---|
| 1.0.0 | 2026-08-05 | Added a decision flow, evidence factors, mixed-claim handling, and confidence revision rules. |
