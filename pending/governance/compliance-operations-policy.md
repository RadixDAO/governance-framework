# Compliance Operations Policy

| Field | Value |
|---|---|
| **Version** | v1.0.0 |
| **Last updated** | 2026-08-25 |

---

## 1. Purpose

This policy defines the operational practice through which Delegates and the Compliance Liaison implement the Company's compliance obligations. It is subordinate to the **Operating Agreement** and the **Charter**, which contain the structural and statutory compliance framework.

The scope of this policy is:

* Operational UBO monitoring and KYC procedures (§2)
* Operational security for role-holder identity and credentials (§3, §4)
* Regulatory demand disclosure protocol for Delegates (§5)

Statutory obligations themselves — including BOIR filing schedules, KYC requirements, UBO identification thresholds, and non-distribution exceptions — are set out in the Operating Agreement (Article III and Article X) and are not restated here.

---

## 2. UBO Monitoring and KYC Operations

The 25% UBO statutory test, the BOIR filing obligation, and the KYC requirement are defined in **Operating Agreement §10.2, §10.1, and §10.4** (Article X). This section sets out the operational procedures by which those obligations are met, including the KYC tier structure.

### 2.1 Threshold Monitoring

The Permanent RAC (or Transition RAC during the Transition Period) is responsible for monitoring on-chain voting power distribution to identify Governance Participants approaching the 25% UBO threshold. When any wallet or coordinated entity approaches the threshold, the RAC must:

* Initiate outreach to the affected holder
* Notify the Compliance Liaison to prepare for KYC onboarding
* Record the outreach in the RAC's quarterly accountability report

### 2.2 KYC Onboarding Procedure

A Governance Participant reaching the 25% UBO threshold must, within 14 days of crossing the threshold:

* Notify the Compliance Liaison
* Complete KYC verification through the DAO's designated KYC provider
* Provide: full legal name, date of birth, residential address, non-expired passport number, and associated wallet address(es)

The Compliance Liaison maintains UBO KYC records confidentially with the Registered Agent in accordance with Marshall Islands law.

### 2.3 Confidentiality

UBO records are maintained confidentially with the Registered Agent and are not published to the DAO community, consistent with Marshall Islands law. The existence of a UBO relationship and the fact of KYC completion may be disclosed as required by law.

### 2.4 Non-Compliance Consequences

Failure to complete required KYC upon crossing the 25% threshold may result in:

* Suspension of voting rights associated with the affected holdings, pending compliance (§2.4A)
* Referral to legal authorities as required by applicable law
* Civil and criminal penalties under Marshall Islands law (up to USD 500/day civil penalty; up to USD 10,000 criminal fine; up to 2 years imprisonment; possible entity revocation)

### 2.4A Suspension of Voting Rights

The RAC may suspend the voting rights attaching to holdings whose holder has not satisfied a KYC, beneficial-owner identification, or BOIR reporting requirement applicable to that holder under Marshall Islands law and **Operating Agreement Article X** (§10.1, §10.2, §10.4).

A suspension under this section:

* is made by RAC decision at the emergency decision threshold (**DAO Parameters §5.2**), recording the statutory requirement relied on;
* requires prior written notice to the holder and a cure period of **14 days** from that notice;
* extends only to the holdings of the non-compliant holder, and to no voting power source (**Charter §12.1** item 4);
* takes effect on publication to the Official Venue, without disclosure of information held confidentially under §2.3;
* lapses on the holder satisfying the requirement, or on its being established that the requirement did not apply; and
* is subject to the Compliance Challenge (**Proposal & Voting Framework §8**) and to escalation under the **Dispute Resolution & Arbitration Policy**.

A suspension determines who may vote; it does not change how eligible voting power is measured.

This section is the only ground on which voting power recognised under **Proposal & Voting Framework §6.1** may be set aside.

### 2.5 Continuity of the Compliance Liaison Role

If the Compliance Liaison role is vacant or the holder is incapacitated, the RAC must declare a continuity event under the **Governance Continuity Framework** and appoint a temporary replacement subject to GP ratification within 30 days.

---

## 3. Identity and Confidentiality of Role-Holders

Role-holder identities — including Members, Delegates, RAC members, and Treasury Signers — are **publicly disclosed** as part of the election and appointment process, in accordance with the **Elections & Role Governance Policy**.

The following operational details may remain confidential:

* Key management and custody procedures
* Security protocols and infrastructure details
* Specific custody provider arrangements

Such confidentiality is permitted solely for:

* Operational security (OpSec)
* Legal compliance

Identities themselves may not be kept private on the basis of these exceptions.

---

## 4. Credential and Web2 Asset Security

Persons managing the Company's Web2 assets and credentials must:

* Securely manage Web2 credentials using an enterprise password manager
* Use controlled access systems with audit logging
* Maintain recovery procedures for credential loss or compromise

**Recovery independence.** Recovery access to the credential store, and to the domain registrar and platform accounts holding the Company's Web2 assets, must be capable of being exercised **without the cooperation of the person holding the credentials**. No individual may hold sole recovery access. The arrangement is held by the RAC and recorded in the confidential implementation record maintained under **Operating Agreement §9.13**, and is verified at each key rotation review (**DAO Parameters §6A**), the fact of verification being reported to the Official Venue. Repository access is additionally governed by the **Source Code Stewardship Policy §3.2**.

Individuals managing credentials may be subject to KYC where required by their Delegated Function. Credential management responsibilities are assigned through the Web2 Custodian Delegated Function (Delegate Mandate §2.5; delegated functions are established under Operating Agreement §11.5).

---

## 5. Regulatory Demand Disclosure Protocol

Any Delegate or RAC member who receives a legal demand, order, or regulatory inquiry that (a) relates to their role, or (b) would require action inconsistent with a DAO-approved decision, must:

1. **Notify the RAC within 24 hours of receipt**, unless legally prohibited by the demand itself.
2. **If prohibited from disclosing the content of the demand**, notify the RAC that they are under a legal constraint preventing disclosure, without revealing the nature of the constraint.
3. **Refrain from taking any action under the demand** until the RAC and, where time permits, the community have been notified and DAO-authorized legal counsel consulted.

Upon receiving such notification, the RAC immediately escalates to the Governance & Legal Working Group (where operational) and publishes a community notice to the governance forum within 48 hours.

This protocol applies regardless of the jurisdiction from which the demand originates. Each Delegate's primary legal obligation in their Company capacity is to the laws of the Republic of the Marshall Islands and the Operating Agreement (per the Delegate Mandate and the standard of conduct in Operating Agreement §12.7(d)). Where a foreign jurisdiction demand conflicts with this, Delegates and RAC members are expected to seek DAO-authorized legal counsel before compliance and to treat DAO authorization as a condition of compliance where legally possible under Marshall Islands law. This obligation does not prevent a Delegate or RAC member from taking protective action necessary to avoid criminal liability, provided they notify the RAC immediately.

**Demands received at the Registered Agent.** Where a legal demand, service of process, or regulatory correspondence is received at the Registered Agent's address, the Compliance Liaison must forward it to the Delegates and publish notice of receipt to the Official Venue within **48 hours of the Compliance Liaison becoming aware of it**, in addition to this protocol. This forwarding-and-disclosure obligation gives operational effect to the DAO's notices-and-service framework in **Charter §14** and is an operational compliance duty under this policy (under Operating Agreement §11.5).

---

## 6. Cross-References

The following topics are defined in the documents listed and are not restated here:

| Topic | Document |
|---|---|
| Legal entity structure, governing law, formation | Operating Agreement Article II |
| Non-distribution principle and permitted payments | Operating Agreement §§3.4–3.5 |
| Membership and Governance Participation (binding effect post-activation §5.7; advisory §§5.8–5.9) | Operating Agreement Article IV and Article V |
| Delegated Functions, indemnification | Operating Agreement §11.5 (see Delegate Mandate), §12.5 |
| BOIR filing obligation, KYC requirement | Operating Agreement §10.1, §10.4 |
| Transition Period and Transition RAC mandate | Operating Agreement Article VI |
| Treasury custody, multisig thresholds, key management | Operating Agreement §§9.7–9.11; Treasury Signers Rules §10, §16 |
| Asset lock and wind-down | Operating Agreement Article XIII; Charter §11 |
| Continuity statement authority | Operating Agreement §9.3 |
| Governing law and dispute resolution | Operating Agreement Article XIV |
| Notices and service framework (constitutional anchor for §5) | Charter §14 |

---

## 7. Amendments

Amendment procedures and classification requirements are defined in the **Governance Maintenance & Upgrade Framework**.
