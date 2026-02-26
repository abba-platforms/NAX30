# NAX30 CHANGE CONTROL POLICY  
Namibia 30 Index (NAX30)

Version 2.0 – Institutional Change Governance Standard  
Effective Date: February 2026  

---

## 1. Purpose

This Change Control Policy establishes the formal framework governing modifications to the Namibia 30 Index (NAX30) smart contracts, governance configuration, oracle framework, and documentation.

The objective is to ensure:

- Predictable governance execution  
- Transparent modification procedures  
- Controlled upgrade discipline  
- Institutional-grade change traceability  
- Risk-aware protocol evolution  

---

## 2. Scope

This policy applies to changes involving:

- Smart contract upgrades (Proxy / Implementation)
- Registry updates (weights / constituents)
- Governance parameter adjustments
- Oracle configuration changes
- Mint authorization and supply actions
- Timelock configuration modifications
- Governance signer changes
- Documentation updates affecting benchmark methodology

Frontend applications and external exchange infrastructure are outside the scope of this document unless explicitly integrated into governance processes.

---

## 3. Change Classification

Changes are categorized as:

### 3.1 Major Changes

Changes that may materially affect:

- Token logic
- Access controls
- Supply mechanics
- Governance structure
- Oracle quorum rules
- Calculation methodology

Major changes require:

- Governance proposal
- Multi-signature Safe approval
- Timelock scheduling
- Public on-chain execution
- Public documentation update

External audit review may be required prior to execution.

---

### 3.2 Moderate Changes

Changes involving:

- Registry weight updates
- Constituent modifications
- Oracle address rotation
- Governance signer rotation

Moderate changes require:

- Governance proposal
- Timelock scheduling
- Public documentation update

Audit review may be recommended depending on impact.

---

### 3.3 Minor Changes

Changes involving:

- Non-structural documentation updates
- Clarification language
- Formatting adjustments

Minor changes do not require governance execution but must be version-controlled and documented.

---

## 4. Governance Pathway

All on-chain structural changes must follow:

1. Proposal creation via Multi-Signature Safe  
2. Safe approval meeting threshold  
3. TimelockController scheduling  
4. Mandatory delay expiration  
5. On-chain execution  

No change may bypass the timelock.

---

## 5. Code Freeze Policy

For Major Changes:

- Code freeze must be declared prior to governance scheduling.
- Relevant commit hash must be tagged.
- Upgrade bytecode must be verified.

Changes during active audit invalidate audit coverage unless re-reviewed.

---

## 6. Documentation Requirements

All Major and Moderate changes must include:

- Updated documentation (Whitepaper, Methodology, Technical Architecture where applicable)
- Version increment
- Public repository commit
- Clear summary of change rationale

Transparency is mandatory.

---

## 7. Risk Review

For Major Changes:

- Risk Committee review is required.
- External audit may be recommended.
- Regulatory implications must be evaluated.

Change execution may be delayed if material risk is identified.

---

## 8. Emergency Changes

In the event of critical vulnerability:

- Emergency governance proposal may be initiated.
- Timelock delay remains enforceable unless emergency override mechanism is formally defined and disclosed.
- Public disclosure must follow execution.

No undocumented emergency powers exist.

---

## 9. Immutable Constraints

The following constraints are structurally enforced unless modified through governance-approved upgrade:

- Maximum supply cap (10,000,000,000 NAX30)
- ERC-20 token standard compliance
- Governance-based mint control
- Registry normalization to 10,000 basis points

Historical transaction records cannot be modified.

---

## 10. Versioning & Archiving

All changes must:

- Increment version number
- Be archived in repository history
- Maintain prior versions for audit traceability

No prior documentation may be deleted without archival preservation.

---

## 11. Audit Integration

Major changes may trigger:

- External audit engagement
- Targeted security review
- Remediation cycle prior to activation

Audit findings must be addressed according to EXTERNAL_AUDIT_PLAN.md.

---

## 12. Regulatory Considerations

Material changes must assess potential impact on:

- Securities classification
- MiCA or equivalent digital asset frameworks
- Benchmark regulatory positioning
- AML or compliance implications

Legal review may be obtained prior to execution.

---

## 13. Transparency Principle

All structural changes are:

- Publicly visible on-chain
- Publicly documented in repository
- Subject to governance auditability

Commercial considerations must not override benchmark integrity.

---

## 14. Prohibited Changes

The following actions are prohibited without full governance pathway:

- Unilateral minting
- Direct registry manipulation
- Bypassing timelock delay
- Altering historical blockchain data
- Introducing hidden access control roles

---

## 15. Annual Policy Review

This Change Control Policy shall be reviewed annually.

Amendments require governance approval and documentation update.

---

# Institutional Additions (Version 2.0 Enhancements)

---

## 16. Formal Change Impact Assessment (CIA)

All Major Changes must include a documented Change Impact Assessment covering:

- Technical impact
- Backward compatibility assessment
- Security implications
- Oracle dependency implications
- Liquidity and market impact
- Legal and regulatory impact
- Governance impact

The CIA must be archived in repository history.

---

## 17. Change Approval Matrix

Change approval requirements are as follows:

- Major Change → Multi-Signature + Timelock + Risk Committee Review  
- Moderate Change → Multi-Signature + Timelock  
- Minor Change → Documentation control only  

Where ambiguity exists, the higher classification applies.

---

## 18. Rollback Policy

If an upgrade introduces unintended consequences:

- A rollback proposal may be initiated through governance.
- Rollback follows identical governance pathway (Safe + Timelock).
- Rollback may not reverse historical blockchain state.
- Only implementation logic may be reverted.

Rollback feasibility depends on proxy upgrade architecture constraints.

---

## 19. Separation of Duties

Where practicable:

- Proposal initiators should not be sole approvers.
- Governance signers should not directly control oracle submission.
- Operational roles must remain segregated from governance approval authority.

Conflict management is governed by CONFLICT_OF_INTEREST_POLICY.md.

---

## 20. Notice & Communication Requirements

For Major Changes:

- Public notice must be issued prior to timelock execution.
- Notice should include summary, impact classification, and execution timeline.
- On-chain transaction hash must be published post-execution.

Transparency precedes activation.

---

## 21. Dependency & Library Change Controls

Changes involving:

- Solidity compiler version
- OpenZeppelin dependency versions
- Safe contract upgrades
- Timelock contract modifications

Must be classified as Major Changes and may require external audit review.

---

## 22. Timelock Parameter Controls

Any modification to:

- Timelock delay duration
- Timelock proposer role
- Timelock executor role

Must be classified as Major Change.

Reduction of delay period requires explicit public justification.

---

## 23. Stakeholder Communication Framework

Official communication channels may include:

- Repository publication
- Website notice
- Exchange notification (if listed)
- Public governance announcement

Change communication must occur prior to execution for Major Changes.

---

## 24. Change Audit Log Requirement

All executed changes must include:

- Governance proposal reference
- Timelock operation ID
- Execution transaction hash
- Parameter before/after summary
- Documentation version reference

A structured change log must be maintained.

---

## 25. Post-Implementation Review

Following Major Changes:

- A monitoring period must be observed.
- Index calculation integrity must be verified.
- Oracle submission consistency must be reviewed.
- Governance state must be validated.

A post-implementation review summary may be published.

---

End of Change Control Policy.
