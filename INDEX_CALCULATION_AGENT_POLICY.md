# NAX30 Index Calculation Agent Policy  
Namibia 30 Index (NAX30)

Version 2.0 – Tier-1 Institutional Benchmark Calculation Framework  
Effective Date: February 2026  

---

## 1. Purpose

This Index Calculation Agent Policy defines the responsibilities, controls, procedures, and limitations applicable to the calculation of the Namibia 30 Index (NAX30).

The objective is to ensure:

- Transparent and rules-based calculation  
- Consistency with published methodology  
- Data integrity safeguards  
- Controlled governance oversight  
- Clear separation between calculation and commercial considerations  

---

## 2. Designation of Calculation Agent

The Calculation Agent function is administered under the authority of the Benchmark Administrator.

Calculation execution occurs through:

1. Deterministic on-chain smart contract logic  
2. Oracle-based price input submissions  
3. Governance-controlled registry architecture  

The Calculation Agent role may be performed internally by the Benchmark Administrator or delegated to an authorized entity, provided:

- Delegation is documented  
- Governance oversight remains intact  
- Methodology integrity is preserved  

Replacement of the Calculation Agent requires formal governance procedure.

---

## 3. Calculation Responsibility

The NAX30 benchmark is calculated through a hybrid structure:

1. On-chain smart contract logic  
2. Oracle-based price input submissions  
3. Governance-controlled registry architecture  

The benchmark calculation is deterministic and formula-based.

There is no discretionary manual override of index levels outside formal governance procedures.

Preservation of benchmark integrity supersedes calculation continuity.

---

## 4. Calculation Formula

The index level at time t is calculated as:

NAX30_t = 10,000 × ( Σ (W_i × P_i,t) ) / ( Σ (W_i × P_i,0) )

Where:

W_i = Assigned weight of constituent i  
P_i,t = Current validated price  
P_i,0 = Price at base date  

Weights are stored in the on-chain Registry contract.

The base level is 10,000 basis points (bps).

No discretionary adjustments to formula components are permitted outside formal methodology amendment process.

---

## 5. Valuation Time Reference

Where applicable, constituent pricing references:

- Official Namibia Securities Exchange (NSX) closing prices  
- Published exchange data  

Time reference:

- Namibia Standard Time (UTC+2), unless otherwise specified  

If official closing prices are unavailable, fallback hierarchy applies as defined in the Data Provider Disclosure.

---

## 6. Data Inputs

Price data inputs are sourced through the Oracle framework.

Data hierarchy:

1. Official Namibia Securities Exchange (NSX) disclosures  
2. Validated secondary market feeds  
3. Last traded price fallback  

The calculation agent relies on oracle quorum validation (2-of-3) for price update acceptance.

---

## 7. Oracle Submission Timing & Cut-Off

Oracle submissions must:

- Reflect the most recently validated official data  
- Meet quorum threshold  
- Pass deviation tolerance checks  

Late or stale submissions may be rejected automatically by contract logic or governance rule.

If valid quorum is not achieved within reasonable operational window:

- Index update may pause  
- Last validated level may remain effective  

---

## 8. Divisor & Base Adjustment Governance

The index is normalized to a base value of 10,000 bps.

If divisor adjustments are required due to:

- Corporate actions  
- Structural methodology change  

Such adjustments must:

1. Be approved by the Index Committee  
2. Be executed via governance  
3. Be publicly documented  

No discretionary divisor alteration is permitted outside governance process.

---

## 9. Role of Oracle Operators

Oracle operators:

- Submit constituent price data  
- Operate independently  
- Must meet quorum requirements  
- Cannot unilaterally update index levels  

Oracle configuration changes require governance execution.

---

## 10. Calculation Frequency

Index level updates occur when:

- Valid oracle submissions meet quorum  
- Smart contract state update executes successfully  

The calculation agent does not guarantee real-time or continuous updates.

Update frequency depends on data availability and oracle participation.

---

## 11. Corporate Action Handling

Corporate actions are reflected through:

- Registry updates  
- Weight recalibration  
- Constituent replacement (if required)  

Adjustments require:

1. Index Committee review  
2. Governance approval  
3. Timelock scheduling  
4. On-chain execution  

No discretionary ad hoc adjustments are permitted.

---

## 12. Error Handling & Materiality Threshold

If an error is detected:

- Governance review is initiated  
- Root cause is evaluated  
- Corrective action may be scheduled  

A material error may include:

- Incorrect weight application  
- Incorrect price input exceeding defined deviation tolerance  
- Calculation error resulting in materially misleading benchmark level  

Materiality determination is assessed by governance in consultation with the Index Committee.

Corrective changes must:

- Follow governance process  
- Be publicly auditable  
- Not retroactively alter immutable blockchain history  

Material errors may be disclosed publicly.

---

## 13. Market Disruption Handling

In cases of:

- Exchange trading halt  
- Data feed disruption  
- Oracle quorum failure  

The calculation agent may:

- Pause index updates  
- Maintain last validated level  
- Await quorum restoration  

If benchmark integrity cannot be maintained, governance may suspend calculation temporarily.

No synthetic price estimation is permitted without governance authorization.

---

## 14. Calculation Integrity Safeguards

The calculation framework includes:

- Deterministic formula logic  
- Weight normalization constraints  
- Governance-controlled registry updates  
- Public on-chain verification  

Calculation logic cannot be altered without formal upgrade procedure.

---

## 15. Upgrade & Modification Controls

Any modification to calculation logic requires:

1. Governance proposal  
2. Multi-Signature Safe approval  
3. Timelock scheduling  
4. On-chain execution  

No emergency bypass mechanism exists outside coded governance.

---

## 16. Separation from Commercial Functions

The Calculation Agent operates independently from:

- Token issuance decisions  
- Market-making activities  
- Exchange listing negotiations  
- OTC allocation operations  

Index calculation decisions must not consider token market price performance.

---

## 17. Third-Party Dependencies

Calculation relies on:

- NSX data availability  
- Oracle operator functionality  
- BNB Smart Chain network availability  
- Node infrastructure providers  

The Calculation Agent does not control third-party systems.

---

## 18. Escalation Framework

If integrity concerns arise:

- Issue is escalated to Index Committee  
- Governance Safe is notified  
- Formal review initiated  
- Execution subject to timelock  

All escalation outcomes must be documented.

---

## 19. Record Retention

Calculation-related documentation:

- Is version-controlled  
- Is archived in public repository  
- Maintains historical traceability  

On-chain records provide immutable audit trail.

Administrative documentation retained for minimum five (5) years.

---

## 20. External Review & Audit

Calculation logic and smart contracts:

- May undergo internal audit review  
- May be subject to independent third-party external audit  

Audit findings, if material, may result in governance action.

---

## 21. Official Publication Source

The official source of record for NAX30 is:

- On-chain smart contract state  

Off-chain publications (website, repository, exchange displays) are indicative unless otherwise stated.

---

## 22. Limitations

The Calculation Agent does not guarantee:

- Continuous calculation  
- Real-time publication  
- Convergence of token market price to theoretical index value  
- Immunity from systemic market disruption  

Benchmark levels may diverge from theoretical models due to liquidity or market conditions.

---

## 23. Regulatory Positioning

NAX30 calculation is rules-based and transparent.

The Calculation Agent does not:

- Provide investment advice  
- Guarantee performance  
- Manage assets  
- Operate as a collective investment scheme  

Regulatory classification may vary by jurisdiction.

---

## 24. Review of Policy

This Policy may be reviewed annually.

Amendments require:

1. Index Committee approval  
2. Governance execution  
3. Public documentation update  

---

End of Index Calculation Agent Policy.
