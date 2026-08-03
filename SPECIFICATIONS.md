# Atlas Specifications Registry

## Overview

This document serves as the official registry of all normative specifications published within the Atlas Specifications repository.

Each specification is uniquely identified, versioned, and tracked throughout its lifecycle.

---

# Specification Registry

| Identifier | Name | Category | Version | Status |
|------------|------|----------|---------|--------|
| ASF-0001 | Atlas Specification Framework | Framework | 1.0.0 | Draft |
| ACCS-0001 | Atlas Common Concepts Specification | Foundation | 1.0.0 | Draft |
| AKS-0001 | Atlas Knowledge Specification | Knowledge | 1.0.0 | Draft |
| AES-0001 | Atlas Evidence Specification | Evidence | Planned | Planned |
| ARS-0001 | Atlas Reasoning Specification | Reasoning | Planned | Planned |
| AVS-0001 | Atlas Validation Specification | Validation | Planned | Planned |
| ADS-0001 | Atlas Discovery Specification | Discovery | Planned | Planned |
| AMS-0001 | Atlas Metadata Specification | Metadata | Planned | Planned |
| AIS-0001 | Atlas Interoperability Specification | Interoperability | Planned | Planned |

---

# Dependency Graph

```
ASF-0001
    │
    ▼
ACCS-0001
    │
    ▼
AKS-0001
    │
    ├────────────┐
    ▼            ▼
AES-0001     ARS-0001
    │            │
    └─────┐ ┌────┘
          ▼ ▼
       AVS-0001
          │
          ▼
       ADS-0001
          │
          ▼
       AMS-0001
          │
          ▼
       AIS-0001
```

---

# Specification Categories

## Framework

Defines how Atlas specifications are written and governed.

- ASF-0001

---

## Foundation

Defines the common concepts shared across all Atlas specifications.

- ACCS-0001

---

## Knowledge

Defines the Atlas Knowledge Model.

- AKS-0001

---

## Evidence

Defines evidence representation and provenance.

- AES-0001

---

## Reasoning

Defines reasoning models and inference.

- ARS-0001

---

## Validation

Defines validation rules and conformance evaluation.

- AVS-0001

---

## Discovery

Defines discovery models and knowledge generation.

- ADS-0001

---

## Metadata

Defines metadata structures and semantics.

- AMS-0001

---

## Interoperability

Defines interoperability requirements and exchange models.

- AIS-0001

---

# Lifecycle Status

Specifications may exist in one of the following states:

- Draft
- Review
- Approved
- Stable
- Deprecated
- Archived

The lifecycle is defined by:

- SPECIFICATION_LIFECYCLE.md

---

# Version Policy

Specifications follow Semantic Versioning.

```
MAJOR.MINOR.PATCH
```

Example:

```
1.0.0
```

Versioning rules are defined in:

- VERSIONING.md

---

# Governance

All specification changes follow the Atlas governance process.

```
Proposal

↓

RFC

↓

Review

↓

Approval

↓

Publication
```

Governance rules are defined in:

- GOVERNANCE.md
- SPECIFICATION_PROCESS.md

---

# Conformance

Reference implementations MUST implement the normative requirements defined by the corresponding specification.

Conformance is evaluated through Atlas Standards and Atlas Test Suites.

---

# Repository Relationships

```
Atlas-Core

↓

Atlas-Specifications

↓

Atlas-Standards

↓

Atlas-Kernel

↓

Atlas-SDK

↓

Applications
```

---

# References

Normative references:

- ASF-0001
- ACCS-0001
- SPECIFICATION_PROCESS.md
- SPECIFICATION_LIFECYCLE.md
- VERSIONING.md

---

# Guiding Statement

> The Atlas Specification Registry provides the canonical index of all normative specifications within the Atlas ecosystem.
