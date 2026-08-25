# DAO Parameters Registry

| Field | Value |
|---|---|
| **Version** | v1.0.0 |
| **Last updated** | 2026-08-25 |

---

## 1. Purpose

This document defines the **configurable parameters** governing DAO operations.

These parameters:

* Enable flexibility without modifying core governance documents
* Provide clarity on thresholds, durations, and limits
* May be updated via governance proposals

---

## 2. Scope

This registry defines:

* Voting thresholds
* Quorum requirements
* Time durations
* Budget limits
* Emergency thresholds

---

## 3. Governance Parameters

---

### 3.1 Voting Durations

| Parameter               | Value    | Description                           |
| ----------------------- | -------- | ------------------------------------- |
| Draft Discussion Period | ≥5 days  | Minimum time for community discussion on the RAC-designated platform. Does not apply to Election proposals; see Election Nomination & Discussion Window below. |
| Election Nomination & Discussion Window | 7–10 days | Combined nomination and community discussion period for Election proposals. Nominations open at the start of this window; community discussion runs concurrently. Replaces the separate Draft Discussion and Nomination Period for elections. After this window closes, the Temperature Check opens immediately. |
| Temperature Check Voting Period | 5–7 days | Duration of the TC vote for Constitutional, Governance Process, Treasury/Budget, and Executable proposals |
| Temperature Check Voting Period (Short) | ≥1 day | Duration of the TC vote for Election proposals and multi-option Approval Voting polls |
| DAO Proposal Voting Period | 5–7 days | Duration of the binding DAO Proposal vote |
| TC Elevation Window | 5 business days | Maximum time from the close of a passed Temperature Check to its elevation by the Governance Operator, or to documented grounds for delay being recorded with the RAC. Elapse without either triggers the elevation backstop (Governance Continuity Framework §4.2A) |
| Elevation Backstop Compliance Window | 2 business days | Time for the Governance Operator to comply with a formal RAC elevation instruction before backstop execution proceeds (Governance Continuity Framework §4.2A) |

---

### 3.2 Quorum Requirements

Quorum is measured as a percentage of eligible voting power. Eligible voting power is determined at the voting snapshot and includes all sources listed in §8A — at minimum liquid XRD holdings and LSU holdings converted to their XRD equivalent (the constitutional floor per Charter §12.1 item 4).

| Proposal Type / Vote | Quorum                      |
| -------------------- | --------------------------- |
| Constitutional     | 10% of eligible voting power |
| Governance Process | 7%                     |
| Treasury / Budget  | 7%                     |
| Executable         | 5%                     |
| Temperature Check (TC) | 3%                 |

Quorum is measured as Participation — YES + NO + ABSTAIN — as defined in Proposal & Voting Framework §6.3.

**Election proposals** (Proposal & Voting Framework §4.5) are not listed above. Their quorum is set in **§6B** — Minimum Participation for Elections, and the Election Stage 2 Quorum — which adopts the Governance Process figure of 7%. The Temperature Check row does apply to an Election proposal's Temperature Check, which runs over the shortened period in §3.1.

**Absolute Participation Floor (Treasury / Budget proposals):** In addition to the percentage quorum above, a Treasury / Budget proposal requires a minimum of 50 unique voting addresses. An address counts toward this floor if it cast any vote, including ABSTAIN: the floor measures breadth of participation, not direction of support. Both conditions must be met. This floor is not subject to the Governance Continuity Fallback (§9A).

---

### 3.3 Approval Thresholds

| Proposal Type / Vote | Approval  |
| -------------------- | --------- |
| Constitutional     | ≥ 66% YES |
| Governance Process | ≥ 60% YES |
| Treasury / Budget  | ≥ 50% YES |
| Executable         | ≥ 50% YES |
| Temperature Check (TC) | ≥ 50% YES |

Approval is measured as the YES share of Decisive Votes — YES + NO, excluding ABSTAIN — as defined in Proposal & Voting Framework §6.3.

**Election proposals** (Proposal & Voting Framework §4.5) have no single approval threshold and are not listed above, because neither election mechanism decides on a YES share of the whole vote. Majority Judgment turns on the qualifying grade and the Minimum Qualifying Grade (Proposal & Voting Framework §6.2.4; §6B); the two-stage mechanism ranks by voting power at Stage 1 and applies the Election Stage 2 Approval Threshold per candidate at Stage 2 (§6.2.5; §6B). The Temperature Check row does apply to an Election proposal's Temperature Check.

---

### 3.3A Minimum Affirmative Support

Because ABSTAIN counts toward quorum but not toward approval (Proposal & Voting Framework §6.2.1), a proposal can in principle be carried over its quorum threshold predominantly by ABSTAIN votes and then decided by a very small base of affirmative support. The floor below sets a minimum level of affirmative support that a Standard vote must reach independently of quorum.

| Proposal Type      | Minimum YES (% of eligible voting power) |
| ------------------ | ---------------------------------------- |
| Constitutional     | 3.5% |
| Governance Process | 2%   |
| Treasury / Budget  | 1.5% |
| Executable         | 1%   |

**Measurement.** YES voting power as a percentage of eligible voting power at the voting snapshot (§8A). ABSTAIN and NO volume do not enter this calculation. The floor applies in addition to the quorum (§3.2) and approval (§3.3) tests; all applicable tests must be met for the proposal to pass.

**Scope.** Applies to the Standard vote type only (Proposal & Voting Framework §6.2.1) — Constitutional, Governance Process, Treasury & Budget, and Executable proposals. It is not needed for any other vote type, because the Standard type is the only one offering an ABSTAIN option; where no ABSTAIN option exists, quorum × approval already implies a minimum affirmative share by construction. In particular it does not apply to Temperature Check votes (§6.2.6), Election Stage 2 Confirmation Votes (§6.2.7), Approval Voting (§6.2.2), or Majority Judgment (§6.2.4). Majority Judgment is excluded for a further reason: it produces no YES voting power to measure, and its quorum operates alongside the Grade Quantile (Proposal & Voting Framework §6.2.4) and the Minimum Qualifying Grade (§6B) — a share test inside the count and a threshold on rank, neither of which is a YES share (Proposal & Voting Framework §6.3).

**Derivation.** Each figure is approximately half of the YES share that a zero-ABSTAIN vote clearing its quorum at its approval threshold would produce (e.g. Governance Process: 7% × 60% = 4.2%; floor 2%). ABSTAIN votes may therefore carry at most roughly half of the participation burden. Adjusting that fraction is the intended dial for tuning this section.

**Reduced quorum.** Where the Governance Continuity Fallback (§9A) applies, the floor is halved for that proposal, in step with the reduced quorum. See §9A.

**Not an Entrenched Provision floor.** This section adds a requirement; it does not reduce or weaken any Charter §12.1 Entrenched Provision. The 7% Constitutional quorum floor (Charter §12.1 item 2) is unaffected.

---

### 3.4 Cooldown Periods

| Scenario               | Cooldown    |
| ---------------------- | ----------- |
| Failed Proposal        | 7 days      |
| Minor Fix Resubmission | No cooldown |
| Major Resubmission     | 7 days      |
| Per-Proposer Treasury Submission Limit | 1 Treasury & Budget proposal per rolling 30-day period per wallet address. A second submission within the window requires prior RAC notification and acknowledgement posted to the governance forum before the TC voting period opens. |

---

### 3.5 Multi-Choice Voting Parameters

| Parameter | Value | Description |
| --------- | ----- | ----------- |
| Approval Voting: Maximum Options | 8 | Maximum number of options on the ballot per multi-option Executable proposal (§4.4). Does not apply to election shortlisting; election ballots list all eligible nominees (§6B). |
| Approval Voting: Minimum Winner Threshold | ≥ 30% of total votes cast | Minimum voting power an option must receive to be declared winner. Applies to multi-option Executable proposals (§4.4). Does not apply to election Stage 1 shortlisting; Stage 1 ranks candidates by total voting power only (§6.2.5). |
| Majority Judgment: Grade Scale | Excellent / Very Good / Good / Acceptable / Poor | The five-grade scale for Majority Judgment election votes (§6.2.4). **The order is normative** — Excellent is the highest grade and Poor the lowest, and every qualifying-grade, ranking, and Minimum Qualifying Grade comparison is a comparison of rank on this scale. For implementation the grades carry the fixed indices Excellent = 4, Very Good = 3, Good = 2, Acceptable = 1, Poor = 0; the indices are an encoding of the order, not scores to be averaged. A voter assigns exactly one grade to every candidate, and there is no Abstain grade |
| Result Publication Window | Within 48 hours of vote close | Deadline for RAC to publish the official outcome, quorum calculation, threshold applied, and winner determination; the Compliance Challenge Window (§4) opens upon publication |

---

## 3A. Activation, Ratification & Transition Parameters

These parameters carry the activation and transition mechanics that the **Charter §4A** and the **Operating Agreement** (Article VIII, Schedule 5, §§5.7–5.9, §12.2) defer to the policy framework. They apply during the Advisory Governance Period (formation to the Activation Date).

### 3A.1 Framework Ratification (Activation Condition 6)

| Parameter | Value | Description |
| --------- | ----- | ----------- |
| Ratification Quorum | 10% of eligible voting power | Constitutional-level quorum for the one-time community ratification of the Charter and full policy framework (OA Schedule 5, condition 6) |
| Ratification Approval | ≥ 66% YES | Constitutional-level approval threshold for ratification, measured against Decisive Votes (Proposal & Voting Framework §6.3) |
| Ratification Minimum Affirmative Support | 3.5% of eligible voting power | The Constitutional floor in §3.3A. Ratification is a Standard vote with an ABSTAIN option, so the floor applies |
| Scope | Charter **and** the full policy library | Ratification covers the entire community-written framework, not the Charter alone |
| Timing | **Before formation** | Ratification is taken before the Company exists, on the community's own governance system, and is not an act of the Company or an exercise of authority under the Operating Agreement (Charter §4A.2A). It fixes the version of the framework the founding sequence proceeds on |
| Result determination | Arithmetical, from the record of the system on which the vote was taken | No RAC holds authority to determine this vote when it closes. The thresholds above are applied to the public record and the outcome is published ministerially — see Proposal & Voting Framework §6.5, which governs every other vote but expressly not this one |
| Recognition | Twice: on formation — the Company's ratification and adoption on execution of the Operating Agreement (OA §11.1A) and the Transition RAC resolution (OA Schedule 5, condition 6(a)) — then the Activation Vote | The Activation Vote is the act by which the community adopts the pre-formation ratification within the Company's legal order (Charter §4A.2A; GP-ACTIVATE-1 §2) |

### 3A.2 Activation Vote (sole binding pre-activation vote)

| Parameter | Value | Description |
| --------- | ----- | ----------- |
| Activation Vote Voting Period | 5–7 days | Duration of the binding Activation Vote (OA §8.6) conducted after publication of the Activation Statement |
| Activation Vote Quorum | 10% of eligible voting power | Constitutional-level quorum |
| Activation Vote Approval | ≥ 66% YES | Constitutional-level approval, measured against Decisive Votes (Proposal & Voting Framework §6.3) |
| Activation Vote Minimum Affirmative Support | 3.5% of eligible voting power | The Constitutional floor in §3.3A. The Activation Vote is a Standard vote with an ABSTAIN option, so the floor applies |
| Quorum/Majority Failure | Re-run after the standard failed-proposal cooldown (§3.4) | If the Activation Vote fails to reach quorum or majority, it may be re-initiated after cooldown once the Transition RAC re-confirms the Schedule 5 evidence; the Transition RAC's non-discretionary initiation duty (OA §8.5) continues to apply |

### 3A.3 Advisory-Outcome Recognition Thresholds (OA §5.9)

| Parameter | Value | Description |
| --------- | ----- | ----------- |
| Advisory Recognition — Participation | ≥ 7% of eligible voting power | Participation an advisory outcome must reach to be "recognised", triggering the Transition RAC's acknowledgement/explanation duty (OA §5.9; period set in RAC Mandate) |
| Advisory Recognition — Majority | ≥ 50% YES | Majority required for recognition |
| Advisory Recognition — Entrenched-Provision amendments (higher threshold) | ≥ 10% participation and ≥ 66% YES | The elevated recognition threshold for an advisory outcome supporting a proposed amendment to an Entrenched Provision during the Transition Period (OA §12.2(c)(ii)) |

### 3A.4 Entrenched-Provision Amendment Thresholds

| Phase | Requirements |
| ----- | ------------ |
| During the Transition Period (OA §12.2(c)) | Unanimous affirmative vote of all **seated** Transition RAC members, being **not fewer than two** (OA §12.2(c)(i)), **and** a concurrent recognised advisory outcome meeting the higher threshold in §3A.3 **and** ≥14 days' prior notice to the registered agent and the Official Venue |
| Following the Activation Date (OA §12.2(d)) | Quorum **≥ 20%** of eligible voting power (not less than twice the 10% Constitutional quorum); approval **≥ two-thirds** of all Governance Tokens participating (see note below); where the amendment affects the Permanent RAC's constitutional role, composition, election mechanics, or removal, the prior written consent of the Permanent RAC by **≥ 2/3 of seated members**; and ≥21 days' prior public disclosure to the Official Venue |

**Note — ABSTAIN treatment for post-Activation entrenched amendments.** "All Governance Tokens participating" follows the wording of OA §12.2(d)(ii) and means **Participation**, including ABSTAIN, in the denominator. This is a deliberate divergence from the Decisive Votes rule that governs every other approval threshold (Proposal & Voting Framework §6.3): for a post-Activation Entrenched-Provision amendment, an ABSTAIN vote counts against the two-thirds requirement in the same way a NO vote does. The divergence is intended — it raises the practical bar for amending an Entrenched Provision, which is the purpose of entrenchment. The RAC must apply this denominator, not the §6.3 default, when counting such a vote. The Minimum Affirmative Support floor (§3.3A) is subsumed by the higher requirement here and is not separately applied.

---

### 3A.5 Permanent RAC Election Gating (Activation Condition 7)

| Parameter | Value | Description |
| --------- | ----- | ----------- |
| Minimum Seats for Activation | 5 | Minimum number of Permanent RAC members that must be duly elected and **formally seated** before the Activation Vote (OA Schedule 5, condition 7; §5.1) |
| KYC Before Seating | Mandatory | Every elected Permanent RAC member must complete KYC Tier 1 verification (Compliance Operations Policy) **before** being seated, satisfying OA §1.24 "Seated" and the §114(1)(d) natural-person-control requirement |
| Election Initiation Deadline | Within 90 days of framework ratification (Activation Condition 6) | The Transition RAC must open the Permanent RAC election within this fixed window so the election cannot be stalled |
| Seating Deadline | Before publication of the Activation Statement | Elected members must be seated before the Transition RAC publishes the Activation Statement (OA §8.5) |

---

## 4. Compliance Challenge Parameters

*Formerly styled the "veto" (Proposal & Voting Framework §8); the name changed, the mechanism did not.*

| Parameter                  | Value              |
| -------------------------- | ------------------ |
| Compliance Challenge Window | 48 hours from RAC result publication |
| Compliance Challenge Filing Threshold | 0.1% of eligible voting power (all sources per §8A) held by the filer, verified against the most recent governance snapshot. The RAC's review of the challenge grounds (Proposal & Voting Framework §8.4) is the substantive filter; no aggregate participation requirement applies |
| Compliance Challenge Filing Channel | The designated filing addresses recorded in the **On-Chain Identifiers & Verification Policy §3** — the Governance Operator mailbox as primary recipient, with the RAC mailbox in copy, so that a filing does not depend on any single role holder. **Interim measure pending a governance filing interface.** This parameter is defined by reference so the Channel may be migrated to an interface by parameter update, without amending Proposal & Voting Framework §8.4. Publication to the Official Venue is an independently valid filing route at all times (Proposal & Voting Framework §8.4) |
| Channel Publication Window | 6 hours from receipt — the Governance Operator publishes filings received at the Channel verbatim to the Official Venue, with the receipt timestamp (Proposal & Voting Framework §8.4) |
| Holding Proof Cure Period  | 12 hours from RAC notification — period allowed to complete an incomplete holding proof. Runs inside the RAC's 48-hour determination window and does not extend it (Proposal & Voting Framework §8.3A) |
| Optional Stake Requirement | None               |

---

## 5. RAC Parameters

---

### 5.1 RAC Composition

| Parameter                        | Value                                                                  |
| -------------------------------- | ---------------------------------------------------------------------- |
| Transition RAC Members           | Exactly 3 (named in Operating Agreement Schedule 1 (§6.3); constituted under Operating Agreement Article VI) |
| Permanent RAC Members            | Between 5 and 7 (set per election; defined in RAC Mandate §7). Adjustable by Governance Process proposal; minimum 5. |
| Term Length (Permanent RAC)      | 6 months                                                               |
| Routine Decision Quorum          | Simple majority (more than half of seated members), where "seated members" excludes members recused on the matter — see Recusal and Quorum below |
| Routine Decision Approval        | Simple majority YES of non-recused seated members participating        |
| Recusal and Quorum               | A member recused from a matter under **Conflict of Interest Policy §5.1** is excluded from both the quorum denominator and the approval calculation **for that matter only**, in the same way as a vacated seat. A RAC decision may not be taken on a matter where fewer than **3** non-recused members remain (Permanent RAC) or fewer than **2** non-recused members remain (Transition RAC). Where the floor is not met, the matter is escalated under **DAO Parameters §6C** and the RAC publishes a recusal-quorum notice to the Official Venue stating the matter, the number of recusals, and the escalation route. Recusal is recorded in the decision record; it is not an abstention and does not count as a NO |
| Seat Vacancy Definition          | A seat is immediately vacated upon: (a) confirmed death notified by a pre-registered emergency contact; (b) written resignation; or (c) written declaration from a pre-registered emergency contact that the member is medically incapacitated and unable to perform their function. Vacated seats are excluded from quorum calculations immediately upon notification. |
| Emergency Contact Requirement    | Each RAC member must register an emergency contact at appointment and update it at each term renewal. Emergency contacts are held by the Compliance Liaison and the Governance & Legal WG. |

---

### 5.2 RAC Emergency Thresholds

| Parameter                 | Value         |
| ------------------------- | ------------- |
| Quorum                    | ≥ 2/3 members |
| Approval Threshold        | ≥ 75%         |
| Emergency Action Duration | Max 7 days    |

---

## 6. Treasury Parameters

---

### 6.1 Budget Limits

| Parameter                          | Value                |
| ---------------------------------- | -------------------- |
| Working Group Budget Cap           | Defined per proposal |
| Single Transaction Limit           | $12,000 USDC |
| Expense Pre-Authorisation Threshold | $500 USDC — expenses at or above this value require advance approval by the body holding the budget (Contributor Compensation Policy §8). Measured per claim |
| Emergency Spend Limit              | $5,000 USDC — for operational emergencies (asset security, key rotation, critical infrastructure) |
| Governance Reconstitution Limit    | $25,000 USDC — available only when a RAC or signer continuity event has been declared under Governance Continuity §4.1 or §4.2; covers emergency election costs, legal filings, and Registered Agent compliance fees; subject to GP ratification within 30 days |
| Legal Defense Advancement Limit    | $25,000 USDC per legal proceeding — a bridging pool covering immediate legal response costs for one or more Delegates or RAC members named in the same proceeding arising from their role, before a GP can authorize ongoing funding; the $12,000 Single Transaction Limit does not apply within this pool; does not require a declared continuity event; subject to GP ratification within 30 days and the repayment undertaking in OA §12.5 |
| Rolling 30-Day Outflow Cap         | $50,000 USDC or 5% of treasury value (whichever is lower) — maximum total Treasury / Budget disbursements across all passed proposals in any rolling 30-day window. Signers must refuse execution of any proposal that would cause the rolling total to breach this cap and must report the refusal to RAC immediately. Adjustable by Treasury & Budget proposal. |
| Emergency Safe Address             | Must be designated **before the Company receives the principal asset transfer** (OA Schedule 5, conditions 8–9). During the Transition Period, designation is made by Transition RAC resolution published to the Official Venue, as part of establishing the treasury and custody framework (OA §6.5(d)); thereafter, changes to the designated address require a Treasury & Budget proposal. Until designated, Tier 2 emergency asset movement (Emergency & Safeguards Policy §6) is not available. The designated address is recorded in the **On-Chain Identifiers & Verification Policy §5** with its explorer verification link. |

---

### 6.2 Treasury Structure

| Parameter                 | Value       |
| ------------------------- | ----------- |
| Multi-account Requirement | Yes         |
| Multisig Threshold        | See §6A. Post-activation: 3-of-5 standard, 4-of-5 high-risk. Transition Period: 2-of-3 standard; protected/high-risk unanimous among all seated signers, minimum two (3-of-3 at full strength) (3 Transition RAC signers; OA §9.10–9.11) |
| Audit Requirement         | Mandatory — an independent treasury audit is required annually. The RAC is responsible for scoping the audit and bringing an auditor appointment to governance for approval. The first audit process must be initiated within the first 12 months of entity formation. |
| Account Architecture Authority | Phase-dependent. **Transition Period:** the Transition RAC establishes and may adjust the account architecture (number of accounts, operational/reserve/grants segmentation, custody, initial signer set) by resolution published to the Official Venue (OA §6.5(d)), each account under multisig at the §9.11 thresholds; signer/threshold changes and material-asset moves are protected matters (OA §9.12). Once the Activation Statement is published, the structure is settled (changes only to remedy a security incident). **Post-activation:** changes by Governance Proposal only. Operative rule: Treasury Signers Rules §10A.1. |

---

### 6.3 On-Chain Identifiers

The concrete on-chain identifiers for the treasury and governance infrastructure — the multi-signature treasury account(s), the Emergency Safe Address, the governance smart-contract component, the Owner Badge, and the voting-power resources — are not held in this registry. They are recorded, with public explorer verification links and their setup and use rules, in the **On-Chain Identifiers & Verification Policy**, which is the operational record referenced by **Operating Agreement §11.4** and **Certificate of Formation Article VII**. This registry holds only the numeric parameters governing those identifiers (§6.1, §6.2, §6A).

---

## 6A. Treasury Signers Parameters

> **Phase scope.** The table below specifies the **post-activation** (permanent) signer set. During the **Transition Period** the signer set is the **3 Transition RAC members** acting as initial signers (Operating Agreement §9.10–9.11): **2-of-3** for standard actions and, for protected / high-risk matters, **unanimity of all seated signers, being not fewer than two** (3-of-3 at full strength), with the continuity floor at fewer than **2** available signers (Treasury Signers Rules §15; Governance Continuity Framework §4.6) and seat replacement under Operating Agreement §6.11. The 5-signer / 3-of-5 / 4-of-5 values below take effect on the **Activation Date**, when Treasury Signing passes to the 5 Delegates then holding it.
>
> **Seat composition.** The 5 seats are **allocated seats** and **elected seats**, and the default number of elected seats is **zero** (Delegate Mandate §3.1). An allocated seat is seated by RAC allocation from among seated RAC members and has no term of its own; an elected seat is filled under the Elections & Role Governance Policy §§5–9, its holder need not hold a RAC seat, and it carries the Signer Term Length below. Elected seats arise only where the DAO has so resolved by Governance Process proposal, where an allocated seat has converted under the conversion duty (Delegate Mandate §3.3), or where the Transition RAC designated one in the initial roster (§3.2). Where there are no elected seats and the Permanent RAC is at its minimum of 5 seated members, all 5 hold Treasury Signing.

| Parameter                       | Value                           | Description                                           |
| ------------------------------- | ------------------------------- | ----------------------------------------------------- |
| Number of Treasury Signers    | 5                               | Total signer pool. The roster must comprise exactly 5 holders at all times, allocated seats plus elected seats (Delegate Mandate §3.1) |
| Elected Treasury Signing Seats  | 0 (default)                     | Number of the 5 seats filled by election rather than RAC allocation. Default zero. Set after activation by Governance Process proposal, before activation by the Transition RAC (Delegate Mandate §3.1, §3.2), or raised by one where an allocated seat converts under the conversion duty (Delegate Mandate §3.3). Allocated seats = 5 minus this value |
| Minimum Signing Threshold       | 3 of 5                          | Minimum approvals required for standard actions       |
| High-Risk Signing Threshold     | 4 of 5                          | Minimum approvals required for high-risk actions      |
| Signer Term Length              | 6 months                        | Term of an **elected** Treasury Signing seat. An allocated seat has no term of its own and runs with the holder's RAC seat (Delegate Mandate §3; Elections & Role Governance Policy §8) |
| Max Execution Window            | 5 business days                 | Time allowed to execute an approved action            |
| Max Acknowledgement Window      | 2 business days                 | Time allowed to acknowledge a valid execution request |
| Emergency Execution Window      | ASAP, within 24 hours           | Required response time during emergencies             |
| Required Availability Standard  | Respond within 2 business days  | Minimum expected responsiveness during active periods; declared unavailability periods are excluded (see Treasury Signers Rules §15) |
| Key Rotation Review Interval    | Every 6 months                  | Frequency of key / access review                      |
| Max Unexcused Inactivity Period | 21 days                         | Inactivity threshold before replacement review; declared unavailability periods are excluded (see §6B and Treasury Signers Rules §15) |
| Signer Replacement Window       | 21 days                         | Time to fill a vacant signer seat                     |
| Allowed Unilateral Actions      | None unless explicitly approved | Default rule for signer authority                     |
| Conflict Disclosure Requirement | Mandatory                       | Public or confidential as appropriate                 |
| Signer KYC Requirement          | Required where applicable       | Compliance standard                                   |

---

## 6B. Elections & Roles Parameters

| Parameter                           | Value     | Description                              |
| ----------------------------------- | --------- | ---------------------------------------- |
| Standard Term Length                | 6 months  | Default role duration                    |
| Auto-Renewal                        | Yes — unless challenged | Incumbent role holders are automatically renewed at term end unless a challenge is filed or the role holder declines (see Elections & Role Governance Policy §9) |
| Term Renewal Challenge Window       | 14 days (opens 21 days before expiry, closes 7 days before expiry) | Period during which an eligible Governance Participant may file a unilateral challenge notice to trigger a new election |
| Challenge Filing Threshold          | 0.1% of eligible voting power | Minimum holding required to file a valid challenge notice; verified against the most recent governance snapshot |
| Consecutive Renewal Cap             | 4 terms (2 years maximum continuous service) | After 4 consecutive terms in the same role, a standard election is mandatory; successful re-election resets the count to 1 |
| Election Voting Duration            | 5-7 days  | Length of an election vote. Applies to the Majority Judgment grading round, to Stage 1 shortlisting, and to each Stage 2 confirmation vote. It is the base that both rerun periods double, so the two mechanisms cannot drift apart on voting length |
| Nomination Period                   | 7–10 days (concurrent with Discussion; see §3.1) | Nominations open at the start of the Nomination & Discussion Window and close when the window closes. Governed by the combined window parameter in §3.1. |
| Minimum Participation for Elections | 7% (Governance Process quorum) | Quorum for an election vote, measured as Participation against eligible voting power at the snapshot. Applies to the Majority Judgment election vote (Proposal & Voting Framework §6.2.4) and, as the Election Stage 2 Quorum below, to each Stage 2 confirmation vote. Stage 1 shortlisting has no separate quorum — the Temperature Check result is sufficient (§6.2.5) |
| Removal Vote Threshold              | **None of its own** | A removal is an ordinary Governance Process proposal: 7% quorum, ≥ 60% YES (§3.2, §3.3), subject to the §3.3A floor. Cross-reference only, so that unseating costs at least what seating cost (Elections & Role Governance Policy §10.1) |
| Inactivity Threshold                | 21 days   | Time before inactivity review; declared unavailability periods are excluded. **"Inactivity"** means: no response to governance execution requests, no participation in any multisig signing actions, and no communication with the RAC within the threshold period. Passive activities (reading updates, monitoring forums) do not constitute activity. Declared unavailability periods (per Treasury Signers Rules §15) are excluded from inactivity counting. |
| Replacement Election Trigger Time   | 7 days    | Time before election must start          |
| Replacement Completion Time         | 21 days   | Max time to fill vacancy                 |
| Floor-Protected Resignation Notice  | 14 days   | Advance notice a RAC member (or Treasury Signer) must give where their resignation would reduce seated members below the applicable RAC floor (Permanent RAC: 5; Transition RAC: 3 — §5.1) or active Treasury Signers below the applicable execution quorum (post-activation 3-of-5; Transition Period 2-of-3 — §6A). During the notice period the member remains in office and the replacement process begins; the resignation takes effect on the earlier of a qualified replacement being seated or notice expiry. If the member cannot or will not serve the notice, the seat vacates immediately and the vacancy is escalated as a continuity event (Governance Continuity Framework §4.1/§4.2). A resignation leaving the body at or above the floor takes effect immediately. Operative rule: Elections & Role Governance Policy §11.2. |
| Delegated Function Seating          | RAC allocation (default) | Delegated Functions are allocated by the RAC from among its seated members and run with the holder's RAC seat; an allocated function is not separately elected and carries no term, renewal cycle, or challenge window of its own (Delegate Mandate §3). The DAO may resolve by Governance Process proposal that a function be filled by Election Proposal instead — for **Treasury Signing**, which is held by five Delegates, seat by seat (§6A — Elected Treasury Signing Seats); for every other function, as a whole. An elected seat carries its own term and the Elections & Role Governance Policy §§5–9 apply to it in full. Two exceptions to the seated-RAC-member requirement, and only two: the holder of an elected seat, and an interim Treasury Signer appointed from the Emergency Signer Reserve (Governance Continuity Framework §4.2; Treasury Signers Rules §15). Governance Operations, Legal Signatory, Compliance Liaison and Web2 Custodian are each held by one Delegate; every function must be held at all times, and one the RAC cannot allocate converts to an elected seat (Delegate Mandate §3.3) |
| Delegate Count — Minimum            | 5         | Minimum total Delegates; bounded below by the 5 Treasury Signers required under §6A. May not fall below 5 while the Treasury Signing roster requires 5 holders. Holders of elected Treasury Signing seats count toward this total whether or not they hold a RAC seat. |
| Delegate Count — Maximum            | 12        | Maximum total Delegates. Adjustable by Governance Process proposal. **Note:** where every Delegated Function is seated by RAC allocation from among seated RAC members, the effective maximum is the Permanent RAC size (§5.1 — currently 5 to 7). This value binds only where one or more functions or seats are filled by election, each elected holder without a RAC seat adding to the total. |
| Max Concurrent Roles per Individual | 2         | Limits role concentration. A "role" is an elected or appointed position: a RAC seat, a Delegate seat (regardless of how many Delegated Functions the Delegate holds), a Working Group Steward seat, or a Strategic Coordination WG seat. Delegated Functions held by a single Delegate do not multiply the role count. |
| Conflict Disclosure Requirement     | Mandatory | Required for all roles                   |
| Election Shortlist Multiplier       | 2×        | Stage 1 shortlist slots per open seat (e.g. 3 seats → top 6 advance to Stage 2) |
| Election Stage 1 Max Selections     | Unrestricted | Voters may approve any number of nominees in the Stage 1 Approval Voting proposal |
| Election Stage 2 Quorum             | 7% (Governance Process) | Quorum required for each Stage 2 confirmation vote |
| Election Stage 2 Approval Threshold | ≥ 60% YES (Governance Process) | Approval required for each Stage 2 confirmation vote. Stage 2 uses the Confirmation Vote type (Proposal & Voting Framework §6.2.7) with no ABSTAIN option, so quorum and approval share the same YES + NO denominator. The §3.3A Minimum Affirmative Support floor does not apply; the two thresholds together already imply ≥ 4.2% affirmative support (7% × 60%). The **Grade Quantile** is set to the same figure, so both mechanisms put the same share-of-turnout test to a candidate |
| Election Stage 2 Rerun Quorum       | 5%        | Reduced quorum for the single permitted rerun of a **quorum-held-over** Stage 2 candidate — one who met the Election Stage 2 Approval Threshold in the prior round but missed the Election Stage 2 Quorum (Elections & Role Governance Policy §7.3). Applies only to such candidates; a candidate below the approval threshold is rejected and does not rerun, so a quorum shortfall cannot rescue a rejected candidate. |
| Election Stage 2 Rerun Approval Threshold | ≥ 75% YES | Raised approval threshold for the reduced-quorum rerun, compensating for the lower quorum with a stronger mandate requirement (Elections & Role Governance Policy §7.3) |
| Election Stage 2 Rerun Voting Period | Double the Election Voting Duration (above) | Extended voting window for a Stage 2 rerun, giving thin turnout more time to participate. Defined against the same base as the MJ Rerun Voting Period, so the two mechanisms' reruns cannot diverge in length |
| Max Election Stage 2 Reruns         | 1         | A quorum-held-over candidate may be re-run at the reduced rerun quorum at most once; if still short, the seat is filled by fallback advancement or, failing that, the vacancy / founding re-run process (Elections & Role Governance Policy §7.3, §11, §17.1) |
| Grade Quantile                      | **Three-fifths — fixed in Proposal & Voting Framework §6.2.4; not a parameter** | The share of voting power cast that must place a candidate at or above a grade for that grade to be their qualifying grade. **Cross-reference only** — part of the counting mechanics, not a threshold applied to a result, so it is altered by amending §6.2.4 and does not vary between elections or rounds. Set to equal the Election Stage 2 Approval Threshold below |
| MJ Minimum Qualifying Grade         | Good      | The lowest qualifying grade at which a candidate may be seated (Proposal & Voting Framework §6.2.4; Elections & Role Governance Policy §7A.1). A candidate below it is not seated and the seat passes to the next-ranked electable candidate. The Majority Judgment counterpart to the Election Stage 2 Approval Threshold — a threshold on rank, not on vote share. Not independent of the Grade Quantile above: at three-fifths, Good means three-fifths of the power cast placed the candidate at Good or better, so neither should be altered without reference to the other |
| MJ Rerun Quorum                     | 7% — **the same as the first round** | Quorum for the single permitted rerun of a Majority Judgment election that closed below the Minimum Participation for Elections (Elections & Role Governance Policy §7A.3). Deliberately **not** reduced: a rerun re-puts the same question to the same electorate on the same snapshot, so its remedy is time rather than a lower bar, and a reduced quorum would make the rerun cheaper to control than the round it rescues. Full reasoning: Proposal & Voting Framework §6.2.4. A round that meets quorum but seats nobody is not a quorum failure and does not rerun |
| MJ Rerun Minimum Qualifying Grade   | Good — **the same as the first round** | The electability floor is unchanged on rerun. Raising it would not constrain a block that meets the Grade Quantile, since meeting the quantile means choosing the grade, and would burden a broad electorate while leaving a concentrated one unaffected. The Grade Quantile is likewise unchanged (§6.2.4) |
| MJ Rerun Voting Period              | Double the Election Voting Duration (above) | Extended voting window for a Majority Judgment rerun. This is the entire remedy the rerun offers: the same electorate, measured against the same snapshot and the same thresholds, given twice as long to participate. Runs from the RAC's rerun notice (Elections & Role Governance Policy §7A.3) |
| Max MJ Reruns                       | 1         | A Majority Judgment election may be re-run **at most once**, at the same quorum, Grade Quantile and Minimum Qualifying Grade as the round it follows — the only remedy is the doubled MJ Rerun Voting Period: **more time, not a lower bar**. If the rerun also closes below quorum, no candidate is elected and all seats are referred to vacancy handling (Elections & Role Governance Policy §7A.3, §11, §17.1). The cap applies **per election** and does not limit the number of fresh elections §17.1 may require |
| Election Tie Runoff Quorum          | 3% (Temperature Check quorum) | Quorum for a tie runoff — the Approval Voting poll run among tied candidates under Elections & Role Governance Policy §7.2.1, §7A.4 or §7A.4A. Set at the Temperature Check level, not the 7% election quorum, because the runoff runs over the short Temperature Check period (§3.1) and separates candidates the electorate has already approved through a quorate round; it decides seating order, not eligibility. Measured as Participation, on the runoff's own snapshot (Proposal & Voting Framework §6.1). The minimum winner threshold in §3.5 does not apply. A runoff that fails to reach this quorum, or that is itself tied, leaves the seat unfilled and refers it to vacancy handling (§11; founding election: §17.1) |
| Reserve List Validity Period        | 90 days   | Period from election completion during which a candidate who cleared the election's bar but was not seated (Elections & Role Governance Policy §7.2.1, §7A.2) may fill a same-role vacancy without a replacement election (§7.5). **Does not apply to a seat vacated by removal**, which always goes to a replacement election (§7.5, §10.1A, §11) |

---

## 6C. Dispute Resolution Parameters

| Parameter                       |   Value   | Description                          |
| ------------------------------- | --------- | ------------------------------------ |
| Level 1 Resolution Window       | 3–5 days  | Time for direct resolution           |
| Level 2 Mediation Window        | 5–7 days  | WG mediation time                    |
| RAC Review Window               | 5–7 days  | Time for RAC review                  |
| Max Escalation Time             | 21 days   | Total allowed escalation time        |
| Signer Response Time            | 48 hours  | Time to respond to execution request |
| Signer Dispute Escalation Time  | 48 hours  | Time before escalation allowed       |
| Misconduct Review Window        | 7–14 days | Time to review misconduct claims     |
| Abuse Threshold                 | Case by case (RAC discretion, subject to DAO review) | Limit on repeated frivolous disputes |

---

## 7. Working Group Parameters

> **Phase scope.** The procurement parameters below — the **RFP Threshold**, the **Independent Review Panel Threshold**, the engagement renewal parameters, the award-challenge parameters, and the continuity-bridge parameters — take effect on the **Activation Date** and bind **any body with treasury-spending authority**, not Working Groups alone. From that date they apply to a Working Group engaging a provider within its approved budget, and equally to the **Permanent RAC** where it engages a provider because no relevant Working Group exists (Contributor Compensation Policy §6). The **Transition RAC is not bound** by them when selecting contributors under its narrow formation mandate (Operating Agreement §6.5); that exception is stated in Contributor Compensation Policy §6 and is limited to the Transition Period. Composition and reporting parameters apply from the establishment of each Working Group.

| Parameter           | Value    | Description |
| ------------------- | -------- | ----------- |
| Stewards per WG     | 1–3      | Number of Steward seats per Working Group |
| Term Length         | 6 months | Standard Steward appointment term |
| Reporting Frequency | Monthly  | Progress and spend reporting cadence (Working Group Framework §8) |
| RFP Threshold | $2,500 USDC | Engagements at or above this value require a formal RFP process (Contributor Compensation Policy §6). Measured **per provider per rolling 12-month period**, aggregating all engagements with the same provider or affiliated group, so a single engagement may not be split into smaller direct awards to remain below it. Effective from the Activation Date |
| Independent Review Panel Threshold | $10,000 USDC | Engagements at or above this value **require** an independent review panel to evaluate RFP submissions (Contributor Compensation Policy §6.3). Same per-provider rolling 12-month measurement basis as the RFP Threshold. Effective from the Activation Date |
| Independent Review Panel Minimum Size | 3 | Minimum number of panel members appointed by the RAC under Contributor Compensation Policy §6.3. Members may not be Stewards of the commissioning Working Group, nor hold a disclosed conflict in relation to a bidder |
| Independent Review Panel Minimum Size (RAC engagements) | 2 | Panel size where the Permanent RAC is itself the engaging body because no relevant Working Group exists (Contributor Compensation Policy §6.3, §6). The panel is drawn from the RAC's own seated members, who recuse from the selection decision. Set at 2 because the Permanent RAC has a minimum of five seated members and no RAC decision may be taken with fewer than three non-recused members (§5.1) — a larger panel would deadlock the body at minimum strength |
| Engagement Consecutive Renewal Cap | 2 renewals | Maximum consecutive renewals of a single engagement with the same provider before competition becomes mandatory (Contributor Compensation Policy §6.5.4). The entitlement does not vary with the length of the original term. At the cap the engagement must be competed under an RFP, or continued under a Governance Proposal authorising sole-source engagement. A completed RFP resets the count; a sole-source Governance Proposal does not. Effective from the Activation Date |
| Maximum Engagement Renewal Term | 12 months | Longest term a single renewal may run, regardless of the length of the original term (Contributor Compensation Policy §6.5.1). With the renewal cap above, an engagement may run for its original term plus a maximum of 24 further months. Effective from the Activation Date |
| Engagement Renewal Price Increase Cap | 10% cumulative, measured against the price at original award | Maximum total price increase permitted across all renewals of a single engagement under the price increase exception (Contributor Compensation Policy §6.5.2). Measured against the original award price rather than the preceding renewal, so successive increases cannot compound past the cap. Where a proposed increase would exceed it, the engagement must be competed or continued under a Governance Proposal. Effective from the Activation Date |
| Engagement Renewal Challenge Window | Same as **Term Renewal Challenge Window** (§6B) | Period during which a Governance Participant may file a unilateral challenge notice voiding a proposed engagement renewal (Contributor Compensation Policy §6.5.3). Defined by reference so the two windows cannot diverge |
| Engagement Renewal Challenge Filing Threshold | Same as **Challenge Filing Threshold** (§6B) | Minimum holding required to file a valid engagement-renewal challenge. Defined by reference so the two thresholds cannot diverge |
| Award Challenge Window | Same as the Contributor Compensation Policy §6.3 community comment period — **7 days** | Period during which a selection under an RFP may be challenged (Contributor Compensation Policy §6.3A). Defined by reference to the existing comment period so the two cannot diverge and so arming the window adds no delay to an unchallenged award. Engagement confirmation under §6.4 may not take place while the window is open. Effective from the Activation Date |
| Award Challenge Filing Threshold | Same as **Challenge Filing Threshold** (§6B) | Minimum holding required to file a valid award challenge (Contributor Compensation Policy §6.3A.1). Defined by reference so it cannot diverge from the renewal-challenge and Compliance Challenge thresholds. A qualified bidder holds a referral right only and does not file, so no separate bidder threshold applies |
| Award Challenge Determination Window | 10 business days | Period within which the reviewing body determines an award challenge (Contributor Compensation Policy §6.3A.3). Set to accommodate the ordinary remedy — re-evaluation of submissions already received by a panel constituted free of the defect — rather than only a documentary review. Engagement confirmation is suspended for its duration. Effective from the Activation Date |
| Bridge Challenge Extension | 30 days | Maximum extension of a continuity bridge where the award concluding the competition is itself challenged under Contributor Compensation Policy §6.3A (Contributor Compensation Policy §6.6.3). Prevents a challenge timed near bridge expiry from terminating the service by running the review past the cap. Non-renewable; a second challenge does not extend the bridge again. Effective from the Activation Date |
| Continuity Bridge Cap | 60 days | Maximum duration of a continuity bridge, during which a challenged renewal of a **continuity-critical** engagement continues on unchanged scope and price while the engagement is competed (Contributor Compensation Policy §6.6.3). Set at roughly twice the minimum Contributor Compensation Policy §6 competition path (14-day RFP open period, evaluation, independent review panel above the Independent Review Panel Threshold, 7-day comment, contracting) — long enough to absorb one round of slippage, short enough that the bridge cannot substitute for competing on time. Where the competition has not concluded by expiry, the engagement ends; extension requires a Governance Proposal. Non-renewable; one bridge per engagement. Effective from the Activation Date |
| Bridge RFP Publication Deadline | 10 business days | Period within which the engaging body must publish the RFP after the RAC acknowledges a challenge to a continuity-critical engagement (Contributor Compensation Policy §6.6.3). Measured from the acknowledgement so the bridge cannot be consumed by delay in starting the competition it exists to accommodate. Effective from the Activation Date |
| Pre-Activation Designation Window | 30 days from the Activation Date | Single window in which an engagement already in effect on the Activation Date may be designated continuity-critical (Contributor Compensation Policy §6.6.5). A pre-Activation engagement had no award-time opportunity to be designated; a designation not made within this window is unavailable until a completed competition under Contributor Compensation Policy §6 opens the question again |

---

## 8. Identity & Participation Parameters

| Parameter | Value | Description |
| --------- | ----- | ----------- |
| Voting Basis | XRD and LSU (constitutional floor, entrenched per Charter §12.1 item 4) plus RAC-governed supplementary sources as listed in §8A below | — |
| LSU Inclusion | Active — snapshot-based XRD conversion | — |
| Delegation | **Not yet enabled** — pending platform support | Charter §5 recognises delegation of voting power to a representative of the holder's choosing as a mode of governance participation. It is not yet available because the recognised governance platform does not support it. This row records **implementation status**, not a limitation on the Charter right, and enabling delegation once the platform supports it requires no Charter amendment |
| Sybil Resistance | Not active | — |
| UBO KYC Threshold | >25% of eligible voting power | Triggers mandatory KYC under Marshall Islands DAO Act; annual BOIR filing required Jan 1–Mar 31 |
| Compensation KYC Requirement | Required before first payment | Applies to all compensated contributors, contractors, and grant recipients (Standard and Strategic), **and to any individual or entity receiving expense reimbursement** — including pure documented cost recovery under Execution & Treasury Actions Policy §7.3 Model A, which carries no labour component. There is no de minimis exemption. Mirrors the scope in Contributor Compensation Policy §3.5 |

---

## 8A. Eligible Voting Power Sources

| Tier | Source | How to change |
|---|---|---|
| 1 — Constitutional floor | Liquid XRD | Constitutional Proposal (66% approval, 10% quorum) — cannot be removed |
| 1 — Constitutional floor | LSU → XRD-equivalent at snapshot | Constitutional Proposal (66% approval, 10% quorum) — cannot be removed |
| 2 — RAC-governed | LSULP → XRD-equivalent at snapshot | RAC routine decision + 30-day notice |
| 2 — RAC-governed | Fungible LP pool units (Ociswap, CaviarNine, DefiPlaza) | RAC routine decision + 30-day notice |
| 2 — RAC-governed | Ociswap precision pools (V1 and V2) | RAC routine decision + 30-day notice |
| 2 — RAC-governed | CaviarNine shape pools | RAC routine decision + 30-day notice |

**Rules for RAC changes to Tier 2 sources:**

- Any change must specify an `effectiveFrom` date at least 30 days in the future, ensuring no active proposal is caught between source configurations.
- The RAC must publish the change to the governance forum and notify Governance Participants at least 30 days before `effectiveFrom`.
- The standard 48-hour Compliance Challenge Window (§4) applies to all RAC source-list decisions.
- Adding a new source requires a written rationale demonstrating that the source represents genuine XRD-network economic alignment.
- Removing a Tier 2 source follows the same process as adding one.

---

## 9. Execution Parameters

| Parameter                 | Value          |
| ------------------------- | -------------- |
| Pre-Execution Hold        | 48 hours after RAC result publication (mandatory) — Treasury Signers may not initiate execution of any Treasury / Budget or Executable proposal until the Compliance Challenge Window (§4) has fully closed |
| High-Risk Execution Delay | 24 hours additional after the pre-execution hold (mandatory) — applies to transactions classified as high-risk (4-of-5 signing threshold post-activation; unanimous-of-seated, minimum two, during the Transition Period, per §6A); total minimum 72 hours after RAC result publication |

---

## 9A. Governance Continuity Parameters

| Parameter | Value | Description |
|---|---|---|
| Governance Inactivity Trigger | 3 consecutive quorum failures on the **same proposal** — the same substantive proposal, resubmitted after each failed attempt | Threshold before reduced quorum activates. The trigger is **per-proposal**, not per-category: three unrelated proposals of the same type failing quorum do **not** place other proposals of that type into reduced-quorum mode. Reduced quorum attaches only to the specific proposal that has failed three times in a row |
| Reduced Quorum Threshold | 50% of the standard quorum for that proposal type (minimum 1%) | Applies after inactivity trigger is met. For Constitutional proposals the reduced quorum may not fall below the entrenched 7% floor (Charter §12.1 item 2); the effective reduced Constitutional quorum is therefore 7% |
| Reduced-Quorum Approval Uplift | +15 percentage points | A proposal confirmed **under the reduced quorum** must reach a YES share at least 15 percentage points above its standard approval threshold (Governance Process 60% → 75%; Executable 50% → 65%), compensating the lower quorum with a stronger mandate. Constitutional proposals are unaffected — they retain their standard ≥66% approval and the entrenched 7% quorum floor. Does not apply to a proposal that meets its ordinary quorum |
| Reduced Minimum Affirmative Support | 50% of the standard floor for that proposal type (§3.3A) | The Minimum Affirmative Support floor scales down in step with the reduced quorum, so that the floor cannot defeat the continuity fallback it sits alongside. Governance Process 2% → 1%; Executable 1% → 0.5%; Constitutional 3.5% → 1.75%. In most cases the reduced floor is non-binding, because the Reduced-Quorum Approval Uplift already implies a higher YES share (e.g. Governance Process: 3.5% quorum × 75% uplifted approval = 2.6%); it operates as a backstop against an ABSTAIN-heavy reduced-quorum vote |
| Extended Voting Period | Double the standard voting duration | Applies alongside reduced quorum during inactivity |
| Reconstitution Deadline | 30 days after failure event | Maximum time to re-establish a failed role or body |

**Reduced-quorum notice:** When the reduced quorum activates for a proposal, the RAC must publish a reduced-quorum activation notice to the Official Venue at the opening of the reduced-quorum voting window, stating that the vote proceeds under reduced quorum and the raised approval threshold (Reduced-Quorum Approval Uplift). The extended (doubled) voting period runs from that notice, giving the wider community time to participate before the vote can finalise.

**Treasury / Budget exclusion:** Treasury / Budget proposals are excluded from the Governance Continuity Fallback. A Treasury / Budget proposal that fails to meet quorum must be resubmitted with revised scope or timing; the reduced quorum threshold and extended voting period do not apply.

**Elections exclusion:** Election proposals are excluded from the Governance Continuity Fallback, under **both** election mechanisms — the Majority Judgment election vote and its rerun (Proposal & Voting Framework §6.2.4), and Stage 1 shortlisting and Stage 2 confirmation votes (§6.2.5). Each mechanism carries its own low-turnout handling rather than the reduced quorum threshold in this section, and the two handle it differently:

* **Two-stage** — the Stage 2 quorum-held-over rerun: the Election Stage 2 Rerun Quorum paired with the raised Election Stage 2 Rerun Approval Threshold (§6B; Elections & Role Governance Policy §7.3)
* **Majority Judgment** — a single rerun at the **unchanged** quorum and electability floor over a doubled voting period (§6B; Elections & Role Governance Policy §7A.3). Majority Judgment is the one mechanism in this framework whose low-turnout handling does **not** reduce a quorum, because it has no share-of-votes threshold that could be raised to compensate — see the MJ Rerun Quorum row in §6B

---

## 10. Emergency Parameters

| Parameter           | Value           |
| ------------------- | --------------- |
| Emergency Duration  | Max 7 days      |
| Disclosure Deadline | Within 48 hours |
| Post-Review Window  | 7 days          |
| Governance Capture Notice Period | 24 hours from publication of the RAC's pre-action notice — period within which an objection notice may be filed (Emergency & Safeguards Policy §4) |
| Governance Capture Fast-Track Voting Period | 48 hours — duration of the fast-track vote opened where an objection notice is filed (Emergency & Safeguards Policy §4) |

---

## 11. Amendments

_Amendment procedures, change classification (minor parameter adjustment vs. major structural change), and versioning requirements are defined in the **Governance Maintenance & Upgrade Framework §4–6**._
