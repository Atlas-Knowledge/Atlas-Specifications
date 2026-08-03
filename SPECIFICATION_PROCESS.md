# Specification Process

## Overview

The Atlas Specification Process defines the standard workflow for creating, reviewing, approving, publishing, and maintaining normative specifications.

This process ensures that every Atlas specification is developed consistently, transparently, and independently of any specific implementation.

---

# Guiding Principle

> Specifications are the canonical source of truth.

Implementations MUST follow specifications.

Specifications MUST NOT be derived from implementations.

---

# Specification Workflow

Every specification follows the lifecycle below.

```text
Idea

↓

Proposal

↓

RFC

↓

Draft Specification

↓

Technical Review

↓

Architecture Review (if required)

↓

Approval

↓

Publication

↓

Reference Implementation

↓

Conformance Testing
```

---

# Phase 1 — Idea

A specification begins with the identification of a new capability, concept, or requirement.

Ideas SHOULD describe:

- Motivation
- Problem Statement
- Expected Benefits
- Initial Scope

Ideas are informative only.

---

# Phase 2 — Proposal

A proposal formalizes the idea.

A proposal SHOULD include:

- Title
- Summary
- Scope
- Rationale
- Impact Assessment

Accepted proposals proceed to RFC.

---

# Phase 3 — RFC

Significant specification work SHOULD begin with a Request for Comments (RFC).

The RFC documents:

- Motivation
- Alternatives
- Design Considerations
- Compatibility Analysis
- Risks

RFC review precedes specification drafting.

---

# Phase 4 — Draft Specification

The specification is written according to ASF-0001.

Every specification MUST include:

- Identifier
- Version
- Status
- Scope
- Terminology
- Normative Requirements
- Conformance
- Compatibility
- References

---

# Phase 5 — Technical Review

The draft specification is evaluated for:

- Technical correctness
- Consistency
- Completeness
- Clarity

Review feedback SHOULD be documented.

---

# Phase 6 — Architecture Review

Architecture review is required whenever the specification introduces:

- New foundational concepts
- Breaking changes
- Cross-specification dependencies
- Architectural impacts

Minor editorial revisions do not require architecture review.

---

# Phase 7 — Approval

A specification may be approved when:

- Technical review is complete.
- Required architectural review is complete.
- Normative requirements are complete.
- Compatibility analysis is documented.

Approved specifications become normative.

---

# Phase 8 — Publication

Approved specifications are published within the Atlas Specifications repository.

Publication includes:

- Version
- Status
- Change History
- References

---

# Phase 9 — Reference Implementation

Reference implementations demonstrate compliance.

Reference implementations MUST NOT redefine normative requirements.

Reference implementations SHOULD document implementation decisions separately.

---

# Phase 10 — Conformance Testing

Implementations are evaluated against published specifications.

Conformance testing verifies:

- Mandatory requirements
- Optional capabilities
- Compatibility
- Interoperability

---

# Roles

## Authors

Create and maintain specifications.

## Reviewers

Verify correctness, consistency, and quality.

## Maintainers

Approve, publish, and version specifications.

---

# Specification Principles

Every Atlas specification SHOULD be:

- Technology Neutral
- Deterministic
- Testable
- Traceable
- Extensible
- Backward Compatible whenever practical

---

# Change Management

Changes are classified as:

## Editorial

Clarifications without changing normative meaning.

## Minor

Backward-compatible additions.

## Major

Breaking semantic or normative changes.

Major revisions MAY require:

- RFC
- Architecture Review
- ADR

---

# Deliverables

Each published specification SHOULD provide:

- Normative Specification
- Version History
- Conformance Requirements
- Compatibility Notes
- Informative Examples

---

# References

Normative references:

- ASF-0001 — Atlas Specification Framework
- ACCS-0001 — Atlas Common Concepts Specification
- Atlas Governance

---

# Guiding Statement

> Every Atlas specification follows a predictable, transparent, and reviewable process from idea to implementation.
