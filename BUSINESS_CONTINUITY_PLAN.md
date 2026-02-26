# NAX30 Business Continuity Plan  
Namibia 30 Index (NAX30)

Version 2.0 – Tier-1 Institutional Operational Resilience Framework  
Effective Date: February 2026  

---

## 1. Purpose

This Business Continuity Plan (BCP) outlines the framework designed to maintain operational resilience of the Namibia 30 Index (NAX30) in the event of disruption.

The objective of this Plan is to:

- Preserve benchmark integrity  
- Maintain calculation continuity where possible  
- Ensure governance functionality  
- Protect data integrity  
- Mitigate operational interruption risk  

This Plan applies to administrative, governance, oracle, smart contract, and data infrastructure components of the NAX30 framework.

---

## 2. Scope of Coverage

This Plan addresses continuity risks across:

- Benchmark Administration  
- Governance (Multi-Signature Safe + TimelockController)  
- Oracle Infrastructure  
- Smart Contract Infrastructure  
- Data Sourcing  
- Public Blockchain Network Dependency  
- Third-Party Infrastructure Dependencies  

---

## 3. Operational Dependency Map

NAX30 operational continuity depends on:

1. Official NSX data availability  
2. Oracle operator participation (2-of-3 quorum)  
3. Governance signer coordination  
4. BNB Smart Chain network availability  
5. Administrative oversight  
6. Infrastructure providers (node access, RPC endpoints, hosting environments)  

Failure in one component does not automatically result in benchmark failure due to structural redundancy.

---

## 4. Recovery Objectives

### 4.1 Recovery Time Objective (RTO)

Target Recovery Time Objective (RTO):  
Operational recovery efforts are initiated immediately upon detection of disruption. While no guaranteed recovery time can be assured due to blockchain and exchange dependencies, the Administrator targets restoration of benchmark functionality within commercially reasonable timeframes.

### 4.2 Recovery Point Objective (RPO)

Target Recovery Point Objective (RPO):  
On-chain data persistence ensures zero historical data loss under normal blockchain operation. Off-chain administrative records are retained in accordance with internal record retention policy (minimum five-year retention).

---

## 5. Incident Classification Framework

Disruptions are categorized as follows:

- **Level 1 – Minor Disruption:**  
  Temporary delay in oracle submission or administrative coordination. No benchmark integrity impact.

- **Level 2 – Material Disruption:**  
  Oracle quorum interruption, exchange trading halt, or calculation delay impacting timely publication.

- **Level 3 – Critical Integrity Event:**  
  Smart contract vulnerability, governance compromise, systemic exchange failure, or data corruption affecting benchmark validity.

Escalation procedures scale according to classification level.

---

## 6. Governance Continuity

### 6.1 Multi-Signature Redundancy

Governance operates under threshold-based authorization.

Continuity safeguards include:

- Multiple independent signers  
- Geographic distribution of signers where feasible  
- No reliance on a single individual  
- On-chain execution transparency  

Loss of one signer does not disable governance provided quorum remains intact.

---

### 6.2 Signer Compromise Procedure

If a signer key is:

- Lost  
- Compromised  
- Inaccessible  

Governance may:

1. Remove the affected signer  
2. Replace with a new signer  
3. Execute replacement via timelock  

All changes are publicly auditable.

---

## 7. Oracle Continuity

### 7.1 Quorum Protection

The oracle system operates under a 2-of-3 quorum model.

If one oracle fails:

- Remaining two may continue submissions  

If quorum is not met:

- Index update may pause  
- Last valid index level may remain published  

---

### 7.2 Oracle Replacement

If an oracle operator becomes unavailable:

- Governance may propose replacement  
- Replacement requires Safe approval and timelock scheduling  
- Change is publicly verifiable  

Oracle operators are expected to maintain operational independence and infrastructure redundancy.

---

## 8. Data Source Disruption

If official NSX data becomes temporarily unavailable:

- The most recent validated traded price may be used  
- Index calculation may pause  
- Governance review may be initiated  

If prolonged disruption occurs:

- Governance may evaluate alternative sourcing  
- Any change must follow formal governance process  
- Public documentation must be updated  

---

## 9. Smart Contract Resilience

NAX30 smart contracts:

- Are deployed on BNB Smart Chain  
- Utilize upgradeable proxy architecture  
- Are publicly verifiable  

If a vulnerability is identified:

- Governance review is initiated  
- Upgrade proposal may be scheduled  
- Timelock delay is enforced  
- Upgrade execution is publicly recorded  

No emergency bypass exists outside defined governance mechanisms.

---

## 10. Blockchain Network Disruption

If BNB Smart Chain experiences:

- Network outage  
- Congestion  
- Validator instability  
- Reorganization events  

Index updates may be delayed.

Smart contract state remains persistent once network stabilizes.

Governance may delay structural changes during network instability.

The Administrator does not control blockchain validator operations.

---

## 11. Administrative Continuity

The Benchmark Administrator maintains:

- Repository documentation backups  
- Governance access control protocols  
- Internal coordination procedures  
- Administrative record retention safeguards  

Corporate-level disruption does not automatically invalidate on-chain benchmark logic.

---

## 12. Cybersecurity Safeguards

Operational resilience includes:

- Secure key management practices  
- Multi-device signer distribution  
- Segregation of oracle infrastructure  
- Restricted administrative access  
- Periodic access review  

Absolute security cannot be guaranteed.

---

## 13. Communication Protocol During Disruption

In the event of material or critical disruption:

- Notice may be published via official repository or website  
- Governance execution events remain publicly visible on-chain  
- Structural changes remain subject to timelock transparency  

The Administrator does not guarantee real-time incident disclosure in all circumstances.

---

## 14. Emergency Suspension

In extraordinary circumstances including:

- Exchange closure  
- Oracle failure  
- Smart contract vulnerability  
- Governance capture risk  
- Systemic data corruption  

Governance may:

- Temporarily suspend index updates  
- Maintain last validated index level  
- Initiate remediation process  

All actions require formal governance execution.

---

## 15. Cessation Scenario

If continuity cannot be restored due to:

- Regulatory prohibition  
- Irrecoverable infrastructure failure  
- Governance dissolution  
- Force majeure event  

Cessation may be proposed.

Cessation requires:

1. Governance proposal  
2. Safe approval  
3. Timelock scheduling  
4. Public execution  

Historical index data remains on-chain.

---

## 16. Force Majeure

The Administrator shall not be liable for disruptions caused by:

- Natural disasters  
- War or civil unrest  
- Government intervention  
- Exchange closure  
- Telecommunications failure  
- Widespread cyberattack  
- Systemic blockchain failure  

Force majeure events may impact calculation continuity.

---

## 17. Third-Party Dependency Disclosure

NAX30 relies on:

- Namibia Securities Exchange data  
- BNB Smart Chain network  
- Oracle operators  
- Node and infrastructure providers  

The Administrator does not control third-party infrastructure and cannot guarantee uninterrupted service from external dependencies.

---

## 18. Operational Succession Planning

If the Administrator is unable to continue operations:

- Governance may designate successor administrative authority  
- Documentation and smart contract control remain on-chain  
- Succession must follow governance procedure  

No automatic transfer occurs outside governance authorization.

---

## 19. Testing & Review

This Business Continuity Plan may be reviewed annually.

Governance may:

- Test recovery procedures  
- Evaluate oracle redundancy  
- Review signer distribution  
- Assess operational resilience effectiveness  

Amendments require formal governance process.

---

## 20. Limitations

This Plan does not eliminate:

- Market risk  
- Regulatory risk  
- Blockchain systemic risk  
- Force majeure events  
- Liquidity disruption  

It provides structural mitigation, not risk elimination.

---

## 21. No Guarantee of Continuous Calculation

The Administrator does not guarantee:

- Continuous index calculation  
- Uninterrupted availability  
- Real-time update frequency  
- Market price stability  

The benchmark may experience delay, suspension, or cessation in extreme conditions.

---

## 22. Disclaimer

This Business Continuity Plan describes operational resilience mechanisms for the NAX30 benchmark framework.

It does not:

- Guarantee uninterrupted availability  
- Guarantee price stability  
- Create fiduciary obligations  
- Eliminate systemic risks  

Regulatory interpretation may vary by jurisdiction.

---

End of Business Continuity Plan.
