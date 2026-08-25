# Radix DAO Delegate Mandate

| Field | Value |
|---|---|
| **Version** | v1.0.0 |
| **Last updated** | 2026-08-25 |

> **Scope of this document.** This Mandate is the primary definition of the **Delegates** of the
> Company and the **Delegated Functions** they perform — the DAO's operational execution roles.
> It sits alongside the **RAC Mandate**, which governs the DAO's governance-process oversight body.
> The Delegated Functions are operational and delegated functions established under **Operating
> Agreement §11.5**. They confer legal Membership and beneficial-owner status; the legal force of
> those consequences is located in the **Charter** (§4.2, Membership attachment) and the **Operating
> Agreement** (delegated functions §11.5, indemnification §12.5, the DAO Act §109 standard-of-conduct
> disclaimer in §12.7, and beneficial-owner reporting under Article X). This Mandate defines the roles
> and their operational rules; the legal instruments give them legal effect.

## 1. Purpose

Delegates perform the Company's defined operational functions on behalf of the DAO. They are
**execution agents, not decision-makers**: their authority is limited to carrying out validly
authorized decisions of the Company and to the specific operational scope of the Delegated Function
they hold. Under the Operating Agreement, binding community governance outcomes take legal effect from
the **Activation Date** (**Operating Agreement §5.7**); during the **Advisory Governance Period** the
Company is **member-managed** and authorized decisions are made by the Transition RAC within its
formation mandate (**Operating Agreement Article VI**), while community governance outcomes are
advisory (**§§5.8–5.9**).

The Company is member-managed during the Transition Period and becomes Algorithmically Governed on the
Activation Date (**Operating Agreement §§8.1, 8.8**), after which binding governance authority is
exercised by Governance Participants through the Governance Mechanism. In neither phase do Delegates
govern — they execute.

---

## 2. The Delegated Functions

There are five Delegated Functions. Each is defined below by its scope and authority; the detailed
operational procedure for each lives in the specialized policy cross-referenced under the function.

A single Delegate may hold more than one Delegated Function where the combination does not create a
structural conflict; the safeguards for specific combinations are governed by the **Conflict of
Interest Policy §3.5** (Delegated Function Consolidation). For the role-concentration cap in **DAO
Parameters §6B**, a Delegate counts as **one seat** regardless of how many functions the Delegate
holds.

### 2.1 Treasury Signing

Execute treasury transactions via the multi-signature account. Treasury Signers may only sign
transactions authorized by a Governance Proposal or falling within a budget previously approved by
Governance Proposal. In an emergency, Treasury Signers may act to preserve assets or services,
subject to Governance Proposal ratification within the period specified in the **Emergency &
Safeguards Policy §10**.

The Treasury Signing function must be held by **exactly five Delegates** to support the signing
thresholds in **DAO Parameters §6A** (3-of-5 standard; 4-of-5 high-risk). Those five seats are
ordinarily allocated in full from among seated RAC members; where the DAO or, before the Activation
Date, the Transition RAC has designated one or more of them as **elected seats**, the balance is
allocated and the remainder filled by election under §3.1–§3.2. The comprehensive operational rules —
refusal grounds, custody standards, availability, emergency actions, and breach of duty — are defined
in the **Treasury Signers Rules**.

### 2.2 Governance Operations

Operate the Governance smart contract: elevate approved Temperature Checks to Governance Proposals
via the Owner Badge; update governance parameters per Governance Proposal; maintain the Governance
smart contract. The Governance Operator may not elevate a Temperature Check that has not met the
approval conditions, and may not modify, delay, or suppress an eligible elevation without a
Governance Proposal authorizing the deviation. Elevation and proposal-administration procedure is
defined in the **Proposal & Voting Framework**. The Governance Operator must elevate an eligible
passed Temperature Check within the TC Elevation Window (**DAO Parameters §3.1**) or record
documented grounds for the delay with the RAC; an eligible TC left unelevated beyond that window
triggers the elevation backstop in the **Governance Continuity Framework §4.2A**. The custody and
recovery arrangement for the Owner Badge is determined at deployment of the Governance smart
contract and recorded in the **On-Chain Identifiers & Verification Policy §3** (per **Operating Agreement §11.4 / Schedule 4**);
whatever arrangement is chosen must enable an elevation or badge rotation to proceed without the
Governance Operator's cooperation, sufficient to give effect to that backstop.

**Compliance Challenge Filing Channel.** The Governance Operator holds the primary Compliance Challenge Filing Channel address
recorded in the **On-Chain Identifiers & Verification Policy §3**, monitors it, and publishes every
filing received verbatim to the Official Venue with its receipt timestamp within the Channel
Publication Window (**DAO Parameters §4**). The Governance Operator may not filter, withhold, delay,
or edit a filing. Failure to publish does not invalidate the filing (**Proposal & Voting Framework
§8.4**) and is a breach of the standard of conduct in §4. Where the Governance Operator is unavailable, or is the
subject of a filing, the RAC publishes from the copy address.

### 2.3 Legal Signatory

Sign contracts, continuity statements, and other legal instruments on behalf of the Company, only as
authorized by Governance Proposal. Act as the Company's legal representative for entity maintenance
and compliance filings. Initiate, pursue, settle, or defend legal proceedings as authorized by
Governance Proposal; or, in urgent circumstances where a delay of more than 48 hours would cause
material and irreversible harm to the Company, take protective legal action subject to Governance
Proposal ratification within 30 days. Regulatory-demand handling is governed by the **Compliance
Operations Policy §5**. The Legal Signatory Delegated Function is the Legal Signatory recognised in
**Operating Agreement §1.15 and §9.2**, and acts only within the authority conferred by the Operating
Agreement, the Charter, and a valid governance decision.

### 2.4 Compliance Liaison

Act as Registered Agent liaison; file the annual Beneficial Owner Information Report (BOIR);
coordinate KYC for Delegates, RAC members, and UBO Governance Participants; maintain KYC and
sanctions records in accordance with applicable law; and maintain the Company's good standing with
the Registered Agent. UBO identification, threshold monitoring, BOIR onboarding, and confidentiality
procedures are defined in the **Compliance Operations Policy §2**.

**The Compliance Liaison is not the verifier of their own compliance.** The Compliance Liaison may not
verify their own KYC, record their own sanctions screening, or act in any compliance matter in which
they are the subject. Where the Compliance Liaison is unavailable, or is the subject of such a matter,
the RAC coordinates the verification, record, or filing directly with the Registered Agent and the
Company's designated KYC provider, and discloses that it has done so to the Official Venue. Records
created under this paragraph are held on the same confidential basis as any other (**Compliance
Operations Policy §2, §3**).

### 2.5 Web2 Custodian

Manage social media accounts, source-code repositories, domain names, and other Web2 assets using an
enterprise password manager. The Web2 Custodian may not transfer domain ownership or delete
repositories without a Governance Proposal. Credential and Web2 asset security standards are defined
in the **Compliance Operations Policy §4**; repository access standards are defined in the **Source
Code Stewardship Policy §3.2**.

**Recovery must not depend on the Custodian.** Recovery access to the credential store, and to the
domain registrar and platform accounts holding the Company's Web2 assets, must be arranged so that
recovery and re-assignment can proceed **without the Web2 Custodian's cooperation**. No individual may
hold sole recovery access. The arrangement is established before the Custodian assumes the function,
is held by the RAC, and is recorded in the confidential implementation record maintained under
**Operating Agreement §9.13**; it is verified at each key rotation review (**DAO Parameters §6A**) and
the fact of verification reported to the Official Venue.

---

## 3. Composition & Seating

**Delegated Functions are seated by allocation by the RAC, not by separate election, unless the DAO or
the Transition RAC has provided otherwise for a particular function or seat under §3.1 or §3.2.** The RAC decides
which of its seated members is best fit for each function and publishes the allocation, with its
reasons, to the Official Venue (**Charter §3.2**; **RAC Mandate §6**). The RAC may re-allocate a
function at any time, publishing the change and its reasons in the same way.

* **Who may hold a function.** Only a **seated RAC member** may hold an allocated Delegated Function.
  There are two exceptions, and only two. An interim Treasury Signer appointed from the **Emergency
  Signer Reserve** under the **Governance Continuity Framework §4.2** need not hold a RAC seat, and
  serves only for the maximum interim period stated there (**Treasury Signers Rules §15**). A holder
  of an **elected seat** under the switching bullet below, §3.1 or §3.2 need not hold a RAC seat, and
  holds for the term they were elected to.
* **How long a function lasts.** An allocated Delegated Function **runs with the holder's RAC seat**.
  It has no term, renewal cycle, or challenge window of its own: it begins on allocation and ends on
  the earliest of re-allocation by the RAC, removal under **Elections & Role Governance Policy §10**,
  and the holder ceasing to be seated. **Elections & Role Governance Policy §8 (Term Lengths)** and
  **§9 (Term Renewal)** therefore do not run separately for an allocated function.
* **The community's lever.** Because a function cannot outlive the seat, a challenge to the holder's
  RAC seat under **Elections & Role Governance Policy §9.2** reaches every function allocated to
  them, as does removal under §10. No separate function-level challenge exists or is needed.
* **Switching to election.** The DAO may resolve by **Governance Process proposal** that a Delegated
  Function be filled by Election Proposal instead of by allocation. For Treasury Signing, which is
  held by five Delegates, a resolution operates **seat by seat**: it states how many of the five seats
  are elected seats, and the balance continue to be allocated (§3.1). For every other Delegated
  Function, a resolution converts the function as a whole. While such a resolution is in force, **Elections & Role Governance Policy §§5–7** govern each
  elected seat, a holder elected to it may be a person who holds no RAC seat, and that seat carries
  its own term under §8 and its own renewal cycle under §9. This section is displaced to that extent
  and otherwise continues to apply.
* **Treasury Signing.** The Treasury Signing roster must comprise **exactly five** Delegates at all
  times, to support the signing thresholds in **DAO Parameters §6A** (3-of-5 standard; 4-of-5
  high-risk). The five seats are **allocated seats** and **elected seats**: the number of allocated
  seats is five minus the number of elected seats, and the default number of elected seats is
  **zero** (§3.1). Where there are no elected seats and the RAC is at its minimum of five seated
  members, all five hold Treasury Signing.
* **Function coverage.** Governance Operations, Legal Signatory, Compliance Liaison and Web2 Custodian
  are each held by **one** Delegate. Every Delegated Function must be held at all times. Where a
  function or Treasury Signing seat is unheld, the RAC re-allocates it without delay; where it cannot,
  §3.3 applies.
* **KYC.** All holders are subject to KYC verification before assuming their function (**Operating
  Agreement §10.4**).
* **Role concentration and conflicts.** Holding a Delegated Function alongside a RAC seat is the
  framework's expected model at small scale. It is **not of itself a material conflict of interest**
  (**Conflict of Interest Policy §5.1**); case-specific conflicts are disclosed and recused in the
  ordinary way. For the role-concentration limit in **DAO Parameters §6B**, a RAC seat and a Delegate
  seat count as two roles, however many Delegated Functions the Delegate holds — so a RAC member
  holding any Delegated Function is at the cap and may not also hold a Working Group Steward or
  Strategic Coordination WG seat.

> **A consequence worth stating plainly.** Under this model the body that verifies execution is drawn
> from the same people who execute, and at minimum RAC strength they are the same people. That is a
> deliberate choice for a DAO of this size, made in preference to leaving execution roles unfilled.
> The safeguards that remain are the published allocation, the RAC's own accountability under the
> **RAC Mandate**, removal and challenge under the **Elections & Role Governance Policy**, and the
> DAO's power to switch any function or seat to election at any time under this section and §3.1.

---

### 3.1 Elected Treasury Signing Seats

The default number of elected Treasury Signing seats is **zero**. The roster is allocated in full from
among seated RAC members unless the DAO has resolved otherwise under the switching bullet in §3, a
seat has converted under the conversion duty below, or the Transition RAC has designated an elected
seat under §3.2.

**Setting the number.** After the Activation Date the number is set by Governance Process proposal,
which must state the number of elected seats and the date from which it applies. Before the Activation
Date it is set by the Transition RAC under §3.2. The number may be raised or lowered by the same route
that set it, and a resolution reducing it to zero returns the roster to allocation in full.

**When a change takes effect.** A resolution altering the number of elected seats does not of itself
unseat anyone.

* Where the number **increases**, the RAC identifies which allocated seats are affected and publishes
  them with its reasons. The allocated holders continue to hold those seats until the elected holders
  are seated, and the RAC may not re-allocate an affected seat in the meantime except under the
  **Governance Continuity Framework §4.2**.
* Where the number **decreases**, a sitting elected holder serves out the term they were elected to,
  and the seat becomes an allocated seat on that term's expiry.

**Where the RAC cannot allocate a seat**, §3.3 applies.

---

### 3.2 Initial Composition of the Treasury Signing Roster

The composition of the Treasury Signing roster that takes effect on the **Activation Date** is
established by the Transition RAC as part of its mandate to establish the treasury, custody and signer
framework (**Operating Agreement §6.5(d)**) and to coordinate the constitution of the Permanent RAC
and the post-transition governance framework (**§6.5(g)**). The Transition RAC may designate one or
more of the five seats as **elected seats**.

Where it does so:

* the holder of each elected seat is identified by a **recognised community advisory outcome** at the
  recognition threshold in **DAO Parameters §3A.3**, conducted under the eligibility, nomination and
  candidacy requirements in **Elections & Role Governance Policy §§5–6**;
* the person so identified is **seated by Transition RAC resolution** published to the Official Venue,
  and holds the seat from the Activation Date;
* seating is subject to KYC verification (**Operating Agreement §10.4**) and to every other condition
  precedent for the function; and
* the designation and the seating must both complete **before the Activation Statement is published**
  (**Operating Agreement §8.5**; **Treasury Signers Rules §10A.1**).

The community outcome is advisory and the seating is the Transition RAC's own act, the binding
community acts of the Advisory Governance Period being limited to the three in **Charter §4A.2**
(**Operating Agreement §5.8(b)**). An elected seat established under this section carries its own term
from the Activation Date under **Elections & Role Governance Policy §8** and its own renewal cycle
under §9.

Where the Transition RAC designates no elected seat, the roster passes to the Permanent RAC allocated
in full, and elected seats may arise afterwards only under §3.1 or §3.3.

---

### 3.3 Conversion Where the RAC Cannot Allocate

This section applies to every Delegated Function and, for Treasury Signing, to each allocated seat.

Where the RAC cannot fill a function or allocated seat from among its seated members — because no
seated member is eligible, willing, or able to hold it, or because a seated member is suspended under
**Elections & Role Governance Policy §10.3**, permanently recused, or otherwise unable to act in it —
the RAC **must** publish a certificate to the Official Venue identifying the function or seat and
stating the reason. On publication:

* the function or seat becomes an **elected seat**, and the RAC opens an election for it within the
  **Replacement Election Trigger Time** (**DAO Parameters §6B**); and
* interim coverage until the elected holder is seated is provided under the **Governance Continuity
  Framework §4**, and for Treasury Signing from the **Emergency Signer Reserve** (**Treasury Signers
  Rules §15**).

Conversion is mandatory. For Treasury Signing, the RAC may not decline it on the ground that the
remaining holders can meet the signing thresholds. A function or seat converted under this section
reverts to allocation on expiry of the elected term, unless a resolution under §3 or §3.1 provides
otherwise.

---

## 4. Standard of Conduct

Delegates shall act in good faith with diligence, accountability, and transparency. Delegates shall
disclose conflicts of interest and recuse themselves from decisions where a material conflict exists,
in accordance with the **Conflict of Interest Policy**.

**Primary law obligation.** In performing their Delegated Function, each Delegate's primary legal
obligation is to the laws of the Republic of the Marshall Islands and the Operating Agreement. Where
a Delegate receives a demand, order, or regulatory inquiry from a foreign jurisdiction that conflicts
with a DAO-approved decision or with the Operating Agreement, the Delegate shall seek DAO-authorized
legal counsel before compliance and, where legally possible under Marshall Islands law, treat DAO
authorization as a condition of compliance. This does not prevent a Delegate from taking protective
action necessary to avoid criminal liability, provided they notify the RAC immediately in accordance
with the Regulatory Demand Disclosure Protocol in the **Compliance Operations Policy §5**.

The fiduciary-duty standard and disclaimer applicable to Delegates (adopted under §109 of the Marshall
Islands DAO Act 2022) is set in **Operating Agreement §12.7** and is not restated
here; this Mandate states obligations of conduct within each Delegate's assigned function and does not
create any fiduciary duty beyond what the Operating Agreement provides. Delegates are Covered Persons
for the purposes of Operating Agreement §12.7 and the indemnification in §12.5.

---

## 5. Removal & Replacement

* Any Delegate may be removed by Governance Proposal at any time.
* **How a function is refilled depends on how it was seated.**
  * An **allocated** function left unheld — because its holder was removed from it, resigned it, or
    ceased to be seated — is refilled by **RAC re-allocation** under §3. It does not go to a
    replacement election, and **Elections & Role Governance Policy §11** reaches it only through the
    underlying RAC seat (**Elections & Role Governance Policy §2**). Where the RAC cannot re-allocate
    a Treasury Signing seat from among its seated members, the conversion duty in §3.3 applies.
  * An **elected** seat left unheld is refilled by **replacement election** under **Elections & Role
    Governance Policy §11**, on the trigger and completion times in **DAO Parameters §6B**. Where a
    reserve list for that seat is in effect under **Elections & Role Governance Policy §7.5** and the vacancy did not arise through removal,
    the reserve list is offered first in the ordinary way.
* Where a vacancy creates an immediate operational risk (for example, Treasury Signers falling below
  execution quorum), the **Governance Continuity Framework §4.2** governs interim coverage and
  prevails over this section. Interim appointments made under it are subject to the conditions stated
  there and terminate automatically on the seating of a successor.

**Legal Signatory continuity.** If the Legal Signatory is unavailable, conflicted, or unresponsive
for more than 24 hours in circumstances requiring time-critical legal action, the Compliance Liaison
is authorised to act as interim Legal Signatory for protective or time-critical purposes only. Any
action taken under this provision must be disclosed to the governance forum within 24 hours and is
subject to Governance Proposal ratification within 30 days.

**Compliance Liaison continuity.** If the Compliance Liaison is unavailable, conflicted, or
unresponsive for more than 24 hours in circumstances requiring a time-critical filing or regulatory
response, the Legal Signatory is authorised to act as interim Compliance Liaison for that purpose
only, on the same disclosure and ratification conditions. Where neither Delegate is available, or
where both are the subject of the matter, the RAC acts directly with the Registered Agent under §2.4.

**Web2 Custodian continuity.** If the Web2 Custodian is unavailable, unresponsive, or removed, the RAC
invokes the recovery arrangement under §2.5 and appoints an interim holder pending re-allocation under
§3 or conversion under §3.3. Invocation must be disclosed to the Official Venue within 24 hours.

---

## 6. Membership & Legal Status

Upon seating and following the Transition Period, Delegates are admitted to legal Membership of the
Company. Membership is attached to the Delegated Functions under the **Charter** and given legal
effect by the **Operating Agreement**; this Mandate does not itself confer Membership. Where the
Delegate also holds a Permanent RAC seat — which under §3 is the ordinary case — Membership attaches
to that seat in any event (**RAC Mandate §7**; **Operating Agreement §§4.3, 4.6**).

Delegates qualify as beneficial owners of the Company by virtue of actual control (Marshall Islands
DAO Act §702(r)) and are reportable on the BOIR regardless of where their function is defined. BOIR
identification, KYC tiers, and sanctions screening are governed by the **Operating Agreement**
compliance article and the **Compliance Operations Policy**.

**During the Transition Period, all five Delegated Functions are held by the Transition RAC
collectively.** There is no separate Delegate roster before the Activation Date: the three Transition
RAC members named in **Operating Agreement Schedule 1** hold every function in §2, and the body acts
in respect of each of them under the simple-majority-of-seated decision rule in **Operating Agreement
§6.6**. This gives effect to **Charter §12.2**, which proceeds on the basis that the Delegated
Functions are held by the Transition RAC during that period. Article VI-specific procedures prevail
over the corresponding procedures in this Mandate during the Transition Period.

* **Treasury Signing.** The three Transition RAC members act as the initial signers (**2-of-3**
  standard; protected/high-risk matters require **unanimity of all seated signers, being not fewer
  than two**) as set out in **Operating Agreement Article VI and §§9.10–9.11**. The
  **exactly-five-Delegates** requirement and the 3-of-5 / 4-of-5 thresholds in §3 take effect on the
  Activation Date, when Treasury Signing passes to the five Delegates then holding it. Which of those
  five seats are allocated and which are elected is established by the Transition RAC under §3.2
  before the Activation Statement is published; where it designates none, all five pass to the
  Permanent RAC as allocated seats.
* **Governance Operations.** The Transition RAC holds the Owner Badge collectively. Because elevation
  is a **non-discretionary** duty under §2.2 and must complete inside the TC Elevation Window (**DAO
  Parameters §3.1**), the body shall adopt a standing resolution, published to the Official Venue,
  authorising **any seated member to execute an eligible elevation ministerially** without a further
  decision. The body retains the decision itself: only the Transition RAC acting under §6.6 may
  record documented grounds for delaying an elevation. The Owner Badge and the standing resolution
  are recorded in the **On-Chain Identifiers & Verification Policy §3**.
* **The remaining functions.** Legal Signatory, Compliance Liaison and Web2 Custodian are likewise
  held by the body and exercised under §6.6, subject to the Article VI mandate limits in **Operating
  Agreement §§6.5 and 6.7**.

> **Known limitation, accepted.** During the Transition Period the Governance Operator, the RAC that
> would instruct it, and the Treasury Signers who would execute a backstop elevation are the same
> three people, so the elevation backstop in **Governance Continuity Framework §4.2A** has no
> independent actor in it. The same is true of the signer-failure response in §4.2. This is accepted
> as a consequence of a three-person formation body rather than remedied, and is carried by the
> publication duties in §2.2 and **Elections & Role Governance Policy §17.2** and by the advisory
> recognition route in **DAO Parameters §3A.3**.

---

## 7. Relationship to the DAO

Delegates operate **on behalf of the DAO** and remain fully subordinate to:

* Governance Participant authority exercised through the Governance Mechanism — advisory during the
  Advisory Governance Period and binding from the Activation Date (**Operating Agreement §§5.7–5.9**);
* approved governance processes; and
* the Charter, the Operating Agreement, and this Mandate.

A Delegate may not exercise authority outside the operational scope of their Delegated Function, and
may not expand that authority of their own accord. Indemnification for the good-faith performance of
a Delegated Function is provided under the **Operating Agreement**.

---

## 8. Amendments

This Mandate is an operational policy and may be amended by Governance Process Proposal. Amendment
procedures, classification, and document versioning are defined in the **Governance Maintenance &
Upgrade Framework**.
