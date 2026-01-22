# ATA-1 Registry

The ATA-1 Registry defines the reference process for issuing, recording, and verifying
ATA-1 Trust Anchor records.

This repository does not provide a public anchoring service.
It defines the minimum operational requirements for any entity
claiming to operate an ATA-1–compatible registry.

---

## Purpose

The registry exists to:
- Establish a single source of truth for issued ATA-1 anchors
- Enable independent verification of anchor integrity
- Prevent duplicate or conflicting trust anchor claims

---

## Registry Authority

An ATA-1 Registry operator MAY issue trust anchor records.

An ATA-1 Registry operator SHALL:
- Maintain immutable logs of issued anchors
- Preserve timestamp integrity
- Provide verifiable proof of issuance on request

The reference registry for ATA-1 is determined by adoption and citation,
not by declaration.

---

## Separation of Roles

This specification intentionally separates:
- **The Standard** (ATA-1 core)
- **The Verification Logic** (verifier)
- **The Registry Operation** (this document)

This separation ensures neutrality of the standard
while allowing commercial registry operation.

---

## Status

Registry specification — Draft  
Aligned with ATA-1 Core Specification v0.1
