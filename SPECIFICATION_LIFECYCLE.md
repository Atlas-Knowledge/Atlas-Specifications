# Specification Lifecycle

## Overview

The Atlas Specification Lifecycle defines the maturity model for all normative specifications published within the Atlas ecosystem.

The lifecycle ensures that every specification progresses through clearly defined stages before being considered stable for implementation.

Each stage reflects the specification's level of review, consensus, and implementation readiness.

---

# Lifecycle Goals

The lifecycle exists to:

- Ensure specification quality.
- Encourage technical review.
- Prevent unstable specifications from becoming normative.
- Support long-term maintainability.
- Provide predictable evolution.

---

# Lifecycle States

Every Atlas specification MUST exist in exactly one lifecycle state.

```
Draft

↓

Review

↓

Approved

↓

Stable

↓

Deprecated

↓

Archived
```

---

# Draft

A Draft specification represents the initial normative proposal.

Characteristics:

- Under active development.
- Subject to significant revisions.
- Not recommended for production implementations.

Draft specifications MAY change without preserving compatibility.

---

# Review

The Review state indicates that the specification is technically complete and awaiting evaluation.

Review activities include:

- Editorial review
- Technical review
- Cross-specification consistency review
- Compatibility assessment

Review comments SHOULD be documented.

---

# Approved

An Approved specification has successfully completed all required reviews.

Characteristics:

- Normative requirements finalized.
- Architecture validated.
- Ready for publication.

Approved specifications SHOULD remain stable until publication.

---

# Stable

Stable specifications represent the canonical version intended for production use.

Characteristics:

- Recommended for implementation.
- Backward compatibility expected.
- Normative requirements considered authoritative.

Only Stable specifications SHOULD be used as implementation targets.

---

# Deprecated

A specification becomes Deprecated when:

- A newer specification replaces it.
- Architectural evolution supersedes it.
- Significant limitations have been identified.

Deprecated specifications SHOULD remain publicly accessible.

Existing implementations MAY continue using deprecated specifications temporarily.

---

# Archived

Archived specifications are retained for historical reference.

Characteristics:

- No further maintenance.
- No future revisions.
- Preserved for traceability.

Archived specifications MUST NOT be removed from the repository.

---

# Lifecycle Transitions

Allowed transitions are:

```
Draft
   │
   ▼
Review
   │
   ▼
Approved
   │
   ▼
Stable
   │
   ▼
Deprecated
   │
   ▼
Archived
```

Skipping lifecycle stages SHOULD NOT occur except under exceptional governance decisions.

---

# Version Evolution

Lifecycle progression and versioning are independent.

Example:

```
AKS-0001

Draft
Version 0.1.0

↓

Review
Version 0.8.0

↓

Approved
Version 1.0.0

↓

Stable
Version 1.0.0

↓

Stable
Version 1.1.0
```

---

# Responsibilities

## Authors

Responsible for preparing Draft specifications.

## Reviewers

Responsible for evaluating technical correctness and consistency.

## Maintainers

Responsible for approving lifecycle transitions.

---

# Conformance Expectations

Only Stable specifications SHOULD be considered normative implementation targets.

Draft and Review specifications SHOULD NOT be treated as production requirements.

---

# Deprecation Policy

Deprecation MUST include:

- Reason for deprecation.
- Recommended replacement.
- Compatibility guidance.
- Migration recommendations.

---

# Archival Policy

Archived specifications MUST preserve:

- Original identifier.
- Version history.
- Historical references.
- Normative content.

Archived specifications MUST remain immutable.

---

# References

Normative references:

- ASF-0001 — Atlas Specification Framework
- GOVERNANCE.md
- VERSIONING.md

---

# Guiding Statement

> Specifications evolve through disciplined governance, not through uncontrolled change.
