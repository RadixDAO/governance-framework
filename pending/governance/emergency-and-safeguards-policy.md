# Emergency & Safeguards Policy

| Field | Value |
|---|---|
| **Version** | v1.0.0 |
| **Last updated** | 2026-08-25 |

---

## 1. Scope

This document defines:

* What constitutes an emergency
* Who may act during emergencies
* What actions are permitted
* Safeguards against misuse
* Post-emergency accountability

---

## 2. [Reserved]

*This section number is retained, rather than renumbered, so that references to the sections below remain stable.*

---

## 3. Guiding Principles

Emergency powers must be:

* **Exceptional** — used only when normal governance cannot respond in time
* **Minimal** — limited to what is strictly necessary
* **Temporary** — automatically expire
* **Accountable** — subject to a mandatory retrospective review

---

## 4. Definition of Emergency

An emergency is a situation where immediate action is required to prevent:

* Loss or compromise of treasury assets
* Exploitation of protocol vulnerabilities
* Critical failure of network infrastructure
* Security compromise (e.g., keys, contracts, systems)
* Severe disruption to DAO operations
* Governance capture — a passed proposal that would result in material and irreversible misappropriation of treasury assets in a manner that is plainly contrary to the non-distribution principle (Charter §10–11, Operating Agreement §§3.4–3.5), where the RAC has reasonable grounds to believe the proposal was advanced through coordinated bad-faith token accumulation rather than legitimate community governance

**Governance capture pre-action notice:** Before invoking emergency powers on governance capture grounds, the RAC must publish a pre-action notice to the governance forum stating the specific evidence of bad-faith accumulation.

Any Governance Participant holding at least the Challenge Filing Threshold (DAO Parameters §6B), verified against the most recent governance snapshot, may file an objection notice within the Governance Capture Notice Period (DAO Parameters §10).

Where an objection notice is filed, the RAC opens a fast-track vote over the Governance Capture Fast-Track Voting Period (DAO Parameters §10), at the Treasury / Budget quorum and approval threshold (DAO Parameters §3.2, §3.3), the question being whether the RAC may invoke emergency powers on those grounds. The RAC may invoke them only if that vote passes. Where no objection notice is filed within the notice period, the RAC may proceed.

Execution of the proposal to which the pre-action notice relates is suspended from publication of that notice until the notice period expires with no objection notice filed, or the fast-track vote closes. Treasury Signers must not initiate or complete execution during the suspension.

---

## 5. Emergency Authority

### 5.1 Authorized Body

The Accountability Council (RAC) is authorized to act during emergencies.

When the RAC cannot meet quorum due to deaths or incapacitations, the fallback chain defined in the Governance Continuity Framework §4.1 applies: surviving RAC members (Tier 1), then the Governance & Legal WG (Tier 2), then Governance Participants (Tier 3). Fallback authority is strictly scoped to activation and appointment actions — it does not extend to the full emergency powers held by a functioning RAC.

---

### 5.2 Threshold

Emergency actions require:

* Defined quorum of RAC members
* Elevated approval threshold (e.g., supermajority)

Exact thresholds defined in DAO Parameters.

---

## 6. Permitted Emergency Actions

Emergency actions are divided into two tiers based on whether they involve asset movement.

### Tier 1 — Pause / Restrict (no asset movement)

The RAC may:

* Pause or restrict vulnerable systems
* Halt execution of unsafe proposals
* Initiate protective measures
* Coordinate immediate response actions

**Requires:** ≥2/3 RAC members + 75% approval threshold (DAO Parameters §5.2).
**Disclosure:** Public notice within 48 hours (DAO Parameters §10).

---

### Tier 2 — Asset Movement

The RAC may move treasury assets to the pre-approved emergency safe address only (DAO Parameters §6.1). Assets may not be moved to any other address under emergency authority. **Emergency asset movement does not extend to the Master Badge or the Owner Badge**, which are held in the treasury account but are not treasury assets for this purpose (On-Chain Identifiers & Verification Policy §4): moving either under emergency authority is a prohibited action under §7, since it would relocate the root of governance control at a lower threshold than any rule governing the badge itself. Until an emergency safe address has been designated and recorded in DAO Parameters §6.1, Tier 2 asset movement is not available. The emergency safe address must be designated **before the Company receives the principal asset transfer**: during the Transition Period by Transition RAC resolution published to the Official Venue (OA §6.5(d)), and thereafter changed only by Treasury & Budget proposal (DAO Parameters §6.1).

**Requires:** ≥2/3 RAC members + 75% approval threshold AND immediate notification to all Treasury Signers within 1 hour AND community disclosure within 6 hours.
**Spend limit:** The $5,000 emergency spend limit (DAO Parameters §6.1) applies to new disbursements under emergency authority. Tier 2 protective transfers to the pre-approved address are not subject to the spend cap but are constrained to that address.
**Ratification:** Emergency asset movement is subject to the mandatory 14-day ratification vote (§10).

---

## 7. Prohibited Actions

The RAC must NOT:

* Introduce permanent governance changes
* Override DAO-approved outcomes beyond temporary suspension
* Allocate funds beyond emergency necessity
* Expand authority beyond defined scope

---

## 8. Emergency Execution

Emergency actions may be:

* On-chain (e.g., contract pause, treasury move)
* Off-chain (e.g., coordination, legal actions)

All actions must follow:

* Minimum necessary intervention
* Clear justification

---

## 9. Transparency & Disclosure

### 9.1 Immediate Disclosure

* Action must be logged as soon as safe

---

### 9.2 Post-Event Disclosure

Must include:

* What happened
* What actions were taken
* Why they were necessary
* Impact assessment

---

## 10. Post-Emergency Review

After resolution:

* The RAC must publish a full post-event disclosure within **48 hours** of the emergency action being taken (see DAO Parameters §10)
* A formal DAO review must be **scheduled within 7 days** of disclosure
* The DAO vote on ratification must **conclude within 14 days** of the review being opened
* Community may:

  * ratify actions (no further consequence)
  * reverse actions where possible
  * impose consequences including RAC member removal

**Acts that cannot be reversed are deferred instead of reviewed.** "Reverse actions where possible" is the operative limit of this section. **Charter §12.2 item 6** accordingly withholds authority, until an emergency amendment is ratified, for the three acts that cannot be undone: **seating a person in a role** (a condition precedent under Elections & Role Governance Policy §7.4, reaching reserve-list seating too), **changing the treasury signer set or its thresholds**, and **transferring the Owner Badge or the Governance Operations function**. Each is on-chain or personal state that a failed ratification cannot restore — most acutely the badge, which governs the very mechanism an unwinding would run through. For these the review takes place **before** the act, and the remedies above are addressed to what remains.

This does not slow a genuine emergency. An emergency amendment changes a *rule*; urgent operational action runs on the powers the framework already confers within its rules — interim signers under **Governance Continuity Framework §4.2**, suspension under **Code of Conduct §6.2**, the protective measures in §6 above — none of which requires an amendment.

---

## 11. Post-Emergency Recovery

Emergency actions are intended to stabilize the system and mitigate immediate risks.

Where an emergency impacts governance functionality, system recovery and restoration of normal operations must follow the Governance Continuity Framework.

This ensures that:

* governance bodies are reconstituted where necessary
* authority is returned to standard processes
* temporary emergency measures are removed

Emergency powers must not be used to establish permanent governance changes.

---

## 12. Sunset of Emergency Actions

All emergency actions must:

* Expire automatically
* Return control to normal governance

---

## 13. Interaction with Governance

Emergency actions:

* Do NOT replace governance
* Temporarily override processes only when necessary
* Must defer back to governance as soon as possible

---

## 14. Safeguards Against Abuse

To prevent misuse:

* High approval thresholds required
* All actions publicly recorded
* Retrospective accountability enforced
* DAO retains removal power over RAC members

---

## 15. Compliance Challenge Interaction

* Emergency actions are not open to Compliance Challenge during execution
* Post-action review may override or invalidate outcomes

---

## 16. Emergency Funding

Limited emergency funds may be used for:

* Security mitigation
* Critical response

Must be:

* Justified
* Documented
* Reviewed post-event

---

## 17. Failure to Act

If the RAC fails to act within the emergency response window (DAO Parameters §10):

1. Any Governance Participant may file a Governance Process proposal to initiate emergency governance procedures and compel a response.
2. The Governance Continuity Framework fallback chain (§4.1) activates, allowing surviving RAC members, then the Governance & Legal WG, then Governance Participants to perform the minimum actions required to stabilize the situation.
3. Any RAC member's failure to act during a declared emergency is treated as misconduct and subject to review under the **Code of Conduct §6** and potential removal under **RAC Mandate §9**.

---

## 18. Governance Parameters

Defined separately:

* RAC emergency quorum
* Approval thresholds
* Time limits
* Emergency budget limits

---

## 19. Delegate Written Consent

Where this policy, the **Governance Maintenance & Upgrade Framework §9**, or **Charter §12.2** requires an action by the **written consent of the Delegates**, "written consent" means, for each Delegate, any of the following — all three forms are equally valid:

* a signed statement published by the Delegate to the **Official Venue** (the designated governance forum);
* a transaction signed by the Delegate's KYC-verified wallet address; or
* a signed instrument delivered to the **Legal Signatory** (Delegate Mandate; **Operating Agreement §1.15 and §9.2**).

Unanimous written consent requires consent in one of these forms from **every** Delegate then in office. During the Transition Period, when the Delegated Functions are held by the Transition RAC, "every Delegate then in office" means every seated Transition RAC member (Charter §12.2). A written-consent action takes effect when the consent of the last required Delegate is given, and is subject to any ratification requirement imposed by the provision that invokes it. Where an emergency requires action before a written-consent process can be completed, the RAC emergency authority in §5–§6 applies instead, subject to the post-emergency ratification and review requirements of this policy.

---

## 20. Amendments

_Amendment procedures and classification requirements are defined in the **Governance Maintenance & Upgrade Framework**._
