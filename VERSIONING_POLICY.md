# NAX30 VERSIONING POLICY

Namibia 30 Index (NAX30)

Version 2.0  
Effective Date: February 2026  

---

## 1. Purpose

This Versioning Policy defines the structured framework governing version control for the Namibia 30 Index (NAX30) documentation, methodology, governance framework, and smart contract architecture.

The objective is to ensure:

- Transparent change tracking
- Audit traceability
- Regulatory defensibility
- Deterministic release control
- Institutional-grade governance discipline
- Historical index continuity
- Forward-only methodological application

---

## 2. Versioning Standard

NAX30 follows a structured semantic versioning framework:

MAJOR.MINOR.PATCH

Example:

1.0.0

Version tags must follow:

vX.Y.Z

Example:

v1.0.0  
v1.0.1  
v1.1.0  
v2.0.0  

Release titles may include descriptive text, but semantic tag format must remain consistent.

---

## 3. Version Classifications

### 3.1 MAJOR Version (X.0.0)

A MAJOR version increment reflects structural changes, including:

- Smart contract architecture modifications
- Token logic changes
- Governance framework restructuring
- Oracle quorum redesign
- Fundamental index calculation formula changes
- Maximum supply modification
- Registry schema redesign
- Proxy upgrade affecting state variables

MAJOR changes require:

- Governance approval
- Timelock scheduling
- Public documentation update
- CHANGELOG entry
- Formal repository release tag
- Governance proposal reference ID
- Timelock operation ID
- On-chain transaction hash documentation

---

### 3.2 MINOR Version (X.Y.0)

A MINOR version increment reflects functional or policy enhancements that do not alter core architecture, including:

- Methodology refinements
- Weighting framework adjustments
- Rebalancing framework clarification
- Governance policy additions
- Risk disclosure updates
- Oracle configuration changes (non-structural)
- Documentation structure expansion

MINOR changes require:

- Documentation update
- CHANGELOG entry
- Release tag
- Governance reference if applicable

Backward compatibility must be preserved unless explicitly stated.

---

### 3.3 PATCH Version (X.Y.Z)

A PATCH version increment reflects:

- Documentation clarifications
- Typographical corrections
- Transparency enhancements
- Non-structural disclosures
- Administrative refinements

PATCH changes do not alter:

- Smart contract logic
- Governance structure
- Weight normalization
- Index formula
- Registry architecture
- Oracle quorum

PATCH releases do not require governance vote unless operationally necessary.

---

## 4. Index Continuity Principle

Version changes shall not reset the index base level.

The NAX30 base level (10,000 basis points) remains continuous across all versions unless explicitly reconstituted via MAJOR structural redesign.

Historical time-series data shall remain intact and publicly auditable.

Version increments apply prospectively and do not retroactively alter previously published index levels.

---

## 5. Effective Date & Forward Application

Each version must include:

- Effective Date (ISO 8601 format)
- Forward application statement

Methodology changes apply only from the effective date forward.

Retroactive recalculation of historical index values is prohibited unless required to correct material error, in which case:

- Governance approval is required
- Public disclosure must be issued
- A correction log must be appended to CHANGELOG.md

---

## 6. Backward Compatibility Policy

MINOR and PATCH releases must preserve backward compatibility.

MAJOR releases may introduce structural changes that affect compatibility.

In such cases:

- Historical calculation framework remains archived
- Prior methodology version remains publicly accessible
- Comparative reference documentation must be maintained

---

## 7. Deprecation & Archival Policy

Superseded versions:

- Remain permanently archived in repository history
- May not be deleted
- Must remain accessible for audit and regulatory review

Deprecated methodology documents shall be clearly labeled as “Superseded.”

---

## 8. Smart Contract Versioning

Smart contract deployments are tracked through:

- Proxy address
- Implementation contract address
- Governance proposal reference
- Timelock operation ID
- On-chain execution transaction hash
- Compiler version
- Dependency version (OpenZeppelin, Safe)

Each contract upgrade must correspond to a MAJOR or MINOR repository version increment.

Silent contract changes are prohibited.

---

## 9. Data Schema & Oracle Versioning

Any modification to:

- Oracle payload format
- Registry storage structure
- Event signatures
- State variable layout

Requires:

- MAJOR or MINOR version increment
- Explicit schema documentation
- Governance execution reference

Oracle quorum adjustments require MAJOR version increment.

---

## 10. Dependency Version Lock

Each release must document:

- Solidity compiler version
- OpenZeppelin library version
- Safe contract version
- Any external protocol dependencies

Dependency modifications require at minimum a MINOR version increment.

---

## 11. Public Notice & Communication

MAJOR structural releases should:

- Provide advance notice where feasible
- Be published prior to or concurrent with timelock execution
- Include summary of impact

Emergency changes must be disclosed immediately following execution.

---

## 12. Emergency Versioning Protocol

In case of critical security or integrity event:

- Emergency governance action may be executed
- A MAJOR or MINOR version must be assigned
- Post-event disclosure must be published
- Incident reference must be included in CHANGELOG

Emergency actions do not bypass documentation requirements.

---

## 13. Multi-Document Synchronization Rule

If changes affect:

- Methodology
- Governance framework
- Oracle policy
- Risk disclosure
- Calculation formula

All related documents must be updated in the same release cycle.

Version drift between documents is prohibited.

---

## 14. CHANGELOG Requirement

All version increments must:

- Be recorded in CHANGELOG.md
- Use ISO 8601 date format (YYYY-MM-DD)
- Clearly state whether contract logic changed
- Reference affected documents
- Include governance reference where applicable

---

## 15. Governance Alignment

Version increments must align with:

- GOVERNANCE_CHARTER.md
- CHANGE_CONTROL_POLICY.md
- RISK_COMMITTEE_CHARTER.md
- INDEX_COMMITTEE_CHARTER.md

No version increment may bypass governance procedures.

---

## 16. Structural Classification Statement

NAX30 remains:

- Fixed maximum supply
- Governance-controlled mint
- Non-redeemable
- Market-priced

Versioning does not alter structural classification unless explicitly declared in a MAJOR release.

---

End of Versioning Policy.
