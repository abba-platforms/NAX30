# NAX30 Data Provider Disclosure  
Namibia 30 Index (NAX30)

Version 2.0 – Tier-1 Institutional Benchmark Administrator Standard  
Effective Date: February 2026  

---

## 1. Purpose

This Data Provider Disclosure outlines the sources, validation framework, governance controls, operational oversight, and limitations associated with data used in the calculation of the Namibia 30 Index (NAX30).

This document provides transparency regarding data sourcing, verification procedures, integrity controls, and dependency risks inherent in a blockchain-native benchmark framework.

---

## 2. Primary Data Source

The primary data source for NAX30 constituent pricing is:

- Official disclosures and published price information from the Namibia Securities Exchange (NSX).

Official exchange data is considered authoritative for purposes of benchmark calculation.

Where applicable, pricing data may be sourced directly from publicly available NSX publications or through validated market data distribution channels that reflect official exchange disclosures.

The Benchmark Administrator does not independently audit exchange data.

---

## 3. Secondary & Validated Sources

Where necessary, secondary sources may include:

- Validated market reporting systems  
- Licensed financial data vendors  
- Publicly accessible exchange reporting mechanisms  

Secondary sources are used solely for validation or redundancy purposes.

In the event of discrepancy, official NSX disclosures prevail.

---

## 4. Data Sufficiency & Representativeness

The NAX30 index relies on publicly available market data from a regulated exchange environment.

However:

- Trading frequency on certain securities may be limited  
- Liquidity conditions may vary  
- Market depth may be constrained  

Where data is deemed insufficient to maintain benchmark integrity, governance procedures may be initiated in accordance with the Index Methodology and Governance Charter.

---

## 5. Oracle Submission Framework

NAX30 utilizes a quorum-based oracle framework to transmit pricing data on-chain.

The framework operates under a 2-of-3 quorum confirmation requirement.

Key characteristics:

- Multiple independent oracle operators  
- Median-based aggregation logic  
- Timestamp validation  
- Tolerance thresholds for anomaly detection  

No single oracle operator can independently determine index level updates.

---

## 6. Oracle Operator Oversight

Oracle operators are subject to governance oversight.

Governance may:

- Approve new oracle operators  
- Remove oracle operators  
- Modify quorum parameters (subject to governance procedure)  

Oracle operators must:

- Operate independently  
- Submit publicly sourced pricing data  
- Avoid submission of non-public information  

Changes to oracle configuration require formal governance scheduling and execution.

---

## 7. Data Validation Controls

The following validation controls are applied:

- Timestamp recency checks  
- Cross-source price comparison  
- Quorum confirmation requirement  
- Deviation tolerance thresholds  
- Rejection of materially inconsistent submissions  

Invalid submissions are not included in index calculation.

The calculation process is deterministic and rule-based.

There is no discretionary human override of index levels.

---

## 8. Data Hierarchy

In the event of data inconsistencies, the following hierarchy applies:

1. Official NSX published data  
2. Verified secondary market reporting systems  
3. Most recent validated traded price  

If authoritative data cannot be confirmed, index calculation may be paused in accordance with the Market Disruption Policy.

---

## 9. Corporate Action Data

Corporate action data (including stock splits, reverse splits, rights issues, mergers, and delistings) is sourced from:

- Official NSX announcements  
- Issuer regulatory disclosures  

Adjustments are implemented in accordance with the published Index Methodology.

---

## 10. Data Dependency Risk

NAX30 calculation depends on:

- Accuracy of official exchange disclosures  
- Availability of timely price updates  
- Reliability of oracle infrastructure  

Errors, delays, or inconsistencies in source data may affect calculated index levels.

The Benchmark Administrator does not independently audit exchange data.

---

## 11. Data Error Correction Policy

If a material data error is identified:

- The error will be reviewed  
- Governance review may be initiated  
- Correction may be implemented through formal governance procedure  

Retroactive index restatement is not guaranteed and will be considered only where materially necessary.

All corrections must be:

- Version-controlled  
- Publicly documented  
- Executed via governance framework  

---

## 12. Data Retention Policy

Oracle submissions and governance execution records are recorded on-chain.

Supplementary administrative records related to:

- Conflict disclosures  
- Data anomaly review  
- Governance scheduling  

May be retained for a minimum of five (5) years.

Historical index levels remain publicly verifiable via blockchain records.

---

## 13. Material Data Source Change Policy

If the primary data source changes or becomes unavailable:

- Governance review will be initiated  
- Alternative data sourcing framework may be proposed  
- Public documentation will be updated  
- Changes will be scheduled and executed via formal governance procedure  

No unilateral data source substitution is permitted.

---

## 14. Data Publication Transparency

Smart contract addresses, oracle configuration, governance execution records, and methodology documentation are publicly verifiable.

This enables independent verification of:

- Weight normalization  
- Index formula execution  
- Oracle confirmation logic  
- Governance scheduling  

---

## 15. Confidentiality & Equal Access Principle

Only publicly disclosed pricing information is incorporated into index calculations.

The Benchmark Administrator does not:

- Utilize non-public information  
- Provide selective data access  
- Grant preferential timing of structural changes  

All structural changes are subject to timelock delay and public on-chain scheduling.

---

## 16. Data Integrity Escalation

If a systemic data failure occurs, including:

- Prolonged exchange outage  
- Oracle quorum failure  
- Data corruption  

Governance may:

- Temporarily suspend index calculation  
- Maintain last validated index level  
- Initiate review procedure  

Such actions must follow formal governance process.

---

## 17. Third-Party Data Usage Disclaimer

NAX30 relies on third-party data sources.

The Benchmark Administrator does not:

- Guarantee completeness of exchange disclosures  
- Warrant uninterrupted availability of data feeds  
- Assume liability for external reporting inaccuracies  

Data providers are not responsible for NAX30 token pricing or market performance.

---

## 18. Regulatory Positioning

This Disclosure supports alignment with high-level international benchmark governance standards, including IOSCO Principles for Financial Benchmarks relating to data integrity, transparency, and oversight.

Regulatory interpretation may vary by jurisdiction.

---

## 19. Amendments

This Data Provider Disclosure may be amended only through:

1. Governance proposal  
2. Multi-signature approval  
3. Timelock scheduling  
4. On-chain execution  

All amendments must be version-controlled and archived.

---

End of Data Provider Disclosure.
