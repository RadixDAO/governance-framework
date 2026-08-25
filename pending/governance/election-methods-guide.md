# Election Methods Guide (Principles)

*A companion to the [Elections & Role Governance Policy](elections-and-role-governance-policy.md) and the [Proposal & Voting Framework](proposal-and-voting-framework.md). This guide is **not** part of the governance framework and has no legal force — if anything here seems to differ from a policy, the policy (and above it, the Charter and Operating Agreement) wins. Its only job is to set out the considerations that bear on choosing between the DAO's two election mechanisms. Nothing here is a requirement, a test, or a condition on anyone's discretion.*

*The binding rules are in the Proposal & Voting Framework §4.5, §6.2.4 and §6.2.5, the Elections & Role Governance Policy §7 and §7A, and the [DAO Parameters Registry](../parameters/dao-parameters-registry.md) §6B. For the framework as a whole, see the [Policy Library Reading Guide](../policy-library-reading-guide.md).*

---

## Why there is a choice at all — and who makes it

**Majority Judgment is the default.** Every election runs under it unless the DAO has resolved otherwise by Governance Process proposal, in force before the Nomination & Discussion Window opens (Elections & Role Governance Policy §7). Two-stage remains fully specified and fully operative; it runs where the DAO has said so.

**Nobody chooses per election.** The RAC does not select a mechanism, and neither does the body running a founding election or a re-run. The only decision this guide informs is a **proposal put to the DAO** — whether to resolve a departure from the default for a role or a class of roles, or to return one to it. If you are reading this in order to administer an election, there is nothing here for you to decide.

Both mechanisms are legitimate and both are fully specified. Neither is a placeholder for the other. But they ask the electorate different questions, and from the same field of candidates they will not always return the same people. That is not a defect — it is the reason having two is worth anything. It is also why a departure deserves a reason, and why that reason is worth writing down and putting to a vote.

---

## What the two mechanisms have in common

Most of an election is the same either way. The choice is narrower than it first appears.

| | Both mechanisms |
|---|---|
| Who may stand | Same eligibility and nomination rules (Policy §5–§6) |
| Getting to a ballot | Same Nomination & Discussion Window, same Temperature Check approving the candidate list |
| Who may vote, with how much weight | Same eligible voting power, same snapshot rule — each vote takes its own snapshot when it opens, and only a rerun reuses the snapshot of the round it re-runs (Framework §6.1) |
| Turnout requirement | Same quorum — Minimum Participation for Elections, 7% |
| If turnout is short | One rerun over a doubled voting period. Two-stage lowers the quorum and raises the approval threshold to compensate; Majority Judgment holds both constant (see principle 4) |
| If seats go unfilled | Same referral to vacancy handling (Policy §11; founding elections §17.1) |
| Candidates who cleared the bar but missed a seat | Same 90-day reserve list (Policy §7.5) |
| Who declares the result | The RAC, under the same publication duty and the same 48-hour Compliance Challenge Window |

*Why this is here:* if you are weighing the two mechanisms, weigh only what actually differs. Nothing in the list above should enter the decision.

---

## The one-line difference

> **Majority Judgment** asks *how good is each of these candidates?* — and seats the ones the electorate broadly rates well.
>
> **Two-stage** asks *who is worth considering?*, then *do you affirmatively back this particular person?* — and seats the ones who clear both.

Underneath that sits the substantive difference. Majority Judgment measures **breadth of acceptability**: a candidate's qualifying grade is high only if three-fifths of the voting power rates them at least that well, so a candidate with passionate backing from a third of the electorate and hostility from the rest will not do well. The two-stage mechanism measures something closer to **intensity of endorsement**: Stage 1 ranks candidates by how much voting power actively approves them, and Stage 2 then asks each shortlisted candidate to clear an individual 60% gate.

Neither measurement is the correct one in the abstract. Which one you want depends on the seat.

---

## How the qualifying grade actually behaves

Read this before principle 4. The framework does **not** run Majority Judgment at the median. It settles each candidate's grade at the **Grade Quantile — three-fifths** of the voting power cast (Framework §6.2.4). Everything else is the textbook mechanism; only the crossing point moves. Where you read "median" in outside commentary on Majority Judgment, read "the grade three-fifths of the power placed the candidate at or above."

**It is not the average.** For a candidate graded 61% Excellent and 39% Poor, the average grade is around Good. The **qualifying grade is Excellent**. Accumulate voting power from the top: Excellent alone reaches 61%, which crosses three-fifths, and the calculation stops there — it never reaches the Poor grades at all.

**It is not the most common grade either.** Take a candidate graded 25% Excellent, 10% Very Good, 20% Good, 15% Acceptable, 30% Poor:

| Grade | Share | Running total | Crossed three-fifths? |
|---|---|---|---|
| Excellent | 25% | 25% | no |
| Very Good | 10% | 35% | no |
| Good | 20% | 55% | no |
| Acceptable | 15% | **70%** | **yes — qualifying grade is Acceptable** |
| Poor | 30% | 100% | *(never reached)* |

Poor is the largest single block at 30% — and it is **irrelevant**. Those voters sit entirely below the crossing, so the calculation never gets to them. "Most voters said Poor, so the candidate is rated Poor" is the natural reading and it is wrong.

*The same field at the median would have returned Good, and Good is the electability floor.* That is the whole effect of the quantile in one example: settling at three-fifths costs this candidate their seat, because a scattered electorate that broadly likes a candidate without concentrating above one grade no longer carries them.

**What actually decides the outcome is the grade sitting at the crossing.** Shifting 10 points from Acceptable to Good in the table above lifts the running total at Good to 65% and the candidate qualifies at Good — seated. The hostile 30% never mattered in either case.

**Voting power decides where the crossing falls.** Power is what positions it, so a large holder can control the result outright. But past the crossing, extra power does nothing: a holder with 60% and a holder with 80% produce the identical qualifying grade. Majority Judgment is *monotonic* in voting power, not *proportional* to it — unlike Stage 1 Approval Voting, where every unit of power keeps moving the ranking.

*Why a quantile at all, given all this:* grades are ranks, not quantities — there is no basis for saying Excellent-to-Very-Good is the same distance as Acceptable-to-Poor, so averaging them assumes a scale the ballot doesn't provide. And an average is trivially gamed: everyone grades their favourite Excellent and every rival Poor, and the election becomes a raw power contest. A quantile blunts that, and blunts it harder the higher it is set. It is a real trade, not a mistake.

*Why three-fifths rather than half:* at the median, a block holding half of turnout fixes every candidate's grade at whatever level it likes. Three-fifths is the same figure as the two-stage confirmation threshold, so the two mechanisms ask a block for the same share of turnout. The reasoning is in Framework §6.2.4 and the consequences are in principle 4.

---

## Principles

These pull in a direction. None of them decides a case on its own, and each has a counter-case worth taking seriously.

### 1. Match the ballot to the question the seat actually asks

Some seats need a person the whole electorate can live with — a mediator, an interpreter of rules, a holder of a swing position on a small body. Breadth of acceptability is the right property, and Majority Judgment measures it directly.

Other seats need someone with a real mandate to act, sometimes against opposition. The two-stage mechanism's per-candidate 60% gate produces exactly that: nobody is seated without a majority of decisive votes affirmatively saying yes to *them*.

*The counter-case:* a seat can need both, and then this principle gives you nothing. Move on to the ones that do discriminate.

### 2. Field size is a real constraint, not a preference

A Majority Judgment ballot is only valid if the voter grades **every** candidate. That is what makes the qualifying grades comparable, and it is a genuine cost: with five nominees it is a few minutes' work, with twenty-five it is a research project, and voters who will not do it simply do not vote. Turnout is not free, and quorum is 7%.

Stage 1 shortlisting exists precisely to solve this. Approval Voting over a large field is cheap for the voter — tick the ones you know — and it cuts the field to twice the number of seats before anyone is asked for a considered per-candidate judgement.

*The rough shape of it:* the larger and less familiar the field, the stronger the case for shortlisting first. A field small enough that an engaged voter could form a view on everyone is a field Majority Judgment can handle.

### 3. Two mechanisms, two very different clocks

Majority Judgment is one voting round, plus a rerun only if turnout falls short. Two-stage is Stage 1, then Stage 2, then possible per-candidate reruns, then fallback advancement of the next Stage 1 candidate — each of which is another vote, and the framework requires reruns to wait until all concurrent Stage 2 votes have closed.

Against the 21-day Replacement Completion Time for a vacancy, that difference is not academic.

*The counter-case:* for a founding election or a high-stakes body, the gap between rounds is where the community actually scrutinises a shortlist that has been narrowed to a serious few. Slowness is sometimes the product.

### 4. The crossing point — the most important thing on this page

**Below the Grade Quantile, Majority Judgment is very hard to capture. At exactly the quantile, it hands over everything.** Both halves of that sentence follow from the same property, and you cannot have one without the other. What the quantile decides is *where* that cliff sits.

*Exactly three-fifths, not three-fifths plus one.* The qualifying grade is the highest grade at which the running total **reaches or exceeds** the quantile (Framework §6.2.4), so a bloc holding precisely three-fifths of the voting power cast already fixes the grade — it does not need one more token.

A qualifying grade is fixed by the ballot standing at the crossing and is completely blind to how extreme the grades on either side of it are. So:

| The electorate | Qualifying grade | Stage 2 outcome |
|---|---|---|
| 61% grade Excellent, 39% grade Poor | **Excellent** — top grade, seated | 61% YES → clears the 60% gate |
| 30% grade Poor, rest spread above | Poor is ignored entirely | 70% YES → confirmed |

In the first row, a candidate that 39% of the DAO rates worst-possible receives the *highest available grade*. Those Poor grades change nothing — they would produce the same result if they were Acceptable, or Good, or Very Good. **This is the property that does not go away at any quantile.** What changed is the price: the block in that row needs three-fifths of turnout, not half, and it is the same share the two-stage gate would demand of it.

**Raising the Minimum Qualifying Grade still does not help.** The floor changes *which grade* the required share must confer; it never changes *what fraction* must agree. Set it to Very Good and a three-fifths block grades Very Good instead. **The dial that changes the fraction is the Grade Quantile, and it is not available per election** — it is fixed at three-fifths in Framework §6.2.4 for every Majority Judgment election, and moving it is an amendment to the counting mechanics, not a parameter change.

Two-stage's 60% per-candidate gate is a share-of-turnout test, and Majority Judgment's quantile now is one too, at the same figure. Note what is *not* the same: two-stage applies its test to each candidate on a separate ballot, so a minority declining one candidate leaves the others untouched. Majority Judgment applies its test on one ballot across the whole field.

**What this costs in practice.** Control belongs to whoever holds three-fifths of *turnout*, not three-fifths of the DAO — and exactly three-fifths is enough. At the 7% election quorum that is roughly **4.2% of eligible voting power** — enough to set every candidate's grade, and because one ballot grades every candidate, to sweep an entire body in a single action. At the median it was 3.5%. The number moved; **the single-action scope did not**, and that is now the real difference between the mechanisms rather than the threshold. Under two-stage the same block must win the Stage 1 ranking *and* clear 60% on each candidate separately, across as many separate votes as there are shortlisted candidates.

**And the trade runs the other way too.** A quantile above half is not symmetric. A block holding more than **two-fifths** of turnout — roughly 2.8% of eligible at quorum — can hold any candidate's grade down to its own level, and grading the whole field Poor leaves nobody above the floor. That is cheaper than obstruction was at the median. A round that meets quorum and seats nobody is **not** a quorum failure (§7A.3): no rerun opens, and the seats go to vacancy handling. The framework accepts this deliberately, because a stalled election is recoverable and a captured body is not.

*The other side, and it is real:* Approval Voting rewards coordination in its own way. A disciplined block that approves exactly its own slate concentrates all its power on those names while unorganised voters spread theirs thin, so a *minority* can dominate a Stage 1 ranking. Stage 2's gate then checks it — but only over the candidates Stage 1 chose to show the electorate.

*And the softer objection, which the quantile sharpens rather than softens:* the same insensitivity that ignores a hostile minority also favours the inoffensive, and a higher crossing rewards concentration more. A scattered electorate that broadly approves a candidate without agreeing on how much carries them less far at three-fifths than at half — dispersion across adjacent grades costs more the higher the crossing sits.

**The practical upshot:** the threshold argument for two-stage has been answered. What remains is the argument from scope — one ballot, one snapshot, the whole body — and it is unaffected by the quantile.

### 5. Think about the record the election leaves behind

A Majority Judgment result is a full grade distribution for every candidate — including the ones who lost, and including the incumbents. That is a genuinely useful artefact: comparable across elections, informative at renewal, and hard to spin. A candidate who was seated on a median of Good with a long tail of Poor grades is visibly in a different position from one seated on a solid Very Good.

A two-stage result gives you a Stage 1 power ranking and a Stage 2 yes/no ratio. Enough to know who won; much less to know what the electorate thought.

*Where this matters most:* roles subject to auto-renewal (Policy §9.1). If a term renews unless challenged, the record from the last election is much of what a participant has to go on when deciding whether to challenge.

### 6. Seat count pulls in the opposite direction to field size

Majority Judgment handles multi-seat elections natively: the qualifying-grade ranking *is* the seating order, so filling five seats is the same operation as filling one, and the awkward case the two-stage mechanism has to handle — more candidates confirmed than there are seats — simply does not arise.

But many seats usually means many nominees, and principle 2 then pulls the other way. Three seats from six nominees is comfortable for Majority Judgment. Three seats from thirty is where the shortlist multiplier earns its keep.

### 7. Weigh the cost of seating the wrong person

The two-stage mechanism puts an explicit, individual veto point on every candidate: a 60% approval gate, per person, with no Abstain to soften it. That is an expensive extra round, and for some seats it is cheap insurance — Treasury Signers holding multisig keys, or any role where removing the wrong occupant is slow and damaging.

Majority Judgment's equivalent protection is the Minimum Qualifying Grade, backed by the Grade Quantile. It is a real bar, and because the quantile is three-fifths it is a supermajority bar — but a *different kind* of bar: it asks whether three-fifths of the power grades the candidate at or above a level, not whether they affirmatively endorse that candidate in a ballot about them alone. The floor itself still cannot be tuned into a share requirement; only the quantile sets the share, and it is fixed for every election.

*The trade:* a per-candidate confirmation gate costs a round and buys a **per-candidate** objection. That is what survives now that the share thresholds match: under two-stage a minority declining one candidate leaves the rest of the field untouched, while a Majority Judgment ballot decides every candidate at once. The difference is no longer how large a block must be — it is how finely its objection can be aimed.

### 8. Consistency beats cleverness

Switching mechanisms between consecutive elections for the same role has costs that are easy to miss. Results stop being comparable, so the record from principle 5 loses much of its value. Candidates cannot know what kind of campaign to run. And the switch itself invites the reading — fairly or not — that the mechanism was chosen for the outcome it would produce.

*In practice:* treat the mechanism used last time for a role as the starting point. Departing from it is entirely legitimate; departing from it **without saying why** is what generates suspicion.

### 9. *When* the choice was made matters as much as what was chosen

The two mechanisms favour different candidates from the same field. It follows that a choice made **before** the nominee field is known is defensible in a way that a choice made after it is known is not — however honest the reasoning behind the later choice, and however good the outcome.

This is not a rule, and the framework does not impose a deadline. It is simply an observation about credibility, and it is cheapest to act on early: name the mechanism when the Nomination & Discussion Window opens, publish the reasons alongside it, and the question never arises. The Temperature Check then gives the community a real say — it is a live vote at 3% quorum, and a failed Temperature Check ends that election outright.

*This applies with most force where the body running the election has an interest in its outcome* — an election for the RAC's own successors, or a founding election run by a Transition RAC that the elected body will replace. There, an early and reasoned choice is worth a great deal, and a late one is worth very little.

### 10. Under Majority Judgment, the Minimum Qualifying Grade is the only dial left

Once you have chosen Majority Judgment, the mechanism is fixed — including the Grade Quantile, which is three-fifths for every election and is not selectable (Framework §6.2.4). The only dial left is the floor a candidate must reach to be seated at all — **Good** as standard, and unchanged on a rerun.

Raising the floor is a statement that an empty seat is safer than a mediocre occupant. That is often true — and it is worth being clear-eyed that "empty" means the seat goes to vacancy handling under Policy §11, which is its own process with its own delay. A high floor is not a free stringency.

**What the floor cannot do** is change the share. Following principle 4, a block that meets the quantile chooses the grade, so raising the floor costs it nothing while burdening a genuine broad electorate. That is exactly why the floor is *not* raised on a rerun, and why the rerun's quorum is *not* lowered: swapping a lower turnout bar for a higher grade bar looks like a fair trade and isn't one. The instrument that sets the share is the quantile, and the DAO has already set it.

**And note which way the floor now leans.** Because grades are settled at three-fifths rather than at half, every candidate's qualifying grade is weakly lower than the same ballots would have produced at the median. A floor of Good is therefore a stiffer test than the same word implied before — it now means three-fifths of the voting power placed the candidate at Good or better.

**That stiffening was chosen, not inherited.** Lowering the floor to Acceptable, to hold the effective bar where it sat at the median, was considered and declined. These are the seats where an unfilled seat is the safer failure, so the higher bar is the intended effect. Read the floor against the quantile — and read it knowing the DAO already did, and kept Good.

*A related point worth internalising:* a Majority Judgment round that meets quorum but seats nobody has **not** failed. The electorate answered, and the answer was that none of these candidates should hold the seat. That is a real result, and it does not trigger a rerun.

---

## Side by side

| | Majority Judgment | Two-Stage Approval → Confirmation |
|---|---|---|
| **The ballot** | Grade every candidate: Excellent / Very Good / Good / Acceptable / Poor. Partial ballots invalid | Stage 1: approve any number of nominees. Stage 2: yes/no on each shortlisted candidate |
| **Rounds** | One, plus a rerun only if turnout is short | Two, plus possible per-candidate reruns and fallback advancement |
| **What wins** | Highest qualifying grade at the three-fifths quantile, subject to the Minimum Qualifying Grade floor | Top by approval power into the shortlist, then ≥60% yes individually |
| **Seating order** | The qualifying-grade ranking is the seating order | Stage 2 confirms eligibility; Stage 1 power ranking orders the seating |
| **Measures** | Breadth of acceptability | Intensity of endorsement, per candidate |
| **Main weakness** | Scope, not threshold: three-fifths of turnout (~4.2% of eligible) controls every grade and can sweep a whole body in **one ballot**, and more than two-fifths can hold the entire field below the floor | Stage 1 rewards block coordination; more rounds, more elapsed time |
| **If turnout falls short** | One rerun at the same quorum and floor, doubled period; or the RAC restarts under two-stage | Per-candidate rerun at reduced quorum and raised threshold |
| **Can candidates be fewer than seats?** | Yes — the floor supplies the possibility of losing | Yes — unfilled seats go to vacancy handling |
| **Voter effort** | High and fixed — every candidate, every ballot | Low at Stage 1, moderate at Stage 2 over a shortlist |
| **Record it leaves** | Full grade distribution per candidate | Approval ranking plus a yes/no ratio |
| **Suits** | Small to moderate fields; seats needing broad acceptability; multi-seat bodies; elections you want an evidence trail from | Large or unfamiliar fields; seats needing an individual mandate; roles where seating the wrong person is expensive |

---

## Where a departure is worth proposing

The default answers every case below. This table is about which of them are worth putting to the DAO anyway — it recommends nothing, and none of it binds.

| Seat | Is a departure worth proposing? | The argument |
|---|---|---|
| Permanent RAC | **The strongest case, and it is about scope alone** | The body that publishes results, adjudicates ties, and issues binding interpretations. Not a threshold argument — three-fifths of turnout either way — but every seat is decided by one ballot on one snapshot, where two-stage spreads the same decision across 1 + 2×seats separate votes with separate snapshots (Framework §6.1) |
| Treasury Signers | **A real case** | Multisig keys. The per-candidate gate is a per-candidate *objection*: a minority declining one signer leaves the rest untouched |
| Working Group Stewards | No | Smaller fields, lower stakes, and the grade record is genuinely useful at renewal |
| Strategic Coordination WG | No | As above |
| Filling a single vacancy | No | One round inside the 21-day Replacement Completion Time, and with one seat the scope argument does not arise at all |
| A field of 20+ nominees | **Worth considering** | Grading everyone is a research project and turnout is what pays for it — but this is a property of a particular election, and a resolution must be in force before nominations open, so it is hard to reach in time. A standing resolution for a role that reliably draws large fields is the practical form |

**Two arguments for two-stage have expired; one has not.** Earlier versions of this guide routed the Permanent RAC and Treasury Signers to two-stage because Majority Judgment could be captured more cheaply, and because it offered no supermajority protection. The Grade Quantile answered both: grades settle at three-fifths, the same share as the Stage 2 gate, and it cannot be tuned per election.

What survives is narrower and worth stating precisely. It is not that Majority Judgment is easier to capture — it is that **the same block, at the same cost, gets more for its money**: one ballot decides an entire body, where two-stage makes it win each seat separately, in public, over weeks, against an electorate that can see the earlier results. And a minority's objection under two-stage can be aimed at one candidate without touching the field.

That is a real argument and the DAO may act on it by resolution. It is no longer an argument that Majority Judgment is the weaker mechanism.

---

## Where the binding rules actually are

| Question | Look here |
|---|---|
| The election pipeline, and both mechanisms in outline | [Proposal & Voting Framework](proposal-and-voting-framework.md) §4.5 |
| The Temperature Check as candidate-list approval | Proposal & Voting Framework §3.2 |
| Majority Judgment mechanics — grades, the Grade Quantile, qualifying grades, ties, reruns | Proposal & Voting Framework §6.2.4 |
| Two-stage mechanics | Proposal & Voting Framework §6.2.2, §6.2.5, §6.2.7 |
| Voting power and the snapshot | Proposal & Voting Framework §6.1 |
| Participation and denominators for graded ballots | Proposal & Voting Framework §6.3 |
| How the RAC determines and publishes a result | Proposal & Voting Framework §6.5 |
| Election process, both mechanisms | [Elections & Role Governance Policy](elections-and-role-governance-policy.md) §7 (two-stage: §7.1–§7.3; Majority Judgment: §7A) |
| Reserve list | Elections & Role Governance Policy §7.5 |
| Unfilled seats and vacancies | Elections & Role Governance Policy §11; founding elections §17.1 |
| Term renewal and challenges | Elections & Role Governance Policy §9 |
| Every number named above | [DAO Parameters Registry](../parameters/dao-parameters-registry.md) §3.5, §6B |
| Why elections sit outside the continuity fallback | DAO Parameters Registry §9A |
