# ATA-1 — Trust Anchor Type 1

**ATA-1** is an open, machine-readable standard for cryptographic timestamping and
integrity anchoring of regulatory evidence files.

It defines how organisations can prove that a specific document, dataset, or record
existed in a specific state at a specific point in time — without relying on narrative
assertions or manual attestations.

---

## Purpose

Modern regulatory regimes require evidence, not explanations.

ATA-1 provides a neutral mechanism to anchor evidence files (spreadsheets, invoices,
logs, minutes, datasets) using cryptographic hashes and verifiable timestamps so that
auditors, regulators, and boards can independently verify integrity.

ATA-1 does **not** certify compliance.  
It provides **proof of existence and non-tampering**.

---

## Regulatory Alignment

ATA-1 is designed to support evidence integrity requirements under:

- **AASB S2** — Climate-related Financial Disclosures (Australia)
- **ASSA / ISSA 5000** — Sustainability Assurance Standards
- **Corporations Act (Cth)** — Sustainability record-keeping obligations
- Comparable regimes in the EU, UK, and United States

ATA-1 is jurisdiction-neutral and may be used alongside any reporting framework.

---

## How It Works

1. A source file is hashed using SHA-256.
2. The hash is timestamped and signed.
3. The resulting anchor record is stored or referenced.
4. Any party can later verify that the file has not changed since anchoring.

---

## What ATA-1 Is Not

- Not a legal opinion  
- Not a compliance guarantee  
- Not an emissions calculator  
- Not a reporting framework  

ATA-1 is an **integrity primitive**.

---

## Relationship to Other Standards

ATA-1 is designed to be referenced by higher-level documentation and disclosure
standards, including:

- Model documentation schemas
- Energy and emissions ledgers
- Evidence manifests and assurance bundles

ATA-1 provides the temporal integrity layer those standards depend on.

---

## Status

Initial public release — January 2026  
Version: 0.1  

This specification is intentionally minimal and stable.
