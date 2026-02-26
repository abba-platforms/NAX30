# NAX30 Oracle Policy

Version 2.0 – Institutional Governance Standard  
Effective Date: February 2026  
By [Simon Kapenda](https://linkedin.com/in/simonkapenda)

---

## 1. Purpose

This Oracle Policy defines the governance, operational, and data integrity framework supporting index level calculations for the Namibia 30 Index (NAX30).

The oracle system is responsible for submitting validated constituent price data used in the calculation of index levels as defined in the [NAX30 Index Methodology](https://github.com/abba-platforms/NAX30/blob/main/INDEX_METHODOLOGY.md).

This policy establishes:

- Data integrity standards  
- Quorum and aggregation rules  
- Governance-controlled change management  
- Failure handling procedures  
- Transparency and auditability requirements  

---

## 2. Oracle Architecture

NAX30 operates under a designated oracle operator framework consisting of:

- Three (3) approved oracle addresses  
- On-chain registry-controlled configuration  
- Governance-controlled modification authority  

Oracle addresses are recorded in the registry contract and may only be modified through:

1. Multi-Signature Safe proposal approval  
2. TimelockController scheduling  
3. Delayed on-chain execution  

No unilateral authority exists to modify oracle configuration.

---

## 3. Quorum Requirement

The NAX30 oracle system operates under a **2-of-3 quorum model**.

A valid index update requires:

- At least two (2) oracle submissions  
- Submissions that fall within defined tolerance parameters  

No single oracle may independently update index data.

If only one oracle submits data, no update is processed.

---

## 4. Aggregation Logic

When quorum is achieved:

- If two submissions match within tolerance, the index update is accepted.
- If three submissions are provided, the **median value** is used for final calculation.

If one submission materially deviates beyond tolerance thresholds:

- The outlier submission is excluded.
- The remaining concordant submissions determine validity.

Aggregation logic is deterministic and executed on-chain.

---

## 5. Tolerance Parameters

To mitigate erroneous or malicious submissions, oracle updates must fall within an acceptable deviation band.

Tolerance is defined as:

- A maximum percentage deviation relative to peer submissions.
- The tolerance threshold is governance-configurable.

If deviation exceeds threshold:

- Submission is rejected.
- Governance review may be triggered if repeated.

Tolerance parameters are version-controlled and require governance scheduling to modify.

---

## 6. Timestamp & Data Freshness Policy

Each oracle submission must include a timestamp.

Data freshness requirements:

- Submissions must reflect current trading session data.
- Stale submissions beyond a defined maximum age may be rejected.
- Timestamp validation ensures chronological consistency.

Maximum data age thresholds may be modified only through governance procedures.

---

## 7. Data Hierarchy

Oracle operators must reference data sources in the following priority order:

1. Official Namibia Securities Exchange (NSX) disclosures  
2. Validated secondary reporting systems  
3. Last traded price fallback (if primary sources unavailable)  

In the event of discrepancy:

- Official exchange data prevails.
- Governance review may be initiated if persistent conflict exists.

---

## 8. Update Frequency

Oracle update cadence may be:

- Periodic (e.g., daily or scheduled interval)  
- Event-triggered based on defined market conditions  

The oracle framework does not guarantee continuous real-time updates.

Update frequency may be adjusted through governance scheduling.

---

## 9. Failure Handling & Liveness

If quorum cannot be achieved:

- Index level update is paused.
- The last validated index level remains published.

If one oracle becomes inactive:

- The remaining two operators may continue functioning provided quorum is satisfied.

If two or more operators fail:

- Index updates halt.
- Governance intervention is required.

---

## 10. Oracle Operator Standards

Oracle operators are expected to maintain:

- Secure key custody (hardware-secured where possible)  
- Network-level access controls  
- Monitoring and logging infrastructure  
- Operational uptime consistency  

Operators must avoid conflicts of interest that may compromise data integrity.

---

## 11. Oracle Removal & Replacement

Oracle operators may be removed if:

- Repeated submission deviations occur  
- Persistent downtime is observed  
- Security breach is confirmed  
- Governance determines operational risk  

Removal requires:

1. Safe multi-signature approval  
2. Timelock scheduling  
3. On-chain execution  

Replacement follows identical governance procedure.

---

## 12. Emergency Governance Override

In extreme circumstances, including:

- Exchange closure  
- Coordinated oracle failure  
- Systemic data corruption  

Governance may initiate emergency review procedures.

Emergency actions may include:

- Temporary suspension of updates  
- Registry parameter adjustment  
- Oracle operator replacement  

All emergency actions require governance approval and timelock execution unless explicitly defined otherwise in contract architecture.

---

## 13. Transparency & On-Chain Verification

Oracle addresses are publicly verifiable.

All valid submissions:

- Emit on-chain events  
- Are permanently recorded  
- Are auditable via blockchain explorers  

Governance changes to oracle configuration are traceable and timestamped.

---

## 14. Risk Disclosure

Oracle infrastructure mitigates but does not eliminate:

- Data source dependency risk  
- Coordinated manipulation attempts  
- Infrastructure outages  
- Market volatility  

Index accuracy depends on integrity of external data inputs.

---

## 15. Regulatory Positioning

The oracle mechanism supports index calculation infrastructure only.

It does not:

- Guarantee index value accuracy under all conditions  
- Provide investment advice  
- Represent price verification of underlying securities  

The oracle system is a governance-controlled infrastructure component of the NAX30 benchmark framework.

---

End of Oracle Policy.
