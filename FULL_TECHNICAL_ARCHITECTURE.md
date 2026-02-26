# NAX30 FULL TECHNICAL ARCHITECTURE  
Namibia 30 Index (NAX30)

Version 2.0 – Institutional Technical Architecture  
Effective Date: February 2026  

---

## 1. Purpose

This document describes the technical architecture supporting the Namibia 30 Index (NAX30), including smart contract structure, governance controls, oracle integration, and system design principles.

The objective is to provide:

- Transparent architectural disclosure  
- Smart contract structural clarity  
- Governance execution traceability  
- Upgrade and control boundaries  
- Security posture documentation  

This document is intended to meet institutional-grade disclosure standards consistent with digital financial market infrastructure documentation practices.

---

## 2. System Overview

NAX30 operates as a blockchain-native benchmark instrument deployed on:

- **Network:** BNB Smart Chain (BSC) Mainnet  
- **Token Standard:** ERC-20 compatible (BEP-20)  
- **Decimals:** 18  

The architecture consists of:

1. Upgradeable Token Contract (Proxy Pattern)
2. Implementation Contract
3. Registry Contract (Weights & Constituents)
4. TimelockController
5. Multi-Signature Safe
6. Oracle Framework
7. Governance Execution Layer

All structural components are publicly verifiable on-chain.

---

## 3. Contract Components

### 3.1 NAX30 Proxy (Primary Token Address)

Acts as the user-facing contract.

- Stores token balances
- Forwards logic to Implementation contract
- Upgradeable via governance

Primary Proxy Address:
0xaAd81eb1f27874B8B0CB03C778C6019ea32045Ff

Proxy pattern enforces storage persistence across upgrades.

---

### 3.2 Implementation Contract

Contains token logic including:

- ERC-20 functionality
- Mint function (governance controlled)
- Access control enforcement
- Registry read functions
- Governance authorization checks

Implementation Address:
0x8293C888fFa3601E4197e63f2924E10cA32e5d88

Upgradeable only through governance + timelock execution.

---

### 3.3 Registry Contract

Stores:

- Constituent identifiers
- Weight allocations
- Weight normalization (10,000 bps)
- Registry version history

Registry Address:
0x960cc4EB352c6B920a05Dc3A97BED768E551c4f8

The registry is controlled exclusively through timelock-governed execution.

No direct unilateral modification is possible.

---

### 3.4 TimelockController

Enforces mandatory delay for:

- Registry updates
- Contract upgrades
- Governance parameter changes
- Oracle modifications
- Mint scheduling

Timelock Address:
0xdc38cab671EECbd13D5c8771DC44C5729C2B4267

Timelock guarantees:

- Deterministic operation IDs
- Public scheduling events
- Transparent execution history

Timelock delay duration is publicly verifiable on-chain.

---

### 3.5 Multi-Signature Safe

Holds proposal authority.

Safe Address:
0x397314A5CAA3F891A2d85DAc109be2078b510155

Responsibilities:

- Propose governance actions
- Approve scheduled operations
- Execute timelock submissions

Signature threshold is enforced at contract level and publicly verifiable.

No single signer can unilaterally modify system parameters.

---

## 4. Index Calculation Architecture

Index value calculation is defined by:

NAX30_t = 10,000 × ( Σ (W_i × P_i,t) ) / ( Σ (W_i × P_i,0) )

Where:

W_i = Weight of constituent i  
P_i,t = Current price  
P_i,0 = Base date price  

Weights are stored in Registry.

Price data is sourced via Oracle framework.

Index calculation may be:

- Independently replicated by third parties  
- Computed off-chain using published methodology  
- Validated against registry weights  

Token price does not auto-adjust to calculated value.

No redemption or NAV enforcement mechanism exists.

---

## 5. Oracle Framework

### 5.1 Structure

- Designated oracle operators
- 2-of-3 quorum requirement
- Independent submission verification

Minimum two concurring submissions required for update validity.

### 5.2 Oracle Controls

Oracle modifications require:

- Governance proposal
- Timelock scheduling
- On-chain execution

Oracle failure does not automatically trigger mint or supply modification.

---

## 6. Supply Architecture

Maximum Supply:
10,000,000,000 NAX30

No:

- Algorithmic emissions
- Inflation schedule
- Automatic minting

Minting requires:

1. Governance proposal
2. Timelock scheduling
3. On-chain execution

Supply expansion cannot occur without delay transparency.

Maximum supply is immutable unless explicitly modified via governed upgrade.

---

## 7. Upgradeability Model

NAX30 uses proxy-based upgrade architecture.

Upgrade process:

1. Governance proposal
2. Safe approval
3. Timelock scheduling
4. Execution after delay
5. Public event emission

Upgrades cannot bypass timelock.

Upgrades may modify:

- Logic
- Access controls
- Operational parameters

Upgrades cannot alter historical transaction data.

Storage layout consistency is preserved to prevent state corruption.

---

## 8. Access Control Model

Role-based access controls exist for:

- Mint authority
- Registry modification
- Oracle configuration
- Upgrade authorization

All privileged functions require governance pathway.

No externally owned account (EOA) has unilateral authority.

---

## 9. Data Flow Architecture

1. NSX-listed securities publish official disclosures
2. Oracle operators source validated price inputs
3. Oracle quorum validates updates
4. Index calculation reflects updated weights + prices
5. Market participants trade token in open markets

There is no custody linkage to underlying securities.

Calculation replicability is publicly achievable using:

- Published weights
- Public price data
- Defined formula

---

## 10. Threat Model

Primary adversaries include:

- External attackers (contract exploitation)
- Insider governance collusion
- Oracle collusion
- Key compromise
- Network-level attack (BSC)

Attack surfaces include:

- Proxy upgrade pathway
- Governance scheduling
- Oracle submission layer
- Multi-signature compromise

Mitigations:

- Multi-signature Safe
- Timelock delay
- Public auditability
- Quorum oracle model
- Fixed supply cap

Residual risk remains.

---

## 11. Key Management & Operational Security

Governance signers are expected to:

- Use hardware-secured wallets
- Avoid centralized key storage
- Maintain operational redundancy
- Follow secure key rotation practices

Signer removal or addition requires governance execution.

Compromised keys must be replaced via governed process.

---

## 12. Governance Parameter Disclosure

Publicly verifiable parameters include:

- Safe signature threshold
- Timelock delay duration
- Oracle quorum requirement
- Maximum supply cap

Any modification to these parameters requires governance + timelock.

---

## 13. Immutable vs Mutable Parameters

Immutable (Absent Governance Upgrade):

- Token decimals
- Historical transaction records

Mutable (Governance Controlled):

- Constituent weights
- Oracle addresses
- Implementation logic
- Mint authorization
- Registry contents

All mutable elements require timelock execution.

---

## 14. Event Transparency

Events emitted include:

- ERC-20 Transfer
- Governance scheduling
- Governance execution
- Upgrade execution
- Registry updates

All state modifications are publicly observable.

---

## 15. Monitoring & Observability

System transparency relies on:

- On-chain event indexing
- Public block explorers
- Governance transaction visibility
- Version-controlled documentation

Independent observers may monitor governance scheduling and execution.

---

## 16. Base Layer Network Risk

NAX30 depends on BNB Smart Chain.

Risks include:

- Validator set concentration
- Network reorganization
- Gas price volatility
- Base-layer governance changes

These risks are external to NAX30 smart contract control.

---

## 17. Security Design Principles

System architecture incorporates:

- Minimal external call exposure
- Governance-controlled upgrade path
- No automatic mint emissions
- Deterministic timelock operations
- Public transparency of state changes
- On-chain event logging

Security philosophy emphasizes:

- Governance delay over speed
- Transparency over opacity
- Controlled supply over algorithmic issuance

---

## 18. Business Continuity

In the event of:

- Oracle failure
- Network disruption
- Governance compromise

Emergency actions require governance pathway.

No centralized emergency override exists outside governed execution.

Index calculation may pause if required to preserve integrity.

---

## 19. Dependency Disclosure

Primary dependencies include:

- Solidity compiler (publicly verifiable)
- OpenZeppelin contract libraries
- Gnosis Safe (multi-signature framework)
- BNB Smart Chain infrastructure

Dependency versions are available via verified contract metadata.

---

## 20. Audit Status

Contracts underwent internal production-grade review aligned with OpenZeppelin enterprise standards.

Independent third-party external audit is anticipated.

All upgrades will be subject to renewed review.

---

## 21. Risk Surface Overview

Primary technical risks include:

- Smart contract vulnerability
- Governance key compromise
- Oracle quorum manipulation
- Network-level risk (BSC)
- Upgrade misconfiguration

Mitigations include:

- Multi-signature Safe
- Timelock enforcement
- Quorum-based oracle model
- Public auditability

Residual risk remains.

---

## 22. Structural Classification

The architecture supports a:

- Fixed cap
- Governance-minted
- Non-redeemable
- Market-priced digital benchmark instrument

It is not:

- An ETF
- A custodial instrument
- A structured note
- A depositary receipt

---

End of Technical Architecture Document.
