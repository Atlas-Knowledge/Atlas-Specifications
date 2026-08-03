# Versioning

## Overview

Atlas Specifications use Semantic Versioning (SemVer) to communicate compatibility, maturity, and change history.

Version numbers provide predictable expectations for specification consumers, implementers, and maintainers.

The version format is:

```
MAJOR.MINOR.PATCH
```

Example:

```
1.0.0
```

---

# Version Components

## MAJOR

Increment the MAJOR version when incompatible normative changes are introduced.

Examples:

- Removing mandatory requirements.
- Changing semantic meaning.
- Breaking backward compatibility.
- Redefining core concepts.

Example:

```
1.0.0

↓

2.0.0
```

---

## MINOR

Increment the MINOR version when backward-compatible functionality or requirements are added.

Examples:

- New optional sections.
- Additional informative appendices.
- New extension points.
- Additional normative requirements that do not break existing implementations.

Example:

```
1.2.0

↓

1.3.0
```

---

## PATCH

Increment the PATCH version for editorial corrections and clarifications.

Examples:

- Typographical corrections.
- Grammar improvements.
- Clarifications.
- Formatting updates.
- Non-normative examples.

PATCH versions MUST NOT introduce new normative requirements.

Example:

```
1.3.0

↓

1.3.1
```

---

# Compatibility Rules

## Backward Compatible

MINOR and PATCH releases SHOULD remain backward compatible.

Implementations conforming to a previous MINOR version SHOULD remain compliant unless explicitly documented.

---

## Breaking Changes

Breaking normative changes MUST require:

- A MAJOR version increment.
- Compatibility analysis.
- Migration guidance.
- Updated conformance requirements.

---

# Version Lifecycle

Versions evolve independently of lifecycle state.

Example:

```
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

# Requirement Stability

Requirement identifiers MUST remain stable whenever possible.

Example:

```
AKS-REQ-0001
```

A requirement identifier SHOULD NOT change solely because the specification version changes.

---

# Change Categories

Every published version SHOULD include a change summary.

Changes are classified as:

## Editorial

No normative impact.

## Clarification

Improves interpretation without changing requirements.

## Extension

Introduces backward-compatible functionality.

## Breaking

Changes normative behavior or compatibility.

---

# Deprecation

Deprecated requirements SHOULD remain documented until removed in a future MAJOR version.

Deprecation notices SHOULD include:

- Reason
- Replacement
- Migration Guidance

---

# Version History

Each specification SHOULD maintain a version history table.

Example:

| Version | Status | Summary |
|---------|--------|---------|
| 0.1.0 | Draft | Initial draft |
| 0.8.0 | Review | Technical review |
| 1.0.0 | Stable | Initial stable release |

---

# References

Normative references:

- ASF-0001 — Atlas Specification Framework
- SPECIFICATION_LIFECYCLE.md
- GOVERNANCE.md

---

# Guiding Statement

> Version numbers communicate compatibility, not merely chronology.
