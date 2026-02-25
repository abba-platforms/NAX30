# Namibia 30 Index (NAX30) — The Whitepaper 

## A Blockchain-Native Digital Benchmark for Namibia’s Public Equity Market

Version 2.0 – Institutional Governance Edition     
Created by: [Simon Kapenda](https://linkedin.com/in/simonkapenda)

---

## 1. Executive Summary

The Namibia 30 Index (NAX30) is a blockchain-native digital benchmark instrument designed to reference a rules-based basket of thirty (30) selected securities listed on the Namibia Securities Exchange (NSX).

Modeled conceptually after leading global benchmarks such as the Dow Jones Industrial Average (DJIA), NAX30 is structured as a modified weighted index. Constituent weights are determined through a defined, rules-based methodology designed to prevent excessive concentration in any single component while preserving representative market exposure.

NAX30 is issued as a governance-controlled digital index token with a fixed maximum supply and on-chain registry architecture.

NAX30 does not confer ownership of underlying securities, does not represent equity or debt in listed companies, and does not constitute units in a collective investment scheme. The token represents digital benchmark exposure only.

Price discovery occurs through open market trading (e.g., NAX30/NADD). There is no redemption mechanism linking token price to underlying securities.

---

## 2. Economic Context & Benchmark Role

Globally, benchmark indices serve as consolidated signals of market direction and economic sentiment:

- Germany relies on the DAX Index.
- The United States monitors the Dow Jones Industrial Average (DJIA) and S&P 500.
- Japan tracks the Nikkei 225.
- The United Kingdom follows the FTSE 100.

Each major economy operates a benchmark index that functions as a directional reference for equity market performance.

NAX30 is structured to operate as a consolidated benchmark reference for Namibia’s equity market.

As a composite benchmark:

- Upward movement reflects broad-based strengthening performance across weighted constituents and improving aggregate market sentiment.
- Downward movement indicates weakening performance and reduced investor confidence within the underlying basket.

NAX30 may therefore serve as a directional indicator of trends within Namibia’s listed equity market and, by extension, Namibia’s broader economic conditions.

---

## 3. Index Universe & Constituents

### 3.1 Eligible Universe

The NAX30 index includes only securities listed on the Namibia Securities Exchange (NSX).

No synthetic derivatives, non-listed instruments, or off-universe securities are included outside NSX eligibility.

### 3.2 Current Constituent Basket

The 30 constituents comprising NAX30 represent an estimated combined market value of approximately N$500 billion (~US$32 billion) across mining, financial services, telecommunications, consumer, property, and energy sectors.

The current constituents are:

1. Paladin Energy Ltd  
2. Deep Yellow Ltd  
3. Bannerman Resources Ltd  
4. Elevate Uranium Ltd  
5. Forsys Metals Corp  
6. Capricorn Group Ltd  
7. FirstRand Namibia Ltd (FNB)  
8. SBN Holdings (Standard Bank Namibia)  
9. Nictus Holdings Ltd  
10. Letshego Holdings Namibia Ltd  
11. Investec Ltd  
12. Sanlam Ltd  
13. Old Mutual Ltd  
14. Nedbank Group Ltd  
15. Standard Bank Group Ltd  
16. Mobile Telecommunications Ltd  
17. Momentum Group Ltd  
18. PSG Financial Services Ltd  
19. Anglo American plc  
20. B2Gold Corp  
21. Oryx Properties Ltd  
22. Vukile Property Fund Ltd  
23. Truworths International Ltd  
24. Shoprite Holdings Ltd  
25. Paratus Namibia Holdings Ltd  
26. Namibia Breweries Ltd  
27. Oceana Group Ltd  
28. Celsius Resources Ltd  
29. Alpha Namibia Industries Renewable Energy Power Ltd  
30. Reconnaissance Energy Africa Ltd.

Constituents are subject to periodic review and governed updates under the index methodology framework.

---

## 4. Base Index Level & Calculation Framework

### 4.1 Base Index Level

NAX30 is initialized at a base reference level of 10,000 basis points (bps).

10,000 bps represents the normalized 100.00% benchmark starting point.

### 4.2 Calculation Formula

NAX30_t = 10,000 × ( Σ (W_i × P_i,t) ) / ( Σ (W_i × P_i,0) )

Where:

W_i = Assigned weight of constituent i  
P_i,t = Current price  
P_i,0 = Price at base date  

Weights normalize to 10,000 basis points and are stored in an on-chain registry contract.

---

## 5. Weighting & Rebalancing Policy

NAX30 operates as a rules-based, modified weighted index.

Weighting objectives:

- Prevent excessive concentration
- Preserve sector representation
- Reflect liquidity and capitalization considerations

### Rebalancing Frequency

Quarterly review may include:

- Weight adjustments
- Constituent inclusion/removal
- Corporate action normalization

All changes require:

1. Multi-signature governance approval  
2. Timelock scheduling  
3. On-chain execution  

All updates are versioned for audit traceability.

---

## 6. Corporate Action Adjustment Framework

Adjustments may be required for:

- Stock splits  
- Reverse splits  
- Bonus issues  
- Rights issues  
- Mergers  
- Delistings  

Adjustments are implemented through governed registry updates following timelock delay.

---

## 7. Oracle Framework

Price inputs are submitted via designated oracle operators.

The framework operates under a 2-of-5 quorum requirement.

Five oracle sources exist. A minimum of two concurring submissions is required for update validity.

Oracle configuration changes require timelock-governed updates.

---

## 8. Token Structure

### 8.1 Standard

- ERC-20 compliant  
- 18 decimals  
- BEP-20 deployed on BNB Smart Chain  
- Upgradeable proxy architecture  

### 8.2 Maximum Supply

Maximum Supply: 10,000,000,000 NAX30

No algorithmic inflation.  
No automatic emissions.  

Minting requires governance scheduling and timelock execution.

---

## 9. Deployment Architecture (BSC Mainnet)

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

## 10. Market Structure & Settlement

Intended benchmark trading pair:

NAX30 / NADD

There is:

- No redemption mechanism  
- No NAV guarantee  
- No custody of underlying equities  

Market price is determined solely through supply-demand interaction.

---

## 11. OTC Allocation Framework

Current OTC Terms:

- OTC Price: N$0.50 per NAX30  
- Minimum Allocation: N$50  
- Delivery: Upon cleared settlement and compliance verification  
- Allocation subject to availability  

OTC Portal:  
https://trade.nax30.io  

Future exchange listing remains subject to independent approval and market conditions.

---

## 12. Governance Architecture

Two-layer governance:

### Multi-Signature Safe

- Proposal authority  
- Threshold-controlled approvals  

### TimelockController

- Mandatory delay  
- Deterministic operation IDs  
- Public on-chain auditability  

---

## 13. Market Price vs Indicative Index Value

NAX30 token market price may trade at a premium or discount to theoretical index value.

There is no arbitrage enforcement mechanism.

Divergence may persist due to liquidity and market conditions.

---

## 14. Data Transparency & Market Disruption Policy

Data hierarchy:

1. Official NSX disclosures  
2. Secondary validated feeds  
3. Last traded price fallback  

If trading halts occur:

- Index may pause  
- Last validated level may remain published  

Emergency actions follow governance procedures.

---

## 15. Smart Contract Security & Audit

Contracts underwent internal production-grade audit aligned with OpenZeppelin enterprise standards.

The contracts are subject to independent third-party external audit review.

All upgrades require:

1. Multi-signature approval  
2. Timelock scheduling  
3. Public execution  

---

## 16. Regulatory Positioning

NAX30:

- Does not represent equity ownership  
- Does not entitle holders to dividends  
- Does not constitute a collective investment scheme by default  
- Functions as a digital benchmark exposure instrument  

Regulatory classification may vary by jurisdiction.

---

## 17. Economic Rationale & Use Cases

NAX30 may support:

- Benchmark referencing  
- Structured product design  
- Treasury modeling  
- Research and capital allocation modeling  
- Digital settlement pair development  

---

## 18. Transparency & Versioning

All methodology changes are:

- Version-controlled  
- Publicly archived  
- Governance-executed  

Annual review may be conducted and published.

---

## 19. Structural Classification

NAX30 is:

- Fixed supply  
- Governance-minted  
- Non-redeemable  
- Market-priced  

It structurally resembles a digital benchmark commodity-style instrument rather than an ETF or structured note.

---

End of Whitepaper.
```0
End of Whitepaper.
