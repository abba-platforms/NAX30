# NAX30 Index Methodology

By [Simon Kapenda](https://linkedin.com/in/simonkapenda)       
Version 1.0  
Effective Date: February 2026  

---

## 1. Index Objective

The Namibia 30 Index (NAX30) is designed to measure the performance of a rules-based basket of thirty (30) selected securities listed on the [Namibia Securities Exchange (NSX)](https://nsx.com.na)

The index serves as a composite benchmark reflecting trends in Namibia’s listed equity market.

---

## 2. Eligible Universe

Eligible securities must:

- Be listed on the Namibia Securities Exchange (NSX)
- Be in good regulatory standing
- Have continuous trading status
- Satisfy minimum liquidity considerations (as determined by the Index Committee)

Synthetic instruments, derivatives, or non-listed securities are not eligible.

---

## 3. Constituent Selection

The index maintains a fixed basket of 30 constituents.

Selection considerations include:

- Market capitalization
- Liquidity profile
- Sector representation
- Trading continuity

Constituent changes occur during scheduled quarterly reviews or extraordinary events.

---

## 4. Base Date and Base Value

Base Index Level: 10,000 basis points (bps)

The base value represents 100.00% normalized benchmark level.

---

## 5. Weighting Methodology

NAX30 is a modified weighted index.

Each constituent is assigned a weight (W_i).

Total weights normalize to 10,000 basis points.

Weight determination may consider:

- Relative market capitalization
- Liquidity factors
- Sector balancing constraints
- Concentration controls

Individual constituent weight caps may be applied to prevent excessive concentration.

---

## 6. Index Calculation Formula

The index level at time t is calculated as:

NAX30_t = 10,000 × ( Σ (W_i × P_i,t) ) / ( Σ (W_i × P_i,0) )

Where:

W_i = Assigned weight of constituent i  
P_i,t = Current price of constituent i  
P_i,0 = Price at base date  

Prices are sourced via designated oracle inputs referencing official NSX disclosures and validated market data.

---

## 7. Corporate Action Adjustments

The index adjusts for:

- Stock splits
- Reverse splits
- Bonus issues
- Rights issues
- Mergers and acquisitions
- Delistings

Adjustments are implemented to preserve index continuity.

Corporate actions may result in:

- Weight recalibration
- Constituent replacement
- Base divisor adjustment (if required)

---

## 8. Rebalancing Policy

Rebalancing occurs quarterly.

Quarterly review may include:

- Weight adjustments
- Constituent inclusion/removal
- Corporate action normalization

Extraordinary rebalancing may occur in cases of:

- Delisting
- Regulatory suspension
- Corporate restructuring

---

## 9. Market Disruption Policy

If trading is halted on the NSX:

- The most recent valid traded prices may be used.
- Index calculation may be temporarily suspended.

If a constituent is suspended:

- Temporary freeze may apply.
- Replacement may occur at next review.

---

## 10. Data Sources

Primary Data Source:

- Official Namibia Securities Exchange disclosures

Secondary Sources:

- Validated market reporting systems

If discrepancies arise, official exchange data prevails.

---

## 11. Publication & Transparency

Methodology updates:

- Must be approved through formal governance procedures.
- Are version-controlled.
- Are publicly archived.

Annual methodology review may be conducted.

---

## 12. Divisor & Continuity Mechanism

To maintain index continuity across corporate actions and constituent changes, a divisor adjustment mechanism may be applied.

The divisor ensures that non-market-driven structural changes do not artificially impact index level.

Divisor adjustments may occur in cases including but not limited to:

- Stock splits
- Mergers
- Constituent replacements
- Extraordinary distributions

All divisor modifications are documented and version-controlled.

---

## 13. Weight Cap Policy

To mitigate excessive concentration risk:

- Individual constituent weights may be capped.
- Sector-level balancing constraints may be applied.
- Excess weight above cap may be redistributed proportionally across remaining constituents.

Specific caps, if applied, are determined during rebalancing and documented in governance records.

---

## 14. Liquidity Screening Criteria

At each quarterly review, liquidity considerations may include:

- Average daily trading volume
- Trading frequency
- Bid-ask spread conditions
- Free-float considerations (if applicable)

Securities failing minimum liquidity thresholds may be reviewed for removal.

---

## 15. Free Float Considerations

If implemented, free float adjustments may be applied to reflect publicly tradable shares rather than total issued shares.

Free float adjustments, if adopted, will be documented and version-controlled.

---

## 16. Extraordinary Event Handling

In the event of:

- Exchange closure
- Prolonged suspension
- Corporate insolvency
- Regulatory delisting

The Index Committee may initiate extraordinary review procedures outside the normal quarterly cycle.

All extraordinary decisions require formal governance approval.

---

## 17. Calculation Frequency

Index level calculation frequency may be:

- Periodic (e.g., hourly, daily), or
- Event-triggered via oracle update

Calculation frequency does not guarantee continuous real-time updates and may be subject to oracle quorum confirmation.

---

## 18. Rounding Policy

For consistency:

- Constituent weights may be rounded to defined precision levels.
- Index values may be rounded to a specified number of decimal places for publication.

Rounding policy does not materially alter benchmark structure.

---

## 19. Backtesting & Historical Simulation

Historical backtesting, if performed:

- Is for illustrative purposes only.
- Does not guarantee future performance.
- May rely on reconstructed historical pricing data.

Backtested data, if published, will be clearly labeled as simulated.

---

## 20. Conflict of Interest Disclosure

Governance participants, oracle operators, or affiliated entities may hold positions in:

- NAX30 tokens
- Underlying constituents

Operational controls are designed to mitigate manipulation risk through:

- Multi-signature governance
- Timelock delays
- On-chain transparency

---

## 21. Index Committee Governance Disclosure

The Index Oversight Committee:

- Operates under defined procedural rules.
- Documents meeting decisions.
- Maintains version-controlled change logs.

Committee authority is administrative and does not override on-chain governance controls.

---

End of Methodology.
