# ATA-1 Verifier

The ATA-1 Verifier defines the canonical verification logic for evaluating
ATA-1 Trust Anchor records.

Any system, auditor, registry, or tool claiming to verify ATA-1–anchored
evidence MUST implement the procedures defined in this repository
or produce functionally equivalent results.


---

## Verification Inputs

To verify an ATA-1 anchor, the verifier requires:

- The original evidence file
- The corresponding ATA-1 anchor record
- The declared hashing algorithm (SHA-256)

---

## Verification Procedure

1. Recompute the SHA-256 hash of the evidence file.
2. Compare the computed hash to the `evidence_hash` field in the anchor.
3. Confirm the anchor timestamp is valid RFC 3339 UTC format.
4. Confirm the anchor structure conforms to `ata-1.schema.json`.

If all checks pass, the anchor is considered **valid**.

---

## Verification Output

A verification process MUST produce one of the following outcomes:

- `VALID` — Evidence matches anchor with no discrepancies
- `INVALID` — Hash mismatch or malformed anchor
- `UNDETERMINED` — Missing or incomplete inputs

---

## Role of the Verifier

The ATA-1 Verifier:

- Confirms data integrity
- Confirms temporal anchoring
- Does NOT assess correctness of disclosures
- Does NOT provide assurance or certification

---

## Reference Implementations

Third parties may implement verifiers in any language or platform,
provided outputs are consistent with this specification.

This document is the canonical reference.
