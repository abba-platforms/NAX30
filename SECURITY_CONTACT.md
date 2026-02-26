# NAX30 Security Contact & Responsible Disclosure  
Namibia 30 Index (NAX30)

Version 2.0 – Tier-1 Institutional Security Reporting Framework  
Effective Date: February 2026  

---

## 1. Purpose

This document establishes the security contact procedure and responsible disclosure framework for the Namibia 30 Index (NAX30) smart contract and governance infrastructure.

The objective is to:

- Provide a clear channel for vulnerability reporting  
- Encourage responsible disclosure  
- Protect benchmark integrity  
- Reduce systemic risk  

This policy does not eliminate technological risk.

---

## 2. Scope

This policy applies to:

- NAX30 smart contracts (Proxy, Implementation, Registry)  
- Governance contracts (TimelockController, Multi-Signature Safe)  
- Oracle submission logic  
- Related on-chain infrastructure  

This policy does not apply to:

- Third-party exchanges  
- Wallet software  
- Blockchain validator infrastructure  
- External service providers  
- Social engineering attacks  
- Phishing domains  
- Third-party forks  
- Economic design critiques (non-security issues)  

---

## 3. Reporting a Vulnerability

Security researchers who identify a potential vulnerability should report it to:

**Email:** security@nax30.io  

Reports should include:

- Description of the vulnerability  
- Affected contract address(es)  
- Steps to reproduce  
- Proof-of-concept (if applicable)  
- Potential impact assessment  
- Suggested remediation (if available)  

Reports should be submitted in good faith and without public disclosure prior to remediation.

---

## 4. Encrypted Communication (PGP)

Researchers may request a PGP public key for encrypted communication.

If implemented, the official public key and fingerprint will be published in this document.

Until a public key is formally published, encrypted reporting may be coordinated via direct request.

---

## 5. Response Targets

The Administrator aims to:

- Acknowledge receipt within 72 hours  
- Assess severity within a commercially reasonable timeframe  
- Provide remediation plan if material  

Response times are targets, not guarantees.

---

## 6. Severity Classification

Reported vulnerabilities may be classified as:

- **Low:** Minimal impact, no material risk to benchmark integrity  
- **Medium:** Limited functional risk without systemic compromise  
- **High:** Material vulnerability affecting smart contract or governance integrity  
- **Critical:** Exploitable issue capable of causing systemic compromise  

Severity classification determines remediation priority.

---

## 7. Response Process

Upon receipt of a valid report:

1. Acknowledge receipt  
2. Assess reproducibility  
3. Classify severity  
4. Escalate to Index Committee and Governance Safe if required  
5. Schedule remediation through timelock if necessary  
6. Coordinate disclosure timing  

Critical vulnerabilities may trigger emergency governance review.

---

## 8. Responsible Disclosure Expectations

Researchers must:

- Avoid exploiting the vulnerability  
- Avoid accessing funds or private data  
- Avoid disruption of network services  
- Avoid public disclosure prior to remediation  
- Limit testing to proof-of-concept validation  

This policy does not authorize active penetration testing on mainnet without permission.

Unauthorized access or exploitation may violate applicable laws.

---

## 9. Safe Harbor (Good Faith Research)

The Administrator will not pursue legal action against researchers who:

- Act in good faith  
- Avoid exploitation  
- Follow responsible disclosure process  
- Provide reasonable remediation window  

This safe harbor does not apply to malicious or exploitative activity.

---

## 10. Coordinated Disclosure

Following remediation:

- The Administrator may publish a summary  
- The vulnerability may be disclosed publicly  
- Audit status documentation may be updated  

Disclosure timing may consider:

- Risk mitigation completion  
- Market impact  
- System stability  

In critical cases, accelerated disclosure may occur.

---

## 11. Governance Key Compromise & Rotation

If governance key compromise is suspected:

- Immediate internal review initiated  
- Governance may remove affected signer  
- Replacement executed via Safe + Timelock  
- Event recorded on-chain  

Key rotation procedures may be implemented as part of remediation.

---

## 12. Security Monitoring

Security posture includes:

- Monitoring of governance transactions  
- Oracle behavior review  
- Public on-chain verification  
- Periodic internal review  

Continuous monitoring does not eliminate risk.

---

## 13. Bug Bounty Status

As of the Effective Date:

- No formal bug bounty program is active.  

A formal bounty framework may be introduced in the future.

---

## 14. Jurisdiction & Legal Compliance

Vulnerability reporting must comply with:

- Applicable Namibian law  
- Applicable international law  
- Blockchain network usage policies  

This policy does not grant immunity from unlawful conduct.

---

## 15. Limitation of Liability

Submission of a vulnerability report does not:

- Create contractual relationship  
- Guarantee financial compensation  
- Authorize system exploitation  
- Transfer ownership of intellectual property  

Participation is voluntary.

---

## 16. Residual Risk Disclosure

While responsible disclosure mechanisms are in place:

- Smart contract systems carry inherent risk  
- Not all vulnerabilities may be detected  
- Third-party dependencies remain outside direct control  

Participants should assume residual technological risk exists.

---

End of Security Contact & Responsible Disclosure Policy.
