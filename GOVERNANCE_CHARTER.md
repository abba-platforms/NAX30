# NAX30 Governance Charter

Version 2.0 – Tier-1 Institutional Benchmark Governance Standard  
Effective Date: February 2026  

---

## 1. Purpose

This Governance Charter defines the administrative, procedural, and structural framework governing the Namibia 30 Index (NAX30).

The objectives of this Charter are to:

- Establish formal oversight mechanisms  
- Define governance authority boundaries  
- Prevent unilateral control  
- Ensure transparency and auditability  
- Align on-chain execution with institutional change management standards  
- Protect benchmark integrity and market neutrality  

NAX30 governance operates under a two-layer control architecture:

1. Multi-Signature Safe (proposal authority)  
2. TimelockController (execution delay enforcement)  

---

## 2. Governance Structure

### 2.1 Multi-Signature Safe

The Multi-Signature Safe:

- Holds proposal authority  
- Requires threshold-based approvals  
- Prevents unilateral administrative action  
- Serves as primary governance proposer  

Safe signer structure:

- Minimum of three (3) independent signers  
- Threshold requirement publicly verifiable on-chain  
- No single signer may independently execute a governance action  

Signer eligibility criteria:

- Demonstrated operational competency  
- No active regulatory disqualification  
- No material conflicts of interest related to index constituents  

Key rotation:

- Signer changes require Safe approval and timelock scheduling  
- All signer modifications are on-chain and auditable  

---

### 2.2 TimelockController

The TimelockController:

- Enforces a mandatory execution delay  
- Generates deterministic operation identifiers  
- Emits scheduling and execution events  
- Ensures transparency prior to structural change  

Minimum delay duration:

- A non-zero mandatory delay period is enforced  
- Any modification of delay duration requires full governance process  

No governance action may execute without timelock scheduling and delay expiration.

---

## 3. Scope of Governance Authority

Governance authority includes, but is not limited to:

- Index constituent updates  
- Weight adjustments  
- Divisor adjustments  
- Oracle operator modification  
- Quorum threshold adjustments  
- Tolerance parameter modification  
- Smart contract upgrades  
- Registry configuration changes  
- Emergency suspension actions  

Governance does not include:

- Direct price manipulation authority  
- Manual override of calculated index values  
- Redemption enforcement  
- Interference with open market trading  

---

## 4. Change Management Process

All governance changes follow the standardized lifecycle:

1. Proposal drafted  
2. Multi-signature Safe approval (threshold met)  
3. Timelock scheduling  
4. Mandatory delay period  
5. On-chain execution  
6. Public event emission  

This ensures:

- Predictability  
- Auditability  
- Delay transparency  
- Stakeholder awareness  

---

## 5. Governance Transparency & Reporting

All governance actions:

- Are publicly recorded on-chain  
- Emit traceable events  
- Can be independently verified  
- Are version-controlled  

Governance activity reporting:

- Material changes must be documented  
- Repository updates must correspond with on-chain actions  
- Annual governance activity summary may be published  

---

## 6. Index Oversight Committee

An Index Oversight Committee may operate in an advisory capacity to:

- Review methodology updates  
- Assess constituent eligibility  
- Evaluate extraordinary events  
- Recommend structural adjustments  

The Committee does not possess unilateral execution authority.

All decisions require formal governance execution via Safe + Timelock.

---

## 7. Emergency Governance Procedures

In the event of:

- Exchange closure  
- Oracle quorum failure  
- Critical contract vulnerability  
- Data integrity compromise  
- Signer key compromise  

Governance may initiate emergency review.

Emergency actions may include:

- Temporary suspension of index updates  
- Oracle operator replacement  
- Signer removal or replacement  
- Parameter adjustment  
- Contract upgrade scheduling  

All emergency interventions must follow governance procedures unless explicitly defined in smart contract logic.

---

## 8. Key Compromise & Recovery Policy

If a Safe signer key is:

- Lost  
- Compromised  
- Inaccessible  

Governance may:

1. Remove the affected signer  
2. Replace with an approved signer  
3. Document the change publicly  

Replacement requires Safe threshold approval and timelock scheduling.

---

## 9. Oracle-Governance Separation Principle

Structural separation is enforced:

- Oracle operators cannot unilaterally control governance  
- Governance signers do not directly submit oracle price data  
- Registry modifications do not bypass quorum confirmation  

This separation mitigates structural manipulation risk.

---

## 10. Smart Contract Upgrade Governance

NAX30 utilizes upgradeable proxy architecture.

All upgrades require:

1. Safe multi-signature approval  
2. Timelock scheduling  
3. On-chain execution  

Upgrade transparency requirements:

- Implementation contract address published  
- Change summary documented  
- Version number incremented  
- Security considerations disclosed  

No upgrade may occur without governance scheduling.

---

## 11. Governance Ethics & Independence

Governance operates under principles of:

- Market neutrality  
- Non-interference with price formation  
- Conflict-of-interest avoidance  
- Transparency of structural changes  

Governance does not:

- Act as an investment advisor  
- Provide financial guarantees  
- Influence trading behavior  

---

## 12. Governance Risk Considerations

Governance risks include:

- Key management failure  
- Collusion risk within Safe threshold  
- Operational coordination delays  
- Timelock misconfiguration  

Mitigation measures include:

- Multi-signature thresholds  
- Mandatory delay enforcement  
- On-chain transparency  
- Public auditability  
- Separation of duties  

---

## 13. Separation of Duties

Governance separation principles:

- Oracle operators do not control governance  
- Governance does not control market price  
- Token holders do not automatically control registry  
- Registry updates require formal scheduling  

This separation reduces systemic concentration risk.

---

## 14. Jurisdiction & Legal Framework

NAX30 governance operates under the legal framework applicable to its governing entity.

Regulatory interpretation of digital benchmark instruments may vary by jurisdiction.

This Charter does not create fiduciary obligations beyond defined governance roles.

---

## 15. Governance Amendments

This Charter may be amended only through:

1. Formal proposal  
2. Safe threshold approval  
3. Timelock scheduling  
4. On-chain execution  

Amendments must be:

- Versioned  
- Archived  
- Publicly accessible  

---

## 16. Governance Dissolution or Transition

If governance structure requires transition:

- Signer set modifications must be executed via governance  
- Registry and timelock authority must remain publicly auditable  
- Control may not be transferred without on-chain scheduling  

Continuity of benchmark integrity is paramount.

---

## 17. Structural Classification

Governance framework supports NAX30 as:

- A governance-controlled digital benchmark instrument  
- A non-redeemable, market-priced asset  
- A methodology-driven reference index  

Governance does not create ownership claims in underlying securities.

---

## 18. Disclaimer

This Governance Charter defines administrative procedures for the NAX30 digital benchmark framework.

It does not:

- Guarantee performance  
- Provide investment advice  
- Alter regulatory classification  
- Create fiduciary obligations beyond defined governance roles  

Regulatory interpretation may vary by jurisdiction.

---

End of Governance Charter.
