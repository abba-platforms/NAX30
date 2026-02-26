# NAX30 Audit Status  
Namibia 30 Index (NAX30)

Version 2.0 – Smart Contract & Governance Audit Disclosure  
Effective Date: February 2026  

---

## 1. Purpose

This document provides a transparent disclosure of the audit status of the Namibia 30 Index (NAX30) smart contract system and governance architecture.

The objective is to:

- Disclose current audit posture  
- Clarify scope of review  
- Identify limitations  
- Outline external audit intentions  
- Maintain transparency with market participants  

This disclosure does not constitute a representation that the system is free from defects.

---

## 2. Smart Contract Architecture Overview

NAX30 is deployed on BNB Smart Chain and consists of:

- Upgradeable proxy contract (primary token address)  
- Implementation contract  
- Registry contract (weights & constituent data)  
- TimelockController  
- Multi-Signature Safe governance  

The architecture utilizes an upgradeable proxy model. Contract logic is not immutable and may be modified through formal governance procedures.

All contracts are publicly verifiable on-chain.

---

## 3. Deployed Contract Addresses (BSC Mainnet)

Deployer:  
0xe844443EBfc36e99C1868584F9cDB52385Ac89c6  

Timelock Controller:  
0xdc38cab671EECbd13D5c8771DC44C5729C2B4267  

Registry Contract:  
0x960cc4EB352c6B920a05Dc3A97BED768E551c4f8  

Multi-Signature Safe:  
0x397314A5CAA3F891A2d85DAc109be2078b510155  

NAX30 Proxy (Primary Token Address):  
0xaAd81eb1f27874B8B0CB03C778C6019ea32045Ff  

Implementation Contract:  
0x8293C888fFa3601E4197e63f2924E10cA32E5d88  

Verified timelock():  
0xdc38cab671EECbd13D5c8771DC44C5729C2B4267  

Verified registry():  
0x960cc4EB352c6B920a05Dc3A97BED768E551c4f8  

---

## 4. Internal Review & Security Controls

Prior to deployment, contracts underwent:

- Internal code review aligned with OpenZeppelin production-grade standards  
- Access control validation  
- Governance permission verification  
- Timelock execution pathway testing  
- Proxy upgrade safety checks  
- Registry integrity validation  
- Oracle quorum verification logic testing  

Internal review focused on:

- Access control restrictions  
- Upgradeability safety  
- Governance execution correctness  
- Deterministic calculation logic  
- Overflow/underflow protection (Solidity ^0.8.x)  

Internal review does not constitute an independent third-party external audit.

---

## 5. External Audit Status

As of the Effective Date:

- No completed third-party external audit report has been published.  
- The contracts are subject to future independent audit review.  

If engaged, an external audit may include:

- Static code analysis  
- Upgradeability review  
- Governance pathway validation  
- Oracle submission logic review  
- Registry manipulation risk analysis  
- Access control verification  
- Economic attack surface review  

Any completed external audit may be published at the Administrator’s discretion.

---

## 6. Economic & Technical Risk Disclosure

Smart contract and governance architecture may be exposed to:

- Oracle collusion risk (despite 2-of-3 quorum safeguards)  
- Governance key coordination risk  
- Smart contract logic vulnerabilities  
- Upgrade implementation risk  
- Blockchain reorganization events  
- Flash-loan related market distortions (if secondary data sources are used)  
- Infrastructure dependency failures  

Mitigation mechanisms reduce but do not eliminate such risks.

---

## 7. Governance Key Management

Governance operates under Multi-Signature Safe control.

Security posture includes:

- Threshold-based execution  
- Signer distribution  
- Timelock delay enforcement  

The Administrator may implement hardware-based key custody and operational key management practices; however, key compromise risk cannot be eliminated.

---

## 8. Upgrade Governance Safeguards

Any contract upgrade requires:

1. Governance proposal  
2. Multi-Signature Safe approval  
3. Timelock scheduling  
4. On-chain execution  

There is no unilateral administrator override.

Upgrade events are publicly observable.

---

## 9. Ongoing Monitoring

Security posture includes:

- Continuous monitoring of governance transactions  
- Review of oracle submission behavior  
- Public contract verification  
- Repository transparency  

Security reviews may be conducted periodically.

---

## 10. Responsible Disclosure

If a vulnerability is identified:

- Issue may be reported to the Administrator  
- Governance review is initiated  
- Patch or upgrade may be scheduled via timelock  

Public disclosure timing may consider security impact.

A formal bug bounty program may be implemented in the future; none is active as of the Effective Date.

---

## 11. Audit History Log

As of Version 2.0:

- Internal review completed prior to deployment  
- No external audit completed  
- No published third-party audit report  

Future updates to audit posture will be documented in this file.

---

## 12. Scope Limitations

Audit review — whether internal or external — cannot guarantee:

- Absence of vulnerabilities  
- Immunity from unforeseen attack vectors  
- Protection against blockchain-level risk  
- Protection against oracle manipulation beyond quorum safeguards  

Smart contracts inherently carry technological risk.

---

## 13. Public Transparency

The following are publicly available:

- Proxy contract address  
- Implementation contract address  
- Registry contract address  
- Timelock address  
- Governance Safe address  
- Source code repository  

Transparency does not eliminate technical risk.

---

## 14. Limitation of Reliance

Participants must not rely solely on this Audit Status disclosure when assessing risk.

Independent review, legal consultation, and technical analysis are recommended.

---

## 15. Risk Statement

Participants should assume:

- Smart contract risk exists  
- Upgrade risk exists  
- Oracle dependency risk exists  
- Governance key management risk exists  
- Blockchain systemic risk exists  

No representation is made that the contracts are free from defects.

---

## 16. Regulatory Positioning

Audit status disclosure does not:

- Imply regulatory approval  
- Imply government endorsement  
- Guarantee compliance classification  

Regulatory interpretation may vary by jurisdiction.

---

End of Audit Status Disclosure.
