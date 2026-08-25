# Execution & Treasury Actions Policy

| Field | Value |
|---|---|
| **Version** | v1.0.0 |
| **Last updated** | 2026-08-25 |

---

## 1. Scope

This document defines:

* How approved proposals are executed
* How treasury actions are carried out
* Who is authorized to execute decisions
* Safeguards around execution and fund usage

---

## 2. [Reserved]

*This section number is retained, rather than renumbered, so that references to the sections below remain stable.*

---

## 3. Execution Principles

All execution must follow these principles:

* **Fidelity** — Actions must match the approved proposal
* **Authorization** — Only designated entities may execute
* **Transparency** — All actions must be publicly recorded
* **Reversibility Awareness** — Irreversible actions require higher scrutiny

---

## 4. Types of Execution

### 4.1 On-Chain Execution

* Automated execution via smart contracts
* Triggered by approved proposals
* Preferred where possible

---

### 4.2 Off-Chain Execution

* Legal agreements
* Payments via external systems
* Operational actions

Must follow governance-approved instructions.

---

### 4.3 Hybrid Execution

* Combination of on-chain and off-chain
* Example: on-chain approval + off-chain implementation

---

## 5. Execution Authority

Execution may be carried out by:

* Smart contracts (automated)
* Treasury signers (e.g., multisig)
* Working Groups (within mandate)

---

### 5.1 Role of RAC

* Ensures execution follows approved decisions
* Verifies compliance
* Does NOT independently execute strategic actions

---

### 5.2 Role of Working Groups

* Execute within approved scope
* Manage operational delivery
* Coordinate contributors

---

### 5.3 Role of Treasury Signers

Treasury Signers are responsible for carrying out treasury execution actions approved by governance.

They:
* execute approved actions within defined time limits
* operate under multi-signature controls
* may refuse or delay execution only on the grounds defined in **Treasury Signers Rules §9**
* remain accountable to DAO governance

Where RAC determines that a refusal is invalid, or where a proposal remains unexecuted beyond the 10-business-day backstop window defined in the Governance Continuity Framework §4.2, RAC may instruct remaining signers to proceed with execution directly.

Detailed operational rules are defined in the Treasury Signers Operational Rules.

---

### 5.4 Execution of DAO-Wide Roles

Every approved proposal that creates a paid role must designate an executing body responsible for selection, onboarding, and contracting.

* If the role falls within a Working Group's mandate, that Working Group is the executing body.
* If the role is DAO-wide with no natural Working Group home, the proposal must explicitly name the executor — either a specific Working Group or the RAC.

**When the RAC is the designated executor:**

The RAC must publicly document the selection process and publish its selection decision to the governance forum for a 7-day acknowledgement period before the engagement is binding. During this period, any Governance Participant holding at least the Compliance Challenge Filing Threshold (DAO Parameters §4) may file a Compliance Challenge (Proposal & Voting Framework §8) on the grounds that the selection does not comply with the approved proposal. The acknowledgement period is the filing window for a challenge under this section.

The RAC may not act as both executor and compliance verifier for the same role. Where the RAC executes a hire, compliance verification responsibility passes to the DAO via the acknowledgement period above.

---

## 6. Treasury Structure

Treasury structure — including multi-account segmentation, multisig thresholds, custody requirements, and audit obligations — is defined in **DAO Parameters §6.2** and **§6A**. Signer-specific security requirements are defined in **Treasury Signers Rules §16**.

---

## 7. Treasury Actions

### 7.1 Authorized Actions

* Transfers
* Grant disbursements
* Payments to contributors
* Operational expenses

---

### 7.2 Restrictions

Treasury actions must NOT:

* Exceed approved budgets
* Deviate from proposal intent
* Be executed without proper authorization
* Be paid to any recipient whose KYC/AML compliance status is unknown or unverified, where KYC is required under the **Contributor Compensation Policy §3.5** or **Operating Agreement §10.4**

---

### 7.3 Cost Models

Treasury disbursements for work-related proposals must specify one of three cost models:

**Model A — Documented expense recovery**
Actual out-of-pocket costs incurred on behalf of the DAO (hosting, tooling, domain fees, travel). Payment is made against submitted receipts or third-party invoices. No labour component.

**Model B — Fixed-rate service delivery**
A flat fee for a defined, verifiable service outcome. The provider uses existing capability (infrastructure, vehicle, skills) acquired independently. The provider volunteers their time and effort; the DAO pays only for the cost of the service output, not for hours worked. No itemized receipts are required — accountability is through outcome verification.

**Model C — Fully compensated work**
Labour plus costs, with defined deliverables, milestones, and reporting obligations. Applies to grants, contractor agreements, and contributor compensation.

---

### 7.4 Payment Documents

All treasury payments must be initiated against a payment document:

* **Invoice** — issued by a registered company or sole trader operating as a business. Must include: provider name and registration details, service description, amount, period covered, and payment address.

* **Monthly claim** — submitted by a private individual. Must include: provider name and wallet address, service description matching the approved proposal, amount, and period covered. No registration details required.

RAC verifies each payment document against the approved proposal before Treasury Signers release payment. Verification confirms: (a) the document matches the approved service and fee, (b) the period claimed has not already been paid, (c) the total does not exceed the authorized commitment.

---

### 7.5 Standing Service Authorization

A governance vote authorizing a recurring fixed-rate service (Model B) constitutes a standing authorization for the full approved term. Treasury Signers may release payment each period upon receipt of a verified claim or invoice without a new governance vote.

Requirements:

* The proposal must state the fee, payment frequency, and maximum term.
* The total authorized commitment (fee × term) is calculated at proposal time and displayed explicitly in the proposal.
* Default maximum term: **6 months**. Longer terms require explicit justification in the proposal.
* At term end, continuation requires a new proposal. RAC may not extend a standing authorization unilaterally.
* The DAO may terminate a standing authorization early via a Governance Process proposal.

---

### 7.6 Treasury Inflows — Donations

The DAO may receive and hold unsolicited, unconditional donations without prior governance approval, provided that:

1. The transfer does not impose any legal, contractual, or operational obligations on the DAO.
2. No rights, ownership claims, or influence over governance are granted in connection with the transfer.
3. The source of funds does not violate applicable law or compliance requirements.

All donations must be:

* Publicly disclosed on the governance forum within **30 days** of receipt, identifying the source (or, where the source is anonymous, that the donation was anonymous) and the amount.
* Recorded in treasury reporting.

Treasury Signers may refuse or return funds if:

* The source is reasonably suspected to be unlawful or sanctioned.
* The transfer includes explicit or implicit conditions.
* Acceptance would create material reputational risk.

Any donation that includes conditions, expectations, or earmarked use must be approved via a Governance Proposal before acceptance.

---

## 8. Budget Execution

Each approved budget must include:

* Scope of spending
* Maximum allocation
* Timeframe

Personnel-cost rules — Steward and contributor rates, RFP thresholds, KYC prerequisites for payment, and expense reimbursement — are defined in the **Contributor Compensation Policy**. Working Group authority over its own budget is set in the **Working Group Framework §7** and is subject to the variance limits in §7.1 of that framework.

---

### 8.1 Spending Within Budget

Working Groups may:

* Allocate funds within approved limits
* Issue RFPs and pay contributors per the **Contributor Compensation Policy**

---

### 8.2 Spending Outside Budget

Requires new governance approval.

---

## 9. Execution Workflow

1. Proposal passes
2. Execution plan confirmed
3. Authorized entity executes
4. Action recorded publicly
5. Outcome reported

---

## 10. Transparency & Reporting

All execution actions must:

* Be publicly visible (on-chain or reported)
* Include sufficient detail for accountability

---

### 10.1 Exceptions

Limited confidentiality is allowed where:

* Required for security
* Required for legal obligations

Confidential actions must be disclosed retrospectively according to the following deadlines:

* **Security-related confidentiality** — no later than **90 days** after the action was taken, or when the security basis no longer applies, whichever is sooner
* **Legal-related confidentiality** — no later than **12 months** after the action was taken, or when the legal proceeding or obligation concludes, whichever is sooner
* Extensions beyond these deadlines require a governance vote

Throughout the confidentiality period the RAC must maintain a confidential record of the action and its basis, which becomes part of the retrospective disclosure.

---

## 11. Verification & Compliance

The RAC is responsible for:

* Verifying execution matches proposal
* Flagging deviations
* Ensuring governance compliance

---

## 12. Execution Failure

If execution of an approved proposal fails or cannot be completed:

1. The executor reports the failure to the RAC within **24 hours** of identifying the blocker.
2. The RAC publishes a disclosure to the governance forum within **48 hours** of notification, including the nature of the failure and any immediate mitigation steps.
3. If the failure cannot be resolved operationally within the execution window, the RAC schedules a Governance Process proposal for community review and remediation within **14 days** of disclosure.
4. If the failure involves a security event or threat to treasury assets, the **Emergency & Safeguards Policy §4** applies and takes precedence over this procedure.

---

## 13. Dispute Handling

Execution disputes are resolved via:

* Governance processes
* Dispute Resolution Policy

---

## 14. Irreversible Actions

Actions that cannot be undone (e.g., large transfers) require:

* Clear proposal specification
* Higher scrutiny during review
* Mandatory pre-execution hold — Treasury Signers must not initiate execution of any Treasury / Budget or Executable proposal until the Compliance Challenge Window has fully closed (per **DAO Parameters §9**). High-risk actions (requiring 4-of-5 signers post-activation, or unanimity of all seated signers during the Transition Period — DAO Parameters §6A) must additionally observe the extended hold defined in **DAO Parameters §9**. Signers who execute before the hold period expires are in breach of their duties under the Treasury Signers Rules regardless of whether a Compliance Challenge is filed.

---

## 15. Delegation & Sub-Execution

Working Groups may:

* Delegate tasks to contributors
* Create sub-processes

Responsibility remains with the Working Group.

---

## 16. Records & Auditability

All execution must:

* Be recorded
* Be auditable
* Maintain historical traceability

---

## 17. Governance Parameters

Defined separately:

* Spending thresholds
* Multisig requirements
* Execution delays (if any)

---

## 18. Amendments

_Amendment procedures and classification requirements are defined in the **Governance Maintenance & Upgrade Framework**._
