# RADIX DAO LLC -- this is the On-Chain Identifiers & Verification Policy incorporated by reference in Schedule 4 of the Operating Agreement of Radix DAO LLC, in accordance with clause 11.4 of that Agreement.

| Field | Value |
|---|---|
| **Version** | v1.0.0 |
| **Last updated** | 2026-08-25 |

---

## 1. Purpose

This policy establishes the single authoritative operational register of the Company's on-chain identifiers, states how each identifier is configured and used under the governance rules, and provides public links through which any person may independently verify the on-chain data.

It exists so that the governance and treasury infrastructure of the Company is publicly recorded, independently verifiable, and maintained by the community through governance rather than embedded in the Company's legal instruments.

The identifiers recorded in this policy are the operational record referred to in **Operating Agreement §11.4**, and correspond to the smart contracts listed in **Exhibit A of the Certificate of Formation**, which **clause 10** of that Certificate requires to be kept current. The Operating Agreement incorporates this register by reference; this policy does not alter, and remains subordinate to, the Operating Agreement and the Charter.

---

## 2. Scope

This policy covers:

* the governance smart-contract component(s), the Master Badge, and the Owner Badge;
* the resources that constitute eligible voting power;
* the recognised Governance Platform, the Official Venue(s), and the Compliance Challenge Filing Channel;
* the treasury multi-signature account(s), any segmented pool accounts, and the Emergency Safe Address.

This policy does **not** cover:

* the numeric thresholds, limits, and durations governing these identifiers, which remain in the **DAO Parameters Registry**;
* the identities of the persons holding signer or role keys, which are governed by the **Treasury Signers Operational Rules**, the **Elections & Role Governance Policy**, and **Operating Agreement Schedule 2**.

This policy records *what the identifiers are and how they are verified*; the operative rules governing their use live in the policies cross-referenced below and are not restated here.

---

## 3. Identifier Register — Governance

The following identifiers constitute the governance system. On-chain entries are recorded on the Radix network and each carries a public verification link; off-chain entries — the governance platform, the Official Venue(s), and the Compliance Challenge Filing Channel — carry a published, publicly reachable location.

An entry shown in square brackets in this section or in §5 is not yet recorded. Each is completed when the corresponding entity is deployed, established, or designated, in accordance with §8. An identifier that has not been recorded may not be relied upon in governance (Charter §6A).

| Function | Network | Identifier | Verify |
|---|---|---|---|
| Governance smart-contract component | Radix Mainnet | `component_rdx1cp90ys553uwxuckev249x5wezucqru0u4qr7qdxdc9tlpmnh93242k` | `https://dashboard.radixdlt.com/component/component_rdx1cp90ys553uwxuckev249x5wezucqru0u4qr7qdxdc9tlpmnh93242k` |
| Master Badge (Owner Badge issuer — mint, recall, invalidate) | Radix Mainnet | `resource_rdx1nt4gugcmzpajreu75g2ul2whcpa48cdyn0h8n8x8zl5c0gstxn8gvd` | `https://dashboard.radixdlt.com/resource/resource_rdx1nt4gugcmzpajreu75g2ul2whcpa48cdyn0h8n8x8zl5c0gstxn8gvd` |
| Owner Badge (governance admin) | Radix Mainnet | `resource_rdx1ng4c5k872hvhr379n0z0x6ht2n0guugns4jeh6mck9y28cu432xvc4` | `https://dashboard.radixdlt.com/resource/resource_rdx1ng4c5k872hvhr379n0z0x6ht2n0guugns4jeh6mck9y28cu432xvc4` |
| Governance package | Radix Mainnet | `package_rdx1p49s2442esdzs7wet7wucpagnftctml8aecc6a74q67r8r023u4dzn` | `https://dashboard.radixdlt.com/package/package_rdx1p49s2442esdzs7wet7wucpagnftctml8aecc6a74q67r8r023u4dzn` |
| Voting-power resource — XRD | Radix Mainnet | `resource_rdx1tknxxxxxxxxxradxrdxxxxxxxxx009923554798xxxxxxxxxradxrd` | `https://dashboard.radixdlt.com/resource/resource_rdx1tknxxxxxxxxxradxrdxxxxxxxxx009923554798xxxxxxxxxradxrd` |
| Recognised Governance Platform | — | `https://vote.radixdao.org/` | Live URL, publicly accessible |
| Official Venue(s) | — | `https://radixdao.org` | Live URL, publicly accessible |
| Compliance Challenge Filing Channel — primary (Governance Operator) | — | `veto@radix.community` | Published to the Official Venue; monitored mailbox, open to any sender |
| Compliance Challenge Filing Channel — copy (RAC) | — | `rac@radix.community` | Published to the Official Venue; monitored mailbox, open to any sender |

**The `veto@` local part is retained deliberately.** The mechanism was renamed (**Proposal & Voting Framework §8**) but the address is already published, and a filer who remembers the former name must still reach a monitored mailbox. Changing it is Routine under §8 if the DAO later prefers to.

**Voting-power sources are not all single resources.** XRD has one fixed resource address across all of Radix Mainnet and is therefore recorded above with its address and a working verification link. **LSUs (Liquid Staking Units) are not a single shared resource:** each validator mints its own distinct LSU resource with its own resource address, so there is no single "LSU address" to record. LSUs are recognised as a *class* of eligible voting power and converted to their XRD-equivalent at the redemption rate at snapshot; their identification is governed by the snapshot methodology (**DAO Parameters §8 and §8A**; **Proposal & Voting Framework §6**), not by a resource entry in this register. The same applies to any other supplementary source (**DAO Parameters §8A**) that is per-validator or per-pool rather than a single resource: where such a source *does* resolve to a single fixed resource address it may be recorded above for convenience; where it does not, it is verified through the snapshot methodology, not this register. XRD and LSU together are the entrenched constitutional floor of eligible voting power (**Charter §12.1 item 4**), whether or not each carries a register entry.

---

## 4. Governance Identifiers — Setup & Use Rules

Each governance identifier is used strictly as provided by the governance framework. This section states the applicable rule by cross-reference; it does not restate the mechanics.

* **Governance component & Owner Badge.** The Owner Badge governs elevation of passed Temperature Checks to Governance Proposals and is operated by the Governance Operator within a non-discretionary mandate (**Delegate Mandate §2.2**). The custody and recovery arrangement for the Owner Badge, chosen at deployment, must permit an elevation or badge rotation to proceed **without the Governance Operator's cooperation**, sufficient to give effect to the elevation and badge-compromise backstop (**Governance Continuity Framework §4.2A**, §7). A deployment lacking this capability does not satisfy the Minimum Operational State.

* **Master Badge.** The Master Badge issues the Owner Badge and can **mint, recall, and invalidate** it. It is therefore the root of governance-infrastructure control rather than a peer of the Owner Badge, and every rule this framework writes about the Owner Badge is capable of being defeated through it: a recalled or invalidated badge disables the elevation pipeline entirely, and a freshly minted one confers elevation authority on a holder bound by no mandate. It is governed accordingly.

  * **Recovery instrument, not an operating credential.** The Master Badge is never used to perform an elevation. Its permitted uses are exhaustive: giving effect to the elevation and badge-compromise backstop (**Governance Continuity Framework §4.2A**); rotating, reissuing, or reclaiming a lost or compromised Owner Badge; and a redeployment or reissue authorised by an approved Governance Proposal.
  * **Custody — the DAO's multi-signature treasury account.** The Master Badge is held in the primary multi-signature treasury account recorded at §5, not by any natural person. It is held by the RAC in its collective capacity and cannot be exercised without a signing quorum, which satisfies the no-single-person requirement. This custody is also what makes the **Governance Continuity Framework §4.2A** backstop operable: that section has the Treasury Signers execute a badge reissue, which they can only do if the badge is reachable from an account they collectively control.
  * **Exercise thresholds.** Ordinary exercise is a protected matter — unanimity of all seated signers, being not fewer than two (**Operating Agreement §9.11**), during the Transition Period, and an approved Governance Proposal of the applicable class from the Activation Date. This is a higher threshold specified for this matter by the ratified framework for the purposes of **Operating Agreement §6.6**, which the framework is competent to set because the ratified policy library forms part of the Charter (**Charter §13**). The sole exception is an exercise under **Governance Continuity Framework §4.2A**, which follows the route and threshold stated there — the backstop must remain reachable when an actor is unavailable or compromised, which a unanimity requirement would defeat.
  * **The line between those two routes is documentary, and is treated as such.** Both are executed by the same signers from the same account, so nothing on-chain distinguishes an ordinary exercise from a backstop exercise — only the record does. An exercise relying on §4.2A is valid only where the published RAC instruction and the elapsed Elevation Backstop Compliance Window are already on the record **before** it occurs. An exercise citing §4.2A without that prior record is a breach of this policy whatever its on-chain form, and is reviewable under the **Emergency & Safeguards Policy §10**. Where the account's access rule can enforce the higher threshold on a badge withdrawal directly, it must be configured to do so; where it cannot, this documentary discipline is the whole of the control, and signers are on notice of that.
  * **Not a treasury asset for emergency purposes.** The Master Badge and the Owner Badge sit in the treasury account but are not treasury assets within the meaning of emergency asset movement: Tier 2 protective movement to the Emergency Safe Address (**Emergency & Safeguards Policy §6**) does not extend to either. Without this exclusion, a Tier 2 action — available at ≥2/3 RAC and 75% approval — would move the root of governance control to an address held under a different arrangement, at a materially lower bar than any rule governing the badge itself.
  * **Disclosure.** Every exercise of the Master Badge is published to the Official Venue within 24 hours, identifying the authority relied on. Because an unexercised badge leaves no on-chain trace, the disclosure record is verifiable against the badge's transaction history: an exercise without a corresponding disclosure is itself detectable.
  * **Minimum Operational State.** A deployment in which the Master Badge is exercisable by a single person, or whose custody and recovery arrangement for the Master Badge is not recorded under §3, does not satisfy the Minimum Operational State (**Governance Continuity Framework §7**).

* **Graded ballot completeness.** Under Majority Judgment a ballot that leaves any candidate ungraded is invalid and is excluded from Participation (**Proposal & Voting Framework §6.2.4, §6.3**). The ballot interface must therefore **reject an incomplete submission at the point of casting**, so that an invalid ballot cannot be cast at all. Without this, honest voter error on a large field reduces measured participation and pushes a round toward quorum failure — a hazard that grows with the number of candidates, which is exactly where Majority Judgment is otherwise most useful. A deployment that accepts incomplete graded ballots does not satisfy the Minimum Operational State.
* **Exact arithmetic in the graded count.** A candidate's qualifying grade is the highest grade at which the voting power graded at or above it **reaches or exceeds** the Grade Quantile of the power cast (**Proposal & Voting Framework §6.2.4**). "Reaches or exceeds" makes exact equality a **passing** case, so the comparison decides seatings precisely at its boundary. It must therefore be evaluated exactly — the quantile held as a rational and the test applied by cross-multiplication over exact decimal values — and never in binary floating point, in which the products involved are not generally representable. The same applies to the majority gauge, where an error in the last place creates or destroys a tie and so changes who is seated. A rounding error here raises no exception and is invisible in the published tallies, which will look internally consistent with the wrong result; nothing downstream would detect it. A deployment that evaluates either comparison in floating point does not satisfy the Minimum Operational State.

* **Reproducible results.** The Grade Quantile in force is fixed by **Proposal & Voting Framework §6.2.4** rather than configured per election, but it can be amended. A deployment must record, against each election, the quantile and the electability floor that applied to it, and must recompute a stored result from those recorded values rather than from the values current at the time of recomputation. Without this an amendment silently changes what an earlier published result recomputes to, and a terminal result ceases to be reproducible (**Elections & Role Governance Policy §7A**).

* **Snapshot handling.** Each vote takes its own snapshot when it opens (**Proposal & Voting Framework §6.1**). The one exception is a **rerun**, which reuses the stored snapshot of the round it re-runs — a Majority Judgment rerun, and a Stage 2 quorum-held-over rerun. The governance component must therefore be capable of opening a vote against a stored snapshot belonging to an earlier round; a deployment without that capability cannot run the rerun provisions as specified. No other vote inherits a snapshot, so no broader capability is required.
* **Voting-power resources.** Eligible voting power is measured at the voting snapshot from the sources defined in **DAO Parameters §8 and §8A**, subject to the entrenched XRD + LSU floor (**Charter §12.1 item 4**). Only single-resource sources (such as XRD) carry a fixed resource address in §3; class-based sources such as LSUs are per-validator and are identified and converted to XRD-equivalent through the snapshot methodology, not through a register address (see the note in §3).
* **Compliance Challenge Filing Channel.** The two addresses recorded in §3 receive Compliance Challenge filings under **Proposal & Voting Framework §8.4**. Both are monitored: the Governance Operator address is the primary recipient and the RAC address is in copy, so that receipt does not depend on any single role holder and a filing directed at the conduct of one is still received by the other. Neither address may be placed behind a sender allowlist, a subscription or registration requirement, or any other filter that would cause a filing from an unknown sender to be rejected, quarantined, or withheld. Filings received are published verbatim to the Official Venue within the Channel Publication Window (**DAO Parameters §4**). The Channel is an interim measure pending a governance filing interface; it is a convenience route, not a gate, because publication to the Official Venue is an independently valid filing route at all times (**Proposal & Voting Framework §8.4**).
* **Security review.** No governance or on-chain system is relied upon before it has been subject to the security-review standard the DAO maintains for smart contracts and on-chain systems it governs (**Charter §9**).

---

## 5. Identifier Register — Treasury

| Function | Network | Identifier | Verify |
|---|---|---|---|
| Primary multi-signature treasury account | Radix Mainnet | `account_rdx1c9l27suy4nte9ymge5c3eqqnnfepgf9p28d9lcsv3jvmd0f0z8j2fx` | `https://dashboard.radixdlt.com/account/account_rdx1c9l27suy4nte9ymge5c3eqqnnfepgf9p28d9lcsv3jvmd0f0z8j2fx` |
| Operational treasury pool (if segmented) | Radix Mainnet | `[account_rdx1… — if established by Governance Proposal]` | `https://dashboard.radixdlt.com/account/[account_rdx1…]` |
| Reserve treasury pool (if segmented) | Radix Mainnet | `[account_rdx1… — if established by Governance Proposal]` | `https://dashboard.radixdlt.com/account/[account_rdx1…]` |
| Grants pool (if segmented) | Radix Mainnet | `[account_rdx1… — if established by Governance Proposal]` | `https://dashboard.radixdlt.com/account/[account_rdx1…]` |
| Emergency Safe Address | Radix Mainnet | `[account_rdx1… — designated per DAO Parameters §6.1]` | `https://dashboard.radixdlt.com/account/[account_rdx1…]` |

---

## 6. Treasury Identifiers — Setup & Use Rules

* **Multi-signature control.** Treasury assets are held in the multi-signature account(s) recorded in §5, under the phase-dependent threshold structure in **DAO Parameters §6.2 and §6A** and **Treasury Signers Operational Rules §10A** — during the Transition Period 2-of-3 for ordinary actions and unanimity of all seated signers (not fewer than two) for protected matters, and from the Activation Date 3-of-5 standard and 4-of-5 high-risk. High-risk transactions correspond to the protected matters in **Operating Agreement §9.12**.
* **Segmentation & account architecture.** Establishing and changing the treasury account architecture is phase-dependent (**Treasury Signers Operational Rules §10A.1**; **DAO Parameters §6.2**): during the Transition Period the Transition RAC establishes and may adjust it by resolution published to the Official Venue under **Operating Agreement §6.5(d)**, settling once the Activation Statement is published so the Permanent RAC inherits a reviewed structure; from the Activation Date it may be changed only by Governance Proposal. Each account remains under multi-signature control on the same threshold structure. A new or changed account is recorded in §5 on establishment.
* **Emergency Safe Address.** The Emergency Safe Address must be designated before the Company receives the principal asset transfer; designation and any later change follow **DAO Parameters §6.1** and the Tier 2 emergency asset-movement rule in **Emergency & Safeguards Policy §6**.
* **Execution discipline.** All movement of treasury assets is subject to the pre-execution hold and irreversible-action controls in **Execution & Treasury Actions Policy §14** and the Compliance Challenge Window in **Proposal & Voting Framework §8**.

---

## 7. Verification

Every identifier recorded in this policy carries a working public verification link. Any Governance Participant may confirm an identifier by opening its link on the Radix Dashboard (`https://dashboard.radixdlt.com`) or an equivalent public explorer and comparing the on-chain entity — component, resource, package, or account — against the value recorded here.

The current register is published to the **Official Venue** and kept accurate. Its public accessibility and accuracy are the evidence supporting **Operating Agreement Schedule 5, condition 5** (the Governance Mechanism, governance contracts, voting mechanism, and Official Venue(s) identified, recorded, and publicly accessible as at the Activation Statement date).

---

## 8. Change & Update Procedure

A change to a recorded identifier is classified by the identifier's significance:

* **Routine.** Recording a newly deployed non-critical identifier, correcting a link, or recording a segmented account already authorised by a passed Governance Proposal — recorded by the Governance Operator or RAC and published to the Official Venue, with the standard 48-hour Compliance Challenge Window (**Proposal & Voting Framework §8**) applying.
* **Governance-critical.** A change to the Governance smart-contract component, the Master Badge, the Owner Badge, a voting-power resource, or the primary treasury account requires an approved Governance Proposal of the applicable class, published to the Official Venue with prior notice, before the change takes effect. Modelled on the RAC source-change discipline in **DAO Parameters §8A**: notice to Governance Participants and the standard Compliance Challenge Window apply.

A change to either **Compliance Challenge Filing Channel** address is **Routine**, and takes effect only on publication of the new address to the Official Venue — an unpublished change is not effective, and a filing sent to the superseded address during the Compliance Challenge Window remains validly filed. This lighter treatment is acceptable because the Channel cannot be used to suppress a filing: publication to the Official Venue is an independently valid filing route at all times (**Proposal & Voting Framework §8.4**), so control of the addresses carries no power to block a challenge.

On any change, the Company updates the record held with the Registered Agent and, to the extent required by section 106(2) or section 107 of the DAO Act, notifies MIDAO and procures an amendment to the Certificate of Formation — a new Certificate or an amendment carrying an updated **Exhibit A** — to reflect the updated identifier (**Operating Agreement §11.4**; **Certificate of Formation clause 10**).

During the Transition Period, identifier recording and changes are made by the Transition RAC by written resolution published to the Official Venue (**Operating Agreement §6.5**); from the Activation Date, authority passes to the standing governance process and the Governance Operator as set out above.

---

## 9. Relationship to Other Documents

This policy operates alongside:

* Operating Agreement (§9.10–§9.12, §11.4, Schedules 2, 4 and 5)
* Charter (§6A, §9, §12.1)
* Proposal & Voting Framework (§8 — Compliance Challenge filing, and the Compliance Challenge Filing Channel recorded in §3)
* Execution & Treasury Actions Policy
* Treasury Signers Operational Rules
* Delegate Mandate
* Emergency & Safeguards Policy
* Governance Continuity Framework
* DAO Parameters Registry

If a conflict arises, the Operating Agreement prevails, followed by the Charter, then approved governance decisions (see **Operating Agreement §11.3**). Nothing in this policy overrides the Operating Agreement or the Charter.

---

## 10. Amendments

_A change to a recorded identifier is made under §8, not by amendment. Amendment of this policy's text follows the **Governance Maintenance & Upgrade Framework §3.2**._
