# CHANGELOG

All notable changes to the Namibia 30 Index (NAX30) repository will be documented in this file.

This project adheres to structured versioning principles.  
Version tags correspond to formal repository releases.

---

## [v1.0.1] – 2026-02-27

### Added
- VERSIONING_POLICY.md establishing formal semantic versioning framework (MAJOR.MINOR.PATCH).
- Index continuity and forward-application control provisions.
- Backward compatibility and deprecation framework.
- Governance reference requirements (proposal ID, timelock ID, transaction hash).
- Smart contract and dependency version lock disclosure standards.
- Oracle schema versioning and quorum classification rules.
- Emergency versioning protocol.
- Multi-document synchronization requirement.

### Documentation
- Strengthened institutional-grade governance and release discipline across repository.

### Smart Contracts
- No changes to deployed smart contracts.
- No changes to token supply.
- No changes to oracle quorum.

---

## [1.0.0] – 2026-02-27

### Added
- Section 5.1 added to INDEX_METHODOLOGY.md documenting initial base weight allocation:
  - 10 constituents assigned 334 basis points
  - 20 constituents assigned 333 basis points
  - Total normalized weight: 10,000 basis points
  - Clarifies integer-based equal-weight normalization in on-chain registry
 
---

## [1.0.0] – 2026-02-26

### Added
- DOCUMENTATION_LICENSE.md (Proprietary Benchmark IP framework)
- README Intellectual Property Notice

### Notes
No smart contract modifications.
Documentation governance clarification only.

---

## [1.0.0] – 2026-02-26
### Initial Institutional Governance Baseline Release

This is the first formal release of the NAX30 institutional benchmark framework.

### Added

- Institutional Whitepaper (Version 2.0 – Governance Edition)
- INDEX_METHODOLOGY.md
- ORACLE_POLICY.md (2-of-3 quorum framework)
- GOVERNANCE_CHARTER.md
- INDEX_COMMITTEE_CHARTER.md
- RISK_COMMITTEE_CHARTER.md
- CHANGE_CONTROL_POLICY.md (Institutional Standard)
- BENCHMARK_STATEMENT_OF_COMPLIANCE.md
- CONFLICT_OF_INTEREST_POLICY.md
- RISK_DISCLOSURE.md
- DATA_PROVIDER_DISCLOSURE.md
- BUSINESS_CONTINUITY_PLAN.md
- INDEX_CALCULATION_AGENT_POLICY.md
- AUDIT_STATUS.md
- EXTERNAL_AUDIT_PLAN.md
- REGULATORY_MEMORANDUM.md
- LEGAL_OPINION_SUMMARY.md
- ADMINISTRATOR_FRAMEWORK.md
- FULL_TECHNICAL_ARCHITECTURE_DOCUMENT.md
- Institutional README.md (Version 2.0)

### Smart Contract Status

- Deployed on BNB Smart Chain (Mainnet)
- Upgradeable proxy architecture
- Governance via Multi-Signature Safe + TimelockController
- Oracle quorum: 2-of-3
- Maximum Supply: 10,000,000,000 NAX30

### Notes

This release formalizes governance and documentation baseline.
No smart contract logic changes were introduced in this release.
