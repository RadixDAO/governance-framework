# Treasury Signers Operational Rules

*Version v1.0.0 — Last updated 2026-08-27*

---

## 1. Purpose

This document defines the operational rules for Treasury Signers.

Treasury Signers are responsible for carrying out approved treasury actions on behalf of the DAO, within strictly limited authority.

They are execution agents, not decision-makers.

---

## 2. Scope

These rules apply to:

* treasury transactions
* custody actions
* contract signing
* execution of approved off-chain actions

---

## 3. Role of Treasury Signers

Treasury Signers may:

* execute treasury transfers approved by governance
* sign agreements authorized by governance
* operate approved custody systems
* perform administrative actions needed to maintain DAO operations

Treasury Signers may not:

* make strategic decisions
* approve new spending
* change proposal intent
* act outside approved mandates
* withhold execution for political reasons
* cast or direct any governance vote from a treasury account
* exercise, transfer, or withdraw the Master Badge or the Owner Badge otherwise than as permitted by the On-Chain Identifiers & Verification Policy §4 — these are held in the treasury account but are instruments of governance control, not treasury assets, and are outside the ordinary signing mandate

These restrictions apply to the exercise of the Treasury Signing function and do not govern conduct in any other role the same person may simultaneously hold.

---

## 4. Core Principles

All signer activity must follow these principles:

### 4.1 Fidelity

Execution must match the approved proposal exactly, or as closely as operationally possible.

### 4.2 Limited Authority

Signers only implement decisions; they do not interpret governance expansively.

### 4.3 Security

All signing activity must prioritize asset protection and operational security.

### 4.4 Accountability

All signer actions must be auditable and attributable.

---

## 5. Eligibility

Treasury Signers must:

* be approved through DAO governance
* satisfy required KYC / legal checks where applicable
* demonstrate operational reliability
* be capable of maintaining confidentiality where needed for security
* not be disqualified by conflict rules

---

## 6. Appointment

A Treasury Signing seat is filled in one of two ways, and which applies is fixed by the roster composition under **Delegate Mandate §3.1**:

* an **allocated seat** is filled by RAC allocation from among seated RAC members, published with reasons to the Official Venue (**Delegate Mandate §3**), and runs with the holder's RAC seat; and
* an **elected seat** is filled by Election Proposal under the **Elections & Role Governance Policy §§5–9**, its holder need not hold a RAC seat, and it carries its own term (**DAO Parameters §6A** — Signer Term Length).

Where the RAC cannot fill an allocated seat from among its seated members, the conversion duty in **Delegate Mandate §3.3** requires it to publish a certificate and open that seat to election rather than leave the roster short.

Where a seat is filled by election, the election proposal must include:

* identity or confidential identity verification pathway
* relevant qualifications
* conflict disclosures
* scope of authority
* term length

---

## 7. Removal

Treasury Signers may be removed by DAO vote at any time.

Immediate suspension may occur through emergency procedures where:

* signer keys are compromised
* signer misconduct is credibly alleged
* signer becomes unavailable in a way that threatens operations

---

## 8. Execution Duties

Treasury Signers must:

* execute valid approved actions within the required time window
* confirm receipt of execution requests
* maintain accurate execution records
* coordinate with relevant Working Groups and legal operators
* escalate ambiguities or blockers promptly

---

### 8.1 Valid Execution Request Format

A valid execution request must include all of the following:

* Reference to the passed governance proposal (proposal ID or equivalent)
* Description of the action to be executed
* Recipient address or counterparty
* Amount or scope (for treasury actions)
* Required execution deadline
* Name or identifier of the requesting Working Group or governance body
* Any supporting documentation required by the proposal

Requests that are missing required fields must not be executed. Signers must notify the requesting party of the missing information within the Max Acknowledgement Window (see DAO Parameters §6A).

---

### 8.2 Verification Against Disbursement Limits

Before signing, each signer must verify the requested disbursement against the budget limits in **DAO Parameters §6.1**. These limits bind the signers directly: a passed proposal authorises a payment, but it does not authorise a payment that breaches a limit, and no proposal is self-executing against this section. From the **Activation Date**, verification covers:

* **Single Transaction Limit.** No single transaction may exceed it, unless the disbursement is authorised as a **Large Milestone Authorization** under DAO Parameters §6.1A, in which case §8.2A applies.
* **Rolling 30-Day Outflow Cap.** The signers maintain a **running total** of all Treasury / Budget disbursements executed in the trailing 30 days, across all passed proposals and all treasury accounts, recorded under §12. Before signing, the signer confirms that the requested disbursement would not carry that total past the cap. The cap is the **lower** of its two legs, so where treasury value has fallen the 5% leg may bind well below the stated figure; the signers value the treasury at the time of verification and record the figure used.
* **One-time outflow uplift.** Where a proposal has granted an uplift under DAO Parameters §6.1B, the signers apply the **uplifted figure in place of the standing cap, and only within the single rolling 30-day window in which the authorised disbursement executes**. Every other disbursement executed in that window counts against the uplifted figure in the ordinary way: an uplift enlarges the window, it does not exempt the authorised payment or reserve headroom for it. The signers record the window's opening and closing dates under §12. On expiry the standing cap in §6.1 resumes **automatically** — no vote, notice, ratification, or act of any body is required to restore it, and the signers may not carry an uplifted figure into a later window. An uplift stated without express amending words is one-time; the signers may not treat it as a change to the §6.1 value.
* **Non-USDC disbursements.** Where the disbursement is made other than in USDC, the signer measures it at its **USDC-equivalent value at the moment of execution**, using the method in DAO Parameters §6.1 (*Measuring non-USDC disbursements*) and the price source register in the **On-Chain Identifiers & Verification Policy §5A**, and records the rate, source, and valuation time under §12. A disbursement authorised under DAO Parameters §6.1A remains authorised despite movement in value since the authorising vote — the DAO authorised a quantity, not a valuation — but it is never exempt from the Rolling 30-Day Outflow Cap, which is applied at execution value in every case.
* **Scheduled payments and structuring.** Where the requested disbursement forms part of a larger obligation, the signer first applies the measurement test in DAO Parameters §6.1 (*How a scheduled payment is measured*). Where the schedule satisfies **both** limbs of that test — each payment corresponding to a distinct period, milestone, or budget period, and the schedule visible to the DAO when it approved the obligation — the payment is measured **individually, at its own value**, and no escalation is required. Where either limb fails, or the disbursement appears to divide an obligation after the fact or to have been shaped to clear a limit, the signer measures against the **total obligation** and escalates to the RAC before execution, whichever body issued the request. A signer genuinely uncertain which applies escalates rather than deciding at the point of signing: the question is one of characterisation, not of signing discretion.

**Authorization is per-disbursement.** Where one proposal authorised several disbursements under DAO Parameters §6.1A, the signers verify each against §8.2A **separately** at the time it is presented. Approval of a schedule is not approval of any payment within it independently of its verification event, an unexecuted authorization does not transfer to another milestone, and the signers may not net one milestone's unused headroom against another's shortfall.

**Refusal is mandatory, not discretionary.** A signer who determines that a requested disbursement would breach a limit in DAO Parameters §6.1 **must** refuse execution, must report the refusal to the RAC **immediately**, and must record it under §12. This refusal is not an exercise of the discretion in §9: the grounds in §9 are permissive, this one is compulsory, and the clarification cycle cap and invalid-refusal consequence in §9 do not apply to it. A refusal under this section is never selective obstruction under §9A, and never a breach of duty under §18, provided the determination is documented.

Where the breach arises from the **timing** of an otherwise valid disbursement rather than its amount — a payment that clears the outflow cap only because of unrelated disbursements already in the window — the signers notify the requesting party and the RAC of the earliest date on which the disbursement can be executed within the cap, and execute it on that date without a further authorisation. The pre-execution holds in DAO Parameters §9 run from result publication and are not restarted by such a deferral.

---

### 8.2A Executing a Large Milestone Authorization

A disbursement exceeding the Single Transaction Limit may be executed only where the signers verify each of the following — conditions 1 to 4 and 6 giving effect to **DAO Parameters §6.1A**, and condition 5 to **Contributor Compensation Policy §6.4**:

1. the authorising Treasury & Budget proposal expressly invokes §6.1A and states the amount, the recipient, and the obligation discharged — an authorisation may not be inferred from a general budget approval, nor left to any other body to fix later;
2. the RAC's published result records approval at or above the **Large Milestone Approval Threshold**;
3. the verification event stated in the proposal has occurred — for a milestone, Steward sign-off under Contributor Compensation Policy §7;
4. the **High-Risk Signing Threshold** is met and the **High-Risk Execution Delay** has elapsed, regardless of how the transaction would otherwise be classified;
5. the scope of work confirmed under Contributor Compensation Policy §6.4 does not condition the payment on an authorization not yet given, or, where it does, that condition is satisfied; and
6. the disbursement, counted in full and **valued at execution**, does not carry the trailing 30-day total past the **Rolling 30-Day Outflow Cap** — or, where the same proposal granted a one-time uplift under DAO Parameters §6.1B, past the uplifted figure, applied only within that uplift's window.

Any condition unsatisfied is a mandatory refusal under §8.2. Where one proposal authorised several disbursements, these conditions are verified **separately for each**, at the time it is presented. The signers record the verification of each condition under §12.

---

## 9. Refusal or Delay

Treasury Signers may refuse or delay execution only when:

* the request is outside approved authority
* the request conflicts with a passed proposal
* required documentation is incomplete
* there is a credible security, legal, or custody risk
* execution would violate applicable law or contractual obligations

Any refusal or delay must be documented and reported.

**This list is permissive; §8.2 is mandatory.** A disbursement that would breach a budget limit in DAO Parameters §6.1 is refused under **§8.2**, which obliges refusal, not under this section, which permits it. The clarification cycle cap and the invalid-refusal consequence below apply only to refusals grounded in this section.

**Clarification cycle cap:** A signer may request clarification once per proposal. After the requesting party provides a clarification — or after 2 business days without the signer providing a further specific written objection — the signer must proceed to execution or formally escalate to RAC under the dispute procedure (DAO Parameters §6C). No second ambiguity claim may be filed on the same proposal by the same signer.

**Invalid refusal consequence:** If RAC finds a signer's stated refusal grounds to be invalid (not among the enumerated permissible reasons in this section), the proposal advances to the remaining signers immediately without restarting the execution window. The refusing signer's refusal is recorded as a breach of duty and reported in the next governance transparency report.

---

## 9A. Selective Obstruction

A documented pattern of delaying or refusing process verification, or selectively enforcing governance rules without documented grounds on record, constitutes misconduct independent of the inactivity clause (DAO Parameters §6B). RAC members may flag this pattern in Treasury Signers; community members may trigger a misconduct review via Governance Process proposal. This provision is enforced under the **Code of Conduct §6** (see also the parallel provision at RAC Mandate §11A).

---

## 10. Multi-Signature Operation

All treasury and legal execution requiring signer authority must occur through approved multi-signature procedures.

No signer may act unilaterally where multi-signature approval is required.

Meeting a signing threshold does not by itself authorise a disbursement: every treasury action is additionally subject to verification against the budget limits in **DAO Parameters §6.1** under §8.2, and a disbursement exceeding the Single Transaction Limit requires a Large Milestone Authorization verified under §8.2A.

---

## 10A. Custody and Asset Control Standards

### 10A.1 Account Architecture

Treasury assets are held in the multi-signature account whose identifier is recorded in the **On-Chain Identifiers & Verification Policy §5** (the operational register referenced by **Operating Agreement §11.4 / Schedule 4**). That account also holds the **Master Badge** and the **Owner Badge**, so that the badges are under the RAC's collective control rather than any person's; their exercise is governed by **On-Chain Identifiers & Verification Policy §4** and not by the treasury thresholds below, and §3 places them outside the ordinary signing mandate. The signing threshold structure is defined in **DAO Parameters §6A** and is phase-dependent: during the Transition Period **2-of-3** for ordinary transition treasury actions and, for protected matters / high-sensitivity actions, **unanimity of all seated signers, being not fewer than two** (3-of-3 at full strength), consistent with **Operating Agreement §9.11**; from the Activation Date **3-of-5** standard and **4-of-5** high-risk under the five Delegates then holding Treasury Signing. Those five seats are **allocated seats**, held by seated RAC members under RAC allocation, and **elected seats**, whose holders need not hold a RAC seat; the default number of elected seats is zero, and the composition is governed by **Delegate Mandate §3.1–§3.2**. These Rules apply identically to both, and nothing in them turns on how a signer was seated except where expressly stated. High-risk transactions correspond to the **protected matters** in **Operating Agreement §9.12**.

**Establishing and changing the account architecture is phase-dependent.** During the Transition Period, the Transition RAC may establish and adjust the treasury account architecture — the number of accounts, segmentation into operational, reserve, and grants pools, the custody arrangement, and the initial signer set — by Transition RAC resolution published to the Official Venue, as part of its mandate to establish the treasury, custody and signer framework (**Operating Agreement §6.5(d)**). This build-time flexibility is bounded: each account must remain under multi-signature control at the Transition-Period thresholds (**Operating Agreement §9.11**), and any change to signer controls or thresholds, or any movement of material treasury assets, is a protected matter requiring unanimous signing of all seated signers (**Operating Agreement §9.12**). From the Activation Date, the established architecture may be changed only by Governance Proposal, each account remaining under multi-signature control on the same threshold structure.

**An emergency amendment does not open this.** A temporary amendment under **Charter §12.2** confers no authority to change the signer set or its thresholds before it is ratified (**Charter §12.2 item 6**; **Emergency & Safeguards Policy §10**): a signer roster is on-chain state, and restoring it after a failed ratification would need the cooperation of whoever holds the keys by then. Urgent coverage is provided instead by interim appointment from the Emergency Signer Reserve under **Governance Continuity Framework §4.2**, which operates within these rules and requires no amendment.

Once the Transition RAC publishes the Activation Statement (**Operating Agreement §8.5**), the account architecture is treated as settled and must not be changed before the Activation Date except to remedy a security incident, so that the community's Activation Vote is cast on the treasury structure it has reviewed. The established architecture is documented in the **On-Chain Identifiers & Verification Policy §5** and forms part of the treasury and custody framework evidencing **Operating Agreement Schedule 5, condition 4**, so that the Permanent RAC inherits a structure changeable only by community vote.

Account segmentation and any later change must be recorded with the Registered Agent and reflected in the register held under the **On-Chain Identifiers & Verification Policy §5** (per Operating Agreement §11.4 / Schedule 4).

### 10A.2 Annual Treasury Audit

The Company shall undergo an annual independent treasury audit as defined in **DAO Parameters §6.2**. The Permanent RAC is responsible for defining audit scope, selecting the auditor by Governance Proposal, and ensuring the auditor has access to sufficient treasury records and on-chain transaction history (see **RAC Mandate §12**).

### 10A.3 Custody Provider Selection

Where the multisig is operated through a third-party custody platform or service, selection and changes to the provider require Governance Proposal approval. The Treasury Signers may evaluate providers and bring recommendations to governance, but may not unilaterally change the custody provider.

### 10A.4 Key Management Standards

Treasury Signers must maintain:

* Hardware-backed key storage where technically feasible
* Documented key generation and backup procedures
* Recovery procedures that do not introduce single points of failure
* Logged participation in key rotation reviews (every 6 months per DAO Parameters §6A)

Specific key management procedures may remain confidential where necessary for operational security, consistent with the **Compliance Operations Policy §3**.

---

## 11. Separation of Duties

Where possible:

* no single signer should control end-to-end execution
* proposal preparation, payment instruction, and transaction approval should be separated
* legal approval and treasury release should be separated for major actions

---

## 12. Recordkeeping

Treasury Signers must maintain records of:

* execution requests
* signed transactions
* approval references
* exceptions or delays
* incidents and escalations
* the **rolling 30-day disbursement total** maintained under §8.2, including the treasury valuation used at each verification and the leg of the Rolling 30-Day Outflow Cap that bound
* each **one-time outflow uplift** applied under §8.2, with its uplifted figure and the opening and closing dates of the window it governed
* each **mandatory refusal** under §8.2, with the limit engaged and the determination relied on
* for each **Large Milestone Authorization** executed under §8.2A, the verification of each of its six conditions

---

## 13. Reporting

Treasury Signers must contribute to:

* routine treasury reporting, which must state the rolling 30-day disbursement total and the headroom remaining under the Rolling 30-Day Outflow Cap
* incident reporting
* emergency disclosures where applicable
* immediate reporting to the RAC of any mandatory refusal under §8.2

Sensitive operational details may remain confidential where necessary for security.

---

## 14. Conflicts of Interest

Treasury Signers are subject to the disclosure and recusal obligations defined in the **Conflict of Interest Policy §2–4**, which is the authoritative source for conflict of interest rules across all role-holders.

In addition, the following execution-specific rule applies: a signer must not approve execution of a payment or agreement that directly benefits them. If such a payment is required by a passed proposal, the signer must recuse themselves from signing, disclose the conflict, and ensure another signer handles the execution.

---

## 15. Availability and Continuity

Treasury Signers must remain reasonably available to support DAO operations.

**Standard availability:**

* The minimum expected responsiveness is **2 business days** during active periods (see DAO Parameters §6A)
* This standard applies to execution requests, RAC communications, and coordination with Working Groups
* Signers may designate "office hours" or a preferred contact window; this does not reduce the 2-business-day response obligation but clarifies expected timing

**Declared unavailability:**

* A signer may declare a period of unavailability of up to **5 consecutive days per calendar month** without triggering the planned absence notice requirement
* Declared unavailability must be communicated to the RAC before the period begins (or as soon as practicable)
* Declared unavailability periods are excluded from inactivity counting (see DAO Parameters §6B)
* This provision exists to allow signers to take leave, travel, or disconnect without administrative burden, provided it does not occur during an active emergency or time-critical execution window

**Planned absence or resignation:**

* Signers must provide a minimum of **14 days' notice** to the RAC and Governance & Legal Working Group before any planned extended absence (>7 days) or resignation
* Notice must include expected duration and confirmation of secure key custody arrangements during the absence

**Unplanned unavailability:**

* If a signer becomes unexpectedly unavailable (illness, emergency, loss of contact), they or a designated contact must notify the RAC within **48 hours** where possible

**Continuity threshold:**

* If the number of available signers falls below the standard signing threshold for the current phase — fewer than **2** during the Transition Period (2-of-3 set) or fewer than **3** post-activation (3-of-5 set) — the Governance Continuity Framework is automatically triggered (§4.2 post-activation; §4.6 during the Transition Period), including interim appointment procedures and elevated signing thresholds

**Emergency Signer Reserve:**

* The Governance & Legal Working Group maintains an Emergency Signer Reserve — a pre-approved list of eligible candidates who may serve as interim signers
* **A Reserve appointment is one of the two exceptions to the seated-RAC-member requirement**, the other being the holder of an elected seat (Delegate Mandate §3.1). An allocated seat is held only by a seated RAC member; a Reserve member appointed as an interim signer under the Governance Continuity Framework §4.2 need **not** hold a RAC seat, and holds signing authority only for the interim period stated there — a maximum of 30 days, or until a formal replacement is seated, whichever comes first. Reserve members remain subject to KYC before assuming the function (Operating Agreement §10.4) and to these Rules in full while appointed
* Reserve membership is approved by DAO vote at least annually. **The founding Permanent RAC election constitutes the Reserve** for the Reserve List Validity Period, for candidates who declared willingness and completed KYC (Elections & Role Governance Policy §17.4). A Reserve so constituted lapses on expiry of that period, after which this paragraph governs; the two routes are cumulative while both run
* Reserve members are not active signers and hold no signing authority until formally appointed under the Governance Continuity Framework §4.2
* When the RAC cannot meet quorum, appointment from the Reserve may be made by the Tier 1 or Tier 2 fallback authority defined in the Governance Continuity Framework §4.1; the appointment becomes effective 24 hours after public disclosure on the governance forum

---

## 16. Security Requirements

Treasury Signers must:

* use secure devices and authentication methods
* follow custody and key-management procedures
* report suspected compromise immediately
* participate in key rotation or access changes when required

---

## 17. Emergency Actions

In emergencies, Treasury Signers may execute urgent protective actions only when:

* properly triggered under the Emergency & Safeguards Policy
* required thresholds are met
* actions are limited to the minimum necessary response

---

## 18. Breach of Duty

Failure to comply with these rules may result in:

* suspension
* removal
* loss of signer eligibility
* additional governance review
* legal escalation where applicable

---

## 19. Relationship to Other Documents

These rules operate alongside:

* Operating Agreement (Articles V, VII, IX)
* Charter
* Compliance Operations Policy
* Execution & Treasury Actions Policy
* Emergency & Safeguards Policy
* DAO Parameters Registry

If a conflict arises, the Operating Agreement prevails, followed by the Charter, then approved governance decisions (see Operating Agreement §11.3).

These rules are governed by the laws of the Republic of the Marshall Islands (Operating Agreement §14.1). Disputes arising under these rules are subject to the dispute resolution procedure in Operating Agreement Article XIV (and the Dispute Resolution & Arbitration Policy as its Tier 1 process).

---

## 19A. Indemnification

Treasury Signers acting in good faith within their authorized mandate are indemnified by the Company in accordance with Operating Agreement §12.5. The Company shall advance reasonable legal expenses to any Treasury Signer facing claims arising from their role, subject to the conditions and exclusions stated in Operating Agreement §12.5. Treasury Signers are encouraged to review §12.5 of the Operating Agreement directly for the full scope of protections and exclusions.

---

## 20. Amendments

_Amendment procedures and classification requirements are defined in the **Governance Maintenance & Upgrade Framework**._
