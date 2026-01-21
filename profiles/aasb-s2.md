# ATA-1 Evidence Profile — AASB S2

This document defines the recommended use of the ATA-1 Trust Anchor
Specification when preparing evidence for AASB S2 climate-related
financial disclosures.

---

## Objective

To provide a consistent, verifiable method for anchoring supporting
evidence used in AASB S2 disclosures, enabling auditors and regulators
to independently verify document integrity and timing.

---

## Scope of Evidence

ATA-1 anchoring SHOULD be applied to, but is not limited to:

- Scope 1, 2, and 3 calculation workbooks
- Energy invoices and meter exports
- Emissions factors and assumptions
- Scenario analysis inputs
- Board and committee minutes approving disclosures
- Management sign-off packs

---

## Anchoring Procedure

For each evidence item:

1. Generate a SHA-256 hash of the source file.
2. Create an ATA-1 anchor record referencing the hash.
3. Record the UTC timestamp of anchoring.
4. Preserve the anchor record alongside disclosure materials.

Each anchor MUST be immutable once generated.

---

## Assurance Use

During assurance or audit:

- The auditor may re-hash the source file
- The hash MUST match the ATA-1 anchor
- Any mismatch indicates post-anchor modification

ATA-1

ATA-1 anchors provide objective evidence of non-tampering but do not
replace professional judgement or assurance procedures.

---

## Director and Management Use

ATA-1 anchors may be used to demonstrate that:

- Reasonable steps were taken to preserve disclosure evidence
- Records existed prior to reporting and assurance milestones
- Evidence was not retrospectively altered

---

## Status

This profile is informational and non-mandatory.
It may be referenced by auditors, preparers, and regulators.
