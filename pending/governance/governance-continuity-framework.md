# Governance Continuity Framework

| Field | Value |
|---|---|
| **Version** | v1.0.0 |
| **Last updated** | 2026-08-25 |

---

## 1. Purpose

This framework defines how the DAO maintains or restores governance capability when governance bodies fail, when execution becomes blocked, or when normal processes cannot function. The continuity mechanisms here are designed to be activated only when standard governance procedures are insufficient, and to surrender authority back to standard processes as soon as recovery is complete.

---

## 2. Guiding Principle

> Governance must remain recoverable under all circumstances.

---

## 3. Scope

This framework applies to failures affecting:

* The Accountability Council (RAC)
* Treasury Signers
* The Governance Operator and the Owner Badge (operator failure or badge compromise)
* The Legal Signatory, the Compliance Liaison, and the Web2 Custodian (Delegate failure or loss of control of the Web2 estate)
* Working Groups
* Governance participation (sustained quorum failure)
* The governance interface itself (interface unavailability)

It governs the procedures by which interim authority may be exercised during such failures and the conditions under which standard governance authority is restored.

---

## 4. Failure Scenarios

---

### 4.1 RAC Failure

Trigger:

* full resignation, inactivity, or inability to function

**Response — Tier 1 (surviving RAC members):**

If the RAC cannot meet quorum due to deaths or incapacitations, any single surviving RAC member may take the following specific activation actions:

* Declare a RAC continuity event on the governance forum
* Declare a signer continuity event if applicable (see §4.2)
* Appoint interim signers from the Emergency Signer Reserve (Treasury Signers Rules §15)

Tier 1 scope is strictly limited to these triggering and appointment actions. Appointment of an interim Legal Signatory is explicitly excluded — that function is covered by Delegate Mandate §5 (the Compliance Liaison is authorised to act as interim Legal Signatory for protective or time-critical purposes). All Tier 1 actions must be publicly disclosed on the governance forum immediately. Interim signer appointments take effect 24 hours after disclosure to allow a community challenge, except where treasury assets are at immediate risk. All Tier 1 actions are subject to GP ratification within 30 days.

**Response — Tier 2 (no RAC members available):**

If no RAC members are available, the Governance & Legal Working Group Stewards (internal majority vote) may:

* Declare a RAC continuity event on the governance forum
* Appoint interim signers from the Emergency Signer Reserve
* Initiate the emergency election process

Tier 2 authority is granted by this policy and is to be incorporated into the Governance & Legal Working Group Charter when that charter is adopted. Working Group Stewards may not appoint themselves as interim signers or RAC members. All Tier 2 actions require immediate public disclosure and a 24-hour challenge window before taking effect. All Tier 2 actions are subject to GP ratification within 30 days.

**Response — Tier 3 (Governance Participants):**

If neither Tier 1 nor Tier 2 can be activated, authority reverts to Governance Participants per Charter §9. An emergency election may be initiated by any Governance Participant via the standard governance forum process.

**Tier 3 during the Advisory Governance Period (pre-Activation):** Before the Activation Date, community governance outcomes are advisory (OA §5.8) and Tier 3 cannot restart binding governance or alter the signer set (signer-control changes are protected matters — OA §§9.11–9.12). Tier 3 action during this period therefore takes the form of an **escalation-and-freeze protocol**:

1. Any Governance Participant may initiate an advisory vote declaring the continuity event and stating the community's requested response; a recognised advisory outcome (DAO Parameters §3A.3) constitutes the community's formal position on the event.
2. Notice of the event and the advisory outcome must be delivered to the **Registered Agent** and — where the principal asset transfer is pending or in progress — to the **Founding Transferor / Asset Transferor**, with a request to pause any in-flight transfer steps until continuity is restored.
3. Where a **Legal Signatory** or **Compliance Liaison** remains in office, that Delegate must engage DAO-authorized legal counsel on the Company's standing and options (Compliance Operations Policy §5; Delegate Mandate §5) and report to the Official Venue.
4. No emergency amendment, signer change, or asset movement may be undertaken under Tier 3 authority during the Advisory Governance Period. The protocol's purpose is to freeze exposure and obtain legal continuity advice, not to reconstitute governance.

The scenario in which no Transition RAC member survives is only partially addressed at the Operating Agreement level: **OA §6.11(e)** permits the Registered Agent to publish notice of the vacancies on the Company's behalf, and the community may identify replacement members by advisory outcome at the elevated recognition threshold (**OA §6.11(b)**), but the seating steps in **OA §6.11(c)** require a written resolution of seated members and therefore cannot complete while no member remains. That residual risk is deliberately assumed by the Transition RAC as a matter of constitutional design; this protocol preserves the community's position pending resolution and confers no authority the Operating Agreement does not recognise.

In all cases:

* Emergency election for permanent RAC replacement must begin within 7 days of the continuity event (DAO Parameters §6B)
* Election must complete within 21 days of the continuity event (DAO Parameters §6B)
* The Governance Reconstitution Limit (DAO Parameters §6) is available upon declaration of a RAC continuity event

---

### 4.2 Signer Failure

> **Phase scope.** This section governs the **post-activation** signer set (5 signers; 3-of-5 standard, 4-of-5 elevated). During the **Transition Period** the signers are the **3 Transition RAC members** (2-of-3 standard; protected matters require unanimity of all seated signers, being not fewer than two — OA §9.11); their continuity is governed by **§4.6**, which applies the mechanics below with the transition thresholds substituted (trigger: fewer than 2 of 3 available; elevation to 4-of-5 is impossible with three signers, so protected matters pause only while fewer than two seated signers remain, pending seat replacement under OA §6.11).

Trigger:

* active Treasury Signers fall below execution quorum (post-activation: fewer than 3 of 5 available; Transition-Period equivalent in §4.6)
* key compromise confirmed by any signer or the RAC
* refusal to execute a valid approved action without documented grounds (per Treasury Signers Rules §9)

Response:

**Immediate (within 24 hours):**

* RAC declares a signer continuity event and notifies the governance forum. If the RAC cannot meet quorum, the Tier 1 or Tier 2 fallback authority defined in §4.1 satisfies this declaration requirement.
* All non-urgent treasury execution is suspended until quorum is restored
* Emergency actions under the Emergency & Safeguards Policy remain available if required thresholds can be met with available signers

**Forced-execution backstop:** If a passed proposal has not been executed within 10 business days from the close of the Compliance Challenge Window (DAO Parameters §4), and no valid refusal is currently on record with the RAC (i.e., the RAC has not acknowledged a legitimate hold under Treasury Signers Rules §9), the RAC may instruct the remaining available signers to proceed with execution using the minimum 3-of-5 threshold, bypassing the unresponsive or non-compliant signer. This instruction must be published publicly on the governance forum within 24 hours of being issued and is treated as a signer continuity event for reporting purposes. The 10-business-day clock runs from Compliance Challenge Window close, not from proposal passage.

**Interim signer appointment (if active signers < 3):**

* The RAC may appoint up to 2 interim signers from the pre-approved Emergency Signer Reserve (maintained by the Governance & Legal Working Group and approved by DAO vote at least annually, or constituted by the founding Permanent RAC election for the Reserve List Validity Period — Treasury Signers Rules §15; Elections & Role Governance Policy §17.4). An interim signer appointed from the Reserve **need not hold a RAC seat**, and is one of the two exceptions to the rule in Delegate Mandate §3 that an allocated Treasury Signing seat is held only by seated RAC members — the other being the holder of an elected seat (Delegate Mandate §3.1). This is what makes the Reserve usable at minimum RAC strength, where every seated member may already hold Treasury Signing and the body has no spare capacity to re-allocate to
* Interim signers are subject to the full Treasury Signers Rules
* The signing threshold for interim-period actions is raised to **4-of-5** (regardless of whether interim or permanent signers hold the seats)
* Interim appointment must be disclosed to the governance forum within **24 hours** of appointment
* Interim appointment is valid for a maximum of **30 days** or until a formal replacement election is complete, whichever comes first

**Formal replacement:**

* Emergency election for permanent replacement(s) must begin within **7 days** of the continuity event (DAO Parameters §6B)
* Election must complete within **21 days** of the continuity event (DAO Parameters §6B)
* Upon election of permanent replacements, interim appointments are immediately void

**Key compromise:**

* Compromised keys must be rotated and the affected signer suspended pending review
* If compromise affects treasury access, the RAC invokes the Emergency & Safeguards Policy to secure assets

---

### 4.2A Governance Operator Failure

The proposal pipeline depends on the Governance Operator elevating eligible Temperature Checks via the Owner Badge (Proposal & Voting Framework §3.3; Delegate Mandate §2.2). Because the removal of a non-compliant Governance Operator itself requires a proposal to pass through that pipeline, operator failure is a continuity event with its own backstop, parallel to the signer forced-execution backstop in §4.2.

> **Scope limit — read this before relying on the backstop.** The response below is written for a configuration in which the Governance Operator, the instructing RAC, and the executing Treasury Signers are **different people**. Under **Delegate Mandate §3** Delegated Functions are allocated from among seated RAC members, and during the Transition Period all functions are held by the three-member Transition RAC (**Delegate Mandate §6**). In both phases, therefore, the three actors below may be — and at minimum RAC strength will be — the same people, and this backstop has no independent party in it. That is a **known and accepted consequence** of the DAO's scale, not an oversight. What survives in that configuration is the published record: the instruction, the compliance window, and the disclosure duties below all still apply and are all public, so a failure is visible even where it cannot be externally compelled. The backstop recovers its full force only where the DAO has switched Governance Operations or Treasury Signing to election under Delegate Mandate §3, or where an interim signer from the Emergency Signer Reserve is serving (§4.2).

Trigger:

* an eligible passed Temperature Check remains unelevated beyond the TC Elevation Window (DAO Parameters §3.1) with no documented grounds on record with the RAC
* the Governance Operator is unavailable, unresponsive, or refuses to perform an elevation or governance-parameter update required by a valid governance outcome
* compromise of the Master Badge, the Owner Badge, or the Governance Operator's keys is confirmed or credibly suspected

Response:

**Elevation backstop:**

* The RAC may formally instruct the Governance Operator to perform the elevation. The instruction must be published to the governance forum within 24 hours of being issued.
* If the Governance Operator does not comply within the Elevation Backstop Compliance Window (DAO Parameters §3.1), or is unavailable or compromised, the elevation is executed through the Owner Badge recovery or custody arrangement established for the Governance smart contract, by the Treasury Signers at the standard signing threshold for the current phase (DAO Parameters §6A). Where that arrangement operates by reissuing the Owner Badge, the exercise of the Master Badge required to do so is authorised by this section and by that threshold alone — this is the one route by which the Master Badge is exercised without the higher authority otherwise required for it (On-Chain Identifiers & Verification Policy §4), because a backstop that required unanimity could not fire in the circumstances that trigger it.
* A backstop elevation is treated as a continuity event for reporting purposes and must be disclosed to the governance forum within 24 hours of execution.
* Non-compliance with a valid RAC elevation instruction without documented grounds is a breach of duty and grounds for immediate suspension under the Elections & Role Governance Policy §10.3 and removal under §10.

**Badge compromise:**

* A confirmed or credibly suspected compromise of the Owner Badge or the Governance Operator's keys is handled as a key-compromise continuity event: the badge must be rotated or reclaimed through the recovery arrangement, the affected Delegate suspended pending review, and the incident disclosed and reviewed per the Emergency & Safeguards Policy.
* **Compromise of the Master Badge is a different and graver event, and rotation does not answer it.** An attacker holding the Master Badge can re-mint, recall, or invalidate any Owner Badge issued to replace one it has taken, so reissuing the Owner Badge recovers nothing while the Master Badge remains compromised. The response is redeployment: the governance component and its badges must be redeployed and the new identifiers recorded as a Governance-critical change (On-Chain Identifiers & Verification Policy §8), with the compromised identifiers marked superseded in the register so that no verification link resolves to an instrument still under an attacker's control. Until redeployment completes, no elevation may be treated as authoritative.

**Deployment requirement:**

* The custody and recovery arrangement for the Owner Badge is an implementation decision made when the Governance smart contract is deployed, and is recorded in the On-Chain Identifiers & Verification Policy §3 (per Operating Agreement §11.4 / Schedule 4). Whatever arrangement is chosen, it must provide a mechanism by which an elevation or badge rotation can proceed without the Governance Operator's cooperation, sufficient to give effect to this section. A deployment lacking this capability does not satisfy the Minimum Operational State in §7.
* The custody arrangement for the **Master Badge** is recorded in the same register and is subject to the same test, with one addition: it must not be exercisable by any single person (On-Chain Identifiers & Verification Policy §4). A deployment in which one person can mint, recall, or invalidate the Owner Badge alone does not satisfy the Minimum Operational State, whatever the Owner Badge's own custody arrangement provides — the weaker of the two arrangements is the one that governs in practice.

---

### 4.2B Legal Signatory, Compliance Liaison, or Web2 Custodian Failure

Each of these functions is held by one Delegate (Delegate Mandate §3) and has no threshold mechanism by which the holder can be routed around.

Trigger:

* the holder is unavailable, unresponsive, or unable to act for longer than the Max Unexcused Inactivity Period (DAO Parameters §6A), or for more than 24 hours where a time-critical filing, regulatory response, or legal action is required
* the holder refuses to perform an act required by a valid governance outcome
* the function is unheld and the RAC cannot re-allocate it from among its seated members
* for the Web2 Custodian: loss of, or loss of control over, any credential store, domain registrar account, or platform account holding a Company Web2 asset

Response:

* **Interim cover.** The substitutions in Delegate Mandate §5 apply — the Compliance Liaison acts as interim Legal Signatory, the Legal Signatory as interim Compliance Liaison, in each case for protective or time-critical purposes only, with disclosure within 24 hours and Governance Proposal ratification within 30 days. Where neither is available, or both are the subject of the matter, the RAC acts directly with the Registered Agent (Delegate Mandate §2.4).
* **Web2 recovery.** The RAC invokes the recovery arrangement under Delegate Mandate §2.5 and Compliance Operations Policy §4, appoints an interim holder, and discloses the invocation to the Official Venue within 24 hours. Recovery must be exercisable without the Custodian's cooperation; where it is not, the Minimum Operational State in §7 is not satisfied and the failure is reported as such.
* **Restoration.** The RAC re-allocates the function under Delegate Mandate §3, or where it cannot, converts it to an elected seat under Delegate Mandate §3.3. Interim authority ends on the seating of a holder.
* **Refusal or compromise.** Refusal to perform an act required by a valid governance outcome, without documented grounds on record with the RAC, is a breach of duty and grounds for immediate suspension under the Elections & Role Governance Policy §10.3 and removal under §10. Credential compromise is handled as a key-compromise continuity event and reviewed per the Emergency & Safeguards Policy.

---

### 4.3 Governance Inactivity

Trigger:

* 3 consecutive quorum failures on the **same proposal** — the same substantive proposal, resubmitted after each failed attempt (as defined in DAO Parameters §9A). The trigger is per-proposal: unrelated failures within a category do not place other proposals of that type into reduced-quorum mode

Response:

* extended voting periods (double standard duration)
* reduced quorum threshold (50% of standard quorum, minimum 1%) — except that the quorum for Constitutional proposals may not be reduced below the entrenched 7% floor (Charter §12.1 item 2), so the effective reduced Constitutional quorum is 7%
* a raised approval threshold for any proposal confirmed under the reduced quorum (Reduced-Quorum Approval Uplift, DAO Parameters §9A: +15 percentage points above the standard threshold — Governance Process 60% → 75%, Executable 50% → 65%; Constitutional unchanged)
* a reduced-quorum activation notice, published by the RAC to the Official Venue at the opening of the reduced-quorum voting window, before the extended voting period runs

The reduced quorum applies once. A proposal that fails to meet it has failed and is subject to the standard cooldown (DAO Parameters §3.4); the quorum is not further reduced.

The fallback preserves the DAO's decision-making capability during periods of low engagement without abandoning the quorum principle entirely. Thresholds are defined in the **DAO Parameters Registry §9A**.

Treasury / Budget proposals and **election proposals** are excluded from this fallback, under **both** election mechanisms. Each mechanism carries its own low-turnout handling, and the two differ (DAO Parameters §9A):

* **Two-stage** — the Stage 2 quorum-held-over rerun in the Elections & Role Governance Policy §7.3: a reduced rerun quorum paired with a raised approval threshold, over an extended voting period
* **Majority Judgment** — a single rerun at the **unchanged** quorum and the **unchanged** electability floor over a doubled voting period (Elections & Role Governance Policy §7A.3). This is the one mechanism in the framework whose low-turnout handling does not reduce a quorum, because it has no share-of-votes threshold that could be raised to compensate

---

### 4.4 Working Group Failure

A Working Group is treated as failed when it has become inactive or has demonstrated an inability to execute against its mandate — for example, by missing two consecutive reporting cycles, exhausting its budget without delivery, or becoming non-responsive to RAC inquiries. On a finding of Working Group failure, the RAC may initiate a Governance Proposal to restructure the body, replace its Stewards by emergency election, or dissolve it under the Working Group Framework §4. Active contributor engagements and unspent budget funds are handled per the Working Group Framework and the Contributor Onboarding and Offboarding Policy §7.

---

### 4.5 Governance Interface Unavailability

Trigger:

* The primary governance voting interface is inaccessible or non-functional for more than **48 continuous hours**

Response:

**Active votes in progress:**

* All active voting periods are automatically extended by the duration of the outage plus a **48-hour buffer** upon restoration
* The RAC must announce the extension via the governance forum within 12 hours of confirming the outage

**New proposals:**

* No new proposals may enter the voting phase until the primary interface is restored or an alternative interface is confirmed
* Draft and review periods may continue

**Compliance Challenge filing is unaffected:**

* Compliance Challenge filing does not depend on the governance interface. Filings are made to the Compliance Challenge Filing Channel or by publication to the Official Venue under **Proposal & Voting Framework §8.4**, either of which is independently valid
* An interface outage therefore does not extend, suspend, or toll a Compliance Challenge Window. Where a result has been published and its window is running, the window runs to its close on the ordinary timetable

**If outage exceeds 7 days:**

* The RAC may invoke the Emergency & Safeguards Policy if time-sensitive matters (e.g., expiring treasury actions, security incidents) cannot wait for restoration
* The RAC must propose and confirm an alternative voting mechanism via public announcement to the governance forum; the alternative must be:
  * Publicly auditable
  * Accessible to all Governance Participants
  * Recorded on-chain or in a tamper-evident off-chain record

**Restoration:**

* Upon restoration of the primary interface, the RAC must publish a brief incident report (cause, duration, actions taken) within 48 hours
* Any alternative voting results must be migrated or acknowledged in the primary interface record

---

### 4.6 Transition RAC Vacancy (Pre-Activation)

The RAC-failure response in §4.1 presumes a **seated body that reconstitutes through an emergency election under the Elections & Role Governance Policy**. The **Transition RAC** is different: its three seats carry the community's pre-existing founding mandate and are fixed in the Operating Agreement (OA §6.3, Schedule 1), and are **not** elected under the Elections Policy. A Transition RAC seat that vacates before the Activation Date (death, incapacity, or resignation under the Floor-Protected Resignation rule, Elections Policy §11.2) is instead replaced through the vacancy mechanism in **Operating Agreement §6.11**.

**Operational response (within Operating Agreement authority):**

* The surviving Transition RAC members continue to act. Ordinary formation decisions remain valid under the **simple-majority-of-seated** decision rule in **Operating Agreement §6.6**, which already operates on seated members and is unaffected by a seat falling vacant.
* The remaining seated members must, by unanimous written resolution, **declare the seat vacant and publish notice to the Official Venue** (OA §6.11(a)), and must declare a continuity event under this framework. The body must treat restoration of full strength as a priority transition task under its mandate (OA §6.5(g)); a sub-strength state may not be treated as permanent or as a basis to defer the Activation Date (OA §8.3).
* A replacement member is identified by a **recognised community advisory outcome at the elevated Entrenched-Provision recognition threshold** (OA §6.11(b), §12.2(c)(ii); DAO Parameters §3A.3), and is seated only after satisfying onboarding, compliance, KYC, and acceptance requirements and being recorded in Schedule 1 by written resolution of the then-seated members (OA §6.11(c)). Membership and all signer and signatory rights commence only upon completion of those steps (OA §6.11(d)).
* Where the vacancy also reduces active Treasury Signers below the 2-of-3 execution quorum, the **signer-failure** response in §4.2 applies in addition (with transition thresholds substituted per the phase-scope note in §4.2).

**Limits — matters reserved to the Operating Agreement:**

* **Seat replacement authority.** Admitting a new member to the Transition RAC (a change to the persons fixed in OA §6.3 / Schedule 1) remains a formation matter governed exclusively by **OA §6.11**. This framework coordinates the operational response but cannot itself add or substitute a Transition RAC member; the community advisory outcome under OA §6.11(b) *identifies* the replacement — seating occurs only through the OA §6.11(c) steps.
* **Critical-floor interaction.** The Entrenched-Provision amendment threshold and the Schedule 5 condition-waiver require the unanimous affirmative vote of all seated Transition RAC members, **being not fewer than two** (Operating Agreement §12.2(c)(i); DAO Parameters §3A.4), together with a concurrent recognised advisory outcome at the elevated threshold. Protected-matter signing likewise requires unanimity of all seated signers, **being not fewer than two** (Operating Agreement §§9.11–9.12). A single vacancy therefore suspends neither path: both continue at 2-of-2 among the remaining seated members pending replacement under OA §6.11, and the formal route to activate where the Permanent RAC election cannot seat the minimum (Elections Policy §17.1–§17.3) survives attrition. Only if seated membership falls below **two** do Entrenched-Provision amendments, Schedule 5 waivers, and protected-matter execution pause, until a replacement is seated under OA §6.11. Where **no** seated member remains, OA §6.11(e) provides the Registered Agent notice route, subject to the residual seating limits described in §4.1 (Tier 3).

---

## 5. Emergency Recovery Actions

In critical failure scenarios, the Emergency & Safeguards Policy may be invoked alongside this framework. The RAC may take temporary stabilizing actions within its defined limits — for example, suspending non-essential treasury execution or pausing a malfunctioning Working Group — while continuity procedures complete. The DAO retains final authority over all such actions, which remain subject to GP ratification within 30 days unless the Emergency & Safeguards Policy specifies otherwise.

---

## 6. Reconstitution

After any continuity event, the affected roles must be re-established through standard governance within the Reconstitution Deadline defined in DAO Parameters §9A (currently 30 days). Authority must return to standard processes as soon as the relevant election or replacement completes. All temporary measures — interim signer appointments, elevated signing thresholds, fallback voting mechanisms — must be unwound once reconstitution is complete.

---

## 7. Minimum Operational State

The DAO is considered operational when proposals can be submitted and voted on through the governance interface, signers can execute approved actions, every Delegated Function is held (Delegate Mandate §3), the Owner Badge and Master Badge arrangements satisfy §4.2A, the Web2 recovery arrangement satisfies §4.2B, and governance processes (including the RAC's oversight function) are functional. A state in which any of these capabilities is missing is a continuity event triggering the response procedures in §4.

---

## 8. Transparency

All continuity actions must be documented at the time they are taken, publicly reported to the governance forum within the disclosure windows specified in §4, and made subject to DAO review through GP ratification or, where applicable, a retrospective Governance Proposal.

---

## 9. Relationship to Other Documents

This framework operates alongside:

* **Emergency & Safeguards Policy** — emergency response authority and protocol
* **Elections & Role Governance Policy** — emergency elections, vacancy handling, and interim-appointment renewal rules
* **Execution & Treasury Actions Policy** — execution mechanics and forced-execution backstop
* **Treasury Signers Rules §9, §15** — valid refusal grounds and the Emergency Signer Reserve
* **RAC Mandate** — RAC authority limits, including in continuity events
* **Delegate Mandate §2.4, §2.5** — Compliance Liaison subject rule; Web2 recovery independence
* **Delegate Mandate §3, §3.3** — Function coverage and conversion where the RAC cannot allocate
* **Delegate Mandate §5** — Legal Signatory, Compliance Liaison, and Web2 Custodian continuity
* **Compliance Operations Policy §4** — Credential and Web2 asset security, recovery independence
* **Source Code Stewardship Policy §3.2** — Repository access standards
* **Working Group Framework §4** — Working Group dissolution
* **DAO Parameters Registry §6, §6B, §9A** — Governance Reconstitution Limit, replacement timing, and continuity fallback parameters

---

## 10. Amendments

_Amendment procedures and classification requirements are defined in the **Governance Maintenance & Upgrade Framework**._

---

## 11. Guiding Principle

> If governance fails, recovery must be clear, fast, and decentralized.
