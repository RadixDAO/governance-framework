# Radix DAO — Governance Documents

This repository contains the operative governance documents of **Radix DAO LLC**, a Non-Profit Decentralized Autonomous Organization registered under Marshall Islands law.

Everything in this repository is either currently in force or under active consideration for adoption. Nothing here is a draft or historical record — that material is maintained in the [reference library](https://github.com/Shadaffy/radix-dao).

---

## Current status

**No documents are yet operative.** Under the Operating Agreement the framework is adopted and activated through a **sequence** of community acts, not a single founding vote:

1. **GP-PRE-1 — Constitutional Ratification** (pre-formation): the community ratifies the Charter and policy library.
2. **Formation**: the Transition RAC files the Certificate of Formation and Operating Agreement; the Company is **member-managed** and governance is **advisory**.
3. **GP-ELECT-1 — Permanent RAC Election** (Activation Condition 7).
4. **GP-ACTIVATE-1 — Activation Vote**: the Company becomes Algorithmically Governed and governance outcomes become binding.

See the [`pending/`](pending/) folder for the full framework and the proposal sequence. The table below will reflect the operative framework once the Activation Vote passes.

---

## Operative documents

*This section will be populated once GP-PRE-1 passes.*

| Document | Category | Adopted by | Effective date |
|---|---|---|---|
| — | — | — | — |

---

## Under consideration

| Proposal | Status | Documents |
|---|---|---|
| [GP-PRE-1: Constitutional Ratification of the Governance Framework](pending/GP-PRE-1-Framework-Ratification.md) | Ready for review | [View pending documents →](pending/) |
| GP-ELECT-1: Permanent RAC Election | Not yet drafted | [pending/](pending/) |
| GP-ACTIVATE-1: Activation Vote | Not yet drafted | [pending/](pending/) |

---

## Governance history

See [PROPOSALS.md](PROPOSALS.md) for the full record of proposals, what each one activated or amended, and when.

---

## Reading guides (companion, non-operative)

For readers approaching the framework for the first time, three plain-language companion guides explain the **purpose** of each document in non-legal terms, and the reasoning behind one choice the framework leaves open. They are **not** part of the governance framework, are not ratified by GP-PRE-1, and have no legal force — where a guide and an operative document differ, the operative document prevails. The authoritative document list lives in [`pending/README.md`](pending/README.md).

- [Charter Reading Guide](pending/constitutional/charter-reading-guide.md) — why each section of the Charter exists.
- [Policy Library Reading Guide](pending/policy-library-reading-guide.md) — a one-line purpose for every policy and framework.
- [Election Methods Guide](pending/governance/election-methods-guide.md) — the considerations bearing on the choice between the two election mechanisms.

---

## Document precedence

When two documents conflict, the following order applies (highest to lowest):

1. Marshall Islands law and the Certificate of Formation
2. Operating Agreement — the Company's primary legal instrument
3. Charter — governance constitution; subordinate to the OA but prevails over all operational policies
4. Operational policies (governance policies) — subordinate to both the OA and the Charter
5. DAO Parameters Registry — within the operational policy tier

*Note: This is the OA-first hierarchy established by Operating Agreement §11.3 and restated in Charter §13. The Operating Agreement is the legally registered instrument and prevails over the Charter; the Charter and all operational policies derive their legal force from the recognition given to them in the Operating Agreement. Where an operational policy conflicts with the Charter or the OA, it is void to the extent of the conflict. See Governance Maintenance & Upgrade Framework §3.1 for the full conflict-resolution rules.*

---

## Repository structure

| Path | Contents |
|---|---|
| `constitutional/`, `governance/`, `legal/`, `parameters/` | The **active** governance document set — the `.md` source of every document currently in force. Empty until GP-PRE-1 passes. |
| `signed/` | The signed, hashed PDF of each document in the active set. One PDF per active document. |
| `pending/` | Documents under development or in a proposal cycle, in the same category subfolders. |
| `pending/signed/` | The signed, hashed PDFs produced for a pending proposal, once its documents are versioned and executed. Empty until then. |
| `archive/` | Superseded signed PDFs — the prior version of any document that has since been renewed. |
| `PROPOSALS.md` | The governance history: every proposal and the documents it affected. |

### Document lifecycle

1. **Drafting.** Documents for a proposal are placed in `pending/`, in their category subfolder. No PDFs exist yet, so `pending/signed/` is empty.
2. **On passage.** Each document in the proposal is versioned, rendered to PDF, signed, and hashed. The PDFs are placed in `pending/signed/` and their SHA-256 hashes are recorded in the proposal's manifest.
3. **Promotion.** The `.md` sources move to the matching root category folders and the PDFs move to `signed/`. They are now the active governance document set. The `pending/` folders are left empty (with a `.gitkeep`) and are ready for the next proposal cycle.
4. **Renewal.** When an active document is amended by a later proposal, its previous signed PDF moves to `archive/`, and the new `.md` source and its new signed PDF take its place in the root folders and `signed/`.

---

## About this repository

This repository is updated only when a governance proposal passes. Each merge to `main` corresponds to a DAO vote. The commit history is the governance audit trail.

For the complete reference library — including working drafts, templates, analysis materials, and the full activation roadmap — see the [Radix DAO reference repository](https://github.com/Shadaffy/radix-dao).
