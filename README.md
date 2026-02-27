# Namibia 30 Index

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) ![Built with Solidity](https://img.shields.io/badge/built%20with-Solidity-363636) ![ERC-20 Compliant](https://img.shields.io/badge/ERC--20-Compliant-brightgreen) [![Security Policy](https://img.shields.io/badge/Security-Policy-blue.svg)](SECURITY.md)
![Creator](https://img.shields.io/badge/Creator-Simon%20Kapenda-lightgrey.svg)

## Institutional Repository

The Namibia 30 Index (NAX30) is a blockchain-native digital benchmark designed to reference a rules-based basket of thirty (30) selected securities listed on the [Namibia Securities Exchange (NSX)](https://nsx.com.na).

This repository contains the governance documentation, methodology framework, smart contract architecture references, and institutional policies governing the NAX30 benchmark.

NAX30 is structured as a modified weighted index and deployed as a BEP-20 token on the BNB Smart Chain (BSC).

Status: BNB Smart Mainnet Deployed  
Version: Institutional Governance Framework v2.0  
Audit Status: Internal review complete; external audit pending  

---

# 1. Institutional Positioning

NAX30 is designed to function as a composite market benchmark for Namibia’s listed equity market.

The index:

- Does not confer ownership in underlying NSX-listed securities
- Does not entitle holders to dividends or corporate rights
- Does not represent equity, debt, or units in a collective investment scheme by default
- Is not an ETF
- Is not asset-backed
- Is not redeemable against underlying securities
- Functions as a digital benchmark exposure instrument

Market price is determined by open market supply-demand dynamics.

There is no redemption mechanism linking token value to underlying securities.

Premium or discount to indicative benchmark value may persist.

---

# 2. Economic Context

Globally, benchmark indices serve as directional indicators of market performance:

- DAX (Germany)
- Dow Jones Industrial Average & S&P 500 (United States)
- Nikkei 225 (Japan)
- FTSE 100 (United Kingdom)

NAX30 is structured to serve a comparable benchmark function within Namibia’s capital markets infrastructure.

As a composite benchmark:

- Upward movement reflects strengthening aggregate performance.
- Downward movement indicates weakening market sentiment.

NAX30 may serve as a directional indicator of Namibia’s listed equity market performance.

---

# 3. Index Overview

- Index Name: Namibia 30 Index
- Symbol: NAX30
- Blockchain: BNB Smart Chain (BSC)
- Token Standard: ERC-20 / BEP-20 compatible
- Decimals: 18
- Maximum Supply: 10,000,000,000 NAX30
- Governance: Multi-Signature Safe + TimelockController
- Oracle Framework: 2-of-3 quorum
- Base Index Level: 10,000 basis points (bps)
- Creator: [Simon Kapenda](https://linkedin.com/in/simonkapenda)     

Full methodology is available in INDEX_METHODOLOGY.md.

---

# 4. Current Constituents

The NAX30 benchmark currently references the following 30 NSX-listed securities:

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
30. Reconnaissance Energy Africa Ltd  

Constituents are subject to periodic review in accordance with INDEX_METHODOLOGY.md.

---

# 5. Deployment Architecture (BSC Mainnet)

Deployer:  
0xe844443EBfc36e99C1868584F9cDB52385Ac89c6  

Timelock Controller:  
0xdc38cab671EECbd13D5c8771DC44C5729C2B4267  

Registry Contract:  
0x960cc4EB352c6B920a05Dc3A97BED768E551c4f8  

Multi-Signature Safe:  
0x397314A5CAA3F891A2d85DAc109be2078b510155  

NAX30 Proxy (Primary Token Address):  
https://bscscan.com/address/0xaAd81eb1f27874B8B0CB03C778C6019ea32045Ff  

Implementation Contract:  
https://bscscan.com/address/0x8293C888fFa3601E4197e63f2924E10cA32e5d88  

Contracts are verified on BscScan.

---

# 6. Secondary Market Disclosure

NAX30 tokens may be admitted for trading on secondary market venues, subject to independent venue approval and applicable regulatory considerations. Secondary market trading is market-driven, non-redeemable, and subject to liquidity, volatility, exchange counterparty, and blockchain infrastructure risks. NAX30 does not guarantee price stability, liquidity provision, or alignment with theoretical index value.

Participants should review the full Secondary Market Disclosure before engaging in any secondary trading activity:

See: [SECONDARY_MARKET_DISCLOSURE.md](./SECONDARY_MARKET_DISCLOSURE.md)

---

# 7. Governance Framework

NAX30 governance operates under a dual-layer control system:

### Multi-Signature Safe

- Proposal authority
- Threshold-controlled approvals
- Signer structure publicly visible on-chain
- Separation of duties enforced through governance design

### TimelockController

- Mandatory execution delay
- Deterministic operation identifiers
- Public auditability
- No bypass mechanism

All structural changes require Safe approval and timelock scheduling.

See: GOVERNANCE_CHARTER.md

---

# 8. Oracle Framework

The NAX30 oracle framework operates under a 2-of-3 quorum:

- Three designated oracle operators
- Minimum of two concurring submissions required
- Governance-controlled oracle rotation
- Timelock-based configuration updates

Data hierarchy:

1. Official NSX disclosures
2. Secondary validated feeds
3. Last traded price fallback

See: ORACLE_POLICY.md

---

# 9. Smart Contract Model

- Upgradeable proxy architecture
- Governance-controlled mint authority
- Fixed maximum supply
- No algorithmic emissions
- No automatic inflation

All upgrades require:

1. Multi-signature approval
2. Timelock scheduling
3. On-chain execution

See: CHANGE_CONTROL_POLICY.md

---

# 10. OTC Allocation Framework

NAX30 tokens may be distributed through structured OTC allocation processes subject to:

- Compliance review
- Allocation availability
- Cleared settlement
- Governance-controlled issuance

OTC Portal:
https://trade.nax30.io

Future exchange listing is subject to independent approval and market conditions.

---

# 11. Risk Considerations

Risks include:

- Market volatility
- Liquidity constraints
- Oracle dependency risk
- Smart contract upgrade risk
- Governance coordination risk
- Regulatory classification variability

No guarantee of price tracking to theoretical index value.

See: RISK_DISCLOSURE.md

---

# 12. Compliance & Regulatory Positioning

NAX30 is structured as a digital benchmark exposure instrument.

It does not represent:

- Equity ownership
- Fund units
- Depositary receipts
- Structured notes

Regulatory classification may vary by jurisdiction.

Governing Jurisdiction: Namibia.

See: REGULATORY_MEMORANDUM.md

---

# 13. Operational Independence

NAX30 is administered independently of any centralized exchange.

The index is not operated by the Namibia Securities Exchange.

There is no affiliation with listed constituents beyond benchmark referencing.

---

# 14. Transparency & Version Control

All structural changes are:

- Governance-approved
- Timelock-scheduled
- On-chain executed
- Publicly documented
- Version archived

Structured change tracking is maintained.

See: CHANGE_CONTROL_POLICY.md

---

# 15. Audit Status

Smart contracts have undergone internal production-grade review aligned with OpenZeppelin enterprise standards.

External independent audit engagement is planned.

See:
AUDIT_STATUS.md  
EXTERNAL_AUDIT_PLAN.md  

---

# 16. License

Unless otherwise specified, repository documentation is proprietary.

Smart contract licensing is defined within contract headers.

No reproduction or redistribution permitted without authorization unless explicitly licensed.

---

# Intellectual Property Notice

The MIT License applies to smart contract source code only.

All benchmark methodology, governance documentation, and brand materials are proprietary and subject to separate documentation license terms.

---

# 17. Contribution Policy

This repository is governance-controlled.

External contributions are not accepted without formal approval.

All changes must follow CHANGE_CONTROL_POLICY.md.

---

# 18. Security Contact

Security disclosures:
See SECURITY_CONTACT.md

Institutional inquiries:
admin@nax30.io

Official website:
https://nax30.io

---

# Disclaimer

NAX30 is a digital benchmark token designed to provide structured market exposure. It does not represent ownership in the underlying NSX-listed securities and does not constitute investment advice or a solicitation in any jurisdiction where such activity would be unlawful.

---

End of README.
