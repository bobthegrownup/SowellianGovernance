# Sowellian Governance v5



> *"There are no solutions. There are only trade-offs." - Thomas Sowell*



## Abstract

Sowellian Governance is a system for decentralized and autonomous organizations that ties every proposal to measurable outcomes, enforces accountability through economic skin-in-the-game, and grows organizational treasuries through modest fees.

Organizations vote on their collective values, proposers risk bonds, voters bet once to express belief, and outcomes are settled against pre-defined Key Performance Indicators.

The system is designed to align incentives, reward foresight, punish mistakes, and strengthen organizations over time.

## Guiding Principles

- Organizations need clear KPIs to map proposals to.

- Those who make decisions must pay for mistakes.

- Proposers compete to surface valuable ideas.

- Voters stake once to express belief.

- Change should always leave the organization better off.

- Reputation is a metric best measured through participation over time.

## Mechanism Overview

> *"Vote on values, bet on beliefs." - Robin Hanson*

Organizations vote on their values and their council. Proposals are crafted selecting organization specific KPIs. Proposers must stake bonds when they make proposals. Participants take “Sowellian Bets” on binary YES/NO markets around proposals. If there are more bets supporting YES and stake quorum is met by the end of the betting window, the proposal passes. The losing side forfeits their bets to the winning side and the proposer receives 2x (their incentive to propose). Treasury grows from a flat 1% fee on betting activity.

## KPIs as DNA

“ Tell me your KPIs and I’ll know your purpose” - Dean Pappas

At inception, each organization defines its KPI DNA: the set of essential metrics that capture organizational performance.

This catalog is created and amended by token-vote, and each KPI is tied to oracle sources.

Every proposal must specify which KPI it targets and what improvement it expects by the end of the evaluation period.

Examples of KPIs would be

Treasury Value

Market cap

Number of Users

Transactions

Page Views

## Proposal Creation and Quorum

A proposal requires a bond. This is how we can satisfy the principles that create skin in the game and an incentive for people to propose.

The proposal bond is counted as the first yes bet. If the the proposal passes and the KPI I achieved, this bet settles with a 2x ROI compared to other bets

Proposals can be crowdsourced and the 2x ROI is shared accordingly

Proposals must meet 2 criteria to pass

Stake Quorum is met (this is the minimum threshold of bets that need to be made. For example, if a stake quorum is set to $1000, the combined value of YES and NO bets must be greater or equal to $1000)

There is more YES value than NO value

Quorum is how an organization prevents spam and malicious proposals

If a proposal does not reach Stake Quorum by the end of the “Betting Window”, the bond is forfeited and sent to the treasury

Bond threshold: 0.5–1.5% of quorum stake. The bond cannot be less than or greater than this range

Bond threshold rationale: The proposer bond is capped at 1.5% of quorum to protect voter incentives. If a proposer is extremely bullish on their proposal, they can add additional funds through a standard YES bet. This increases their exposure, but without the special proposer multiplier reserved for proposers.

Proposal contents: action, KPI targeted, expected improvement.

For Example: Swap treasury USDC for BTC, targeting treasury value, expecting a 5% increase in USD value

"It is hard to imagine a more stupid or more dangerous way of making decisions than by putting those decisions in the hands of people who pay no price for being wrong." - Thomas Sowell

## Betting (Voting)

Betting is made simple with a straight-forward Yes or No bet. The proposal passes if the stake quorum is met before the end of the “Betting Window”

Binary YES/NO staking.

One-way door: once a stake is placed, it cannot be withdrawn or switched.

Participants may add additional stake to their side (YES or NO) at any time during the betting window, but cannot reduce or move an existing stake.

Stakes lock until the end of the evaluation window.

## Settlement & Treasury

> *"The first lesson of economics is scarcity: There is never enough of anything to satisfy all those who want it. The first lesson of politics is to disregard the first lesson of economics." - Thomas Sowell*

No quorum: If Stake Quorum is not achieved, the proposer bond is forfeited and sent to the treasury .

Quorum achieved, NO wins: all bets and the proposer bond are refunded; treasury receives nothing, the proposal does not move forward.

Proposal passes:

Losers’ stake transfers to winners upon completion of the evaluation window

Treasury = 1% of losers to winners transfer.

Remaining 99% split between proposer and voters.



### Formula

```math

T = \tau \cdot L

```



- **T** = Treasury revenue

- **τ** = Treasury rake (default 1%)

- **L** = Loser stake (total losing side)

## Incentives

We guarantee incentives to ensure a simple understanding of why someone should propose or vote.

Voters

Always earn a positive ROI if on the winning side.

ROI increases with contention (tighter 51/49 votes give higher returns).

ROI is floor-guaranteed at +0.5% even in near-consensus cases (89–90%).

Proposers

Earn exactly 2× the voter ROI when their proposal passes with a positive outcome.

Bond is capped (0.5–1.5% of quorum) so they can’t drain voter upside.

If quorum is missed, the entire bond goes to treasury, ensuring skin-in-the-game.



### Voter ROI Formula

```math

R_v = \frac{(1-\tau)\,L}{W + 2B}

```



- **Rᵥ** = voter ROI (fractional; ×100 for %)

- **W** = total winner stake

- **L** = total loser stake

- **B** = proposer bond (0.5–1.5% of quorum)



### Proposer ROI Formula

```math

R_p = 2 \cdot R_v

```



- **Rₚ** = proposer ROI (fractional; ×100 for %)

- Applies only when **YES** wins

## Council

> *"Democracy is a process by which people are free to choose the wrong man." - Thomas Sowell*

The council acts as a referee for maintaining integrity and protecting the organization from bad actors and faulty oracle results.

Verifies KPI oracle results.

Has override power if oracles fail or contradict.

Council elections and parameters set by token-vote

Council members can be recalled

## Parameters

The Sowellian Governance Parameters allow organizations to fine tune their decision making processes to address different governance styles and proposal types. This is an area that requires further testing and iteration as more organizations adopt Sowellian Governance

- Stake Quorum (suggested to be marketcap or treasury size related)

- Bond threshold (suggested to be derived from Stake Quorum)

- Minimum Bet Amount

- Betting Window

- Evaluation Window

- Election Cycle/KPI Setting

- Incentive Guarantees

- Treasury Rake (suggested at 1%)



**Defaults:**

- **Stake Quorum** = 0.5% of org marketcap (snapshotted at proposal creation).

- **Bond Threshold** = 0.5–1.5% of quorum.

- **Minimum Bet** = org-defined, suggested ≥ 0.1% of quorum.

- **Betting Window** = 7 days.

- **Evaluation Window** = 90 days (3 months).

- **Election Cycle / KPI Setting** = 1 year.

- **Incentive Guarantees** = Voter floor (+0.5%) and Proposer double (2×).

- **Treasury Rake** = 1%.

## Execution

The execution of on-chain instructions happen upon resolution of a proposal. In instances where the execution requires off-chain functions, the proposer is expected to oversee the execution of those functions.

If the execution of the proposal has not started by the end of the evaluation window, the outcome is determined as failed, with the YES bets losing.

## Appendix A: Charts

- Charts

- Voter vs Proposer ROI across contention

- Treasury revenue across contention

## Appendix B: Terms in Sowellian Governance

- A list of novel concepts in Sowellian Governance

- Sowellian Bet - A bet on which proposal is best. The bet determines the proposal result, and it settles after the outcome has been determined.

- Stake Quorum - A quorum determined by the total capital staked in the betting market.

- Bond Cap - The maximum proposer bond (1.5% of quorum), set to protect voter incentives.

- KPI DNA - The catalog of KPIs that are essential for an organization to track and govern toward. Established and amended by token-vote.

- Treasury Rake/Loser’s Transfer - A fixed 1% fee taken from the losers → winners transfer whenever a proposal passes.

- Voter ROI Floor - Guarantee that even at high contention (89–90% YES), voters earn a minimum +0.5% ROI if correct.

- Proposer Multiplier - The proposer’s ROI is always set at 2× the voter ROI, rewarding initiative and risk-taking.

- One-Way Door Voting - Once a stake is placed, it cannot be withdrawn or switched. Voters may add more stake to their chosen side, but never reduce or move existing stake. This prevents manipulation and ensures skin-in-the-game.

## Appendix C: Future Extensions

There are some ideas that are not fully formed, but need to be shared for further discussion and exploration

- Wallet Quorum - A quorum determined by the number of unique wallets participating in the betting market. This is to protect against sybil attacks and flash whales

- Wallet Eligibility Filter - Only wallets that have previously voted with at least 0.1% of quorum stake are counted toward the wallet quorum

- Supermajority Bypass - If a proposal receives >90% YES support, it skips evaluation and is immediately settled as successful.

- Reputation - Use past performance on proposal outcome to determine a different return or use reputation as a filter for functionality
