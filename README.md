# Sowellian Governance

One of my favourite quotes on decision making comes from Thomas Sowell  
“It is hard to imagine a more stupid or more dangerous way of making decisions than by putting those decisions in the hands of people who pay no price for being wrong.”

Sowellian Governance aims to put this philosophy into practice. By using a novel betting mechanism for governance, organizations can align decisions and outcomes with skin in the game. If the decision is a good one, supporters get rewarded. If it is a bad one, they pay a price for being wrong.

Taking a page from Robin Hanson’s Futarchy model, Voters decide the top-level strategy and values of the organization, creating a rigid frame for tactical operations that get decided through betting.

________________

## Core Principles

These Core Principles are what have helped guide the creation of this new system. Each one can be directly mapped to an element in the governance process.

1. Those who make decisions must pay for mistakes.  
All signaling is done through betting. If an idea has the most bets in its favor, the idea is implemented and, upon evaluation, the bet is resolved.

2. Every organization has KPIs and proposals must target them. “Vote on values”  
The most effective way to evaluate the result of a proposal is to objectively measure the outcome. Organizations vote on their values by selecting which KPIs are part of the proposal process. This ensures focus and alignment.

3. Proposers should compete to surface valuable ideas. Bettors should compete to support them. “Proposing with Purpose”  
This is exemplified through the use of a time-weighted stake. The earlier your bet, the higher your reward (if correct). Proposers are defacto the earliest bet and enjoy the highest share of the rewards. This motivates proposers to be the first to share a good idea and bettors to be the first to support or oppose them.

4. Voters stake once to express belief. “Bet on beliefs”  
To best ensure skin in the game, Sowellian governance requires that the bet is held until the outcome is evaluated. If it didn’t, there would be no risk for people to support a poor idea. Results matter and impact those that make the decision.

5. Change should always leave the organization better off  
This makes governance sustainable and prevents spam. Every proposal brings revenue to the treasury; either in the form of a proposal bond for missing quorum or in the form of a 1% rake from the losing bets.

## Voting on Values

Decentralized organizations are often plagued by obtuse policies and perverse incentives. Sowellian Governance ensures that the first step is establishing the following through vote:

- KPIs - what can proposals target as an outcome; this is tied back to values  
  This can be market cap, revenue, user growth, etc. They all share the following criteria.  
  * Objective (on-chain or externally verifiable)  
  * Time-bounded (clear start and end points)  
  * Binary or quantitative (e.g. “+10% users in 3 months”)

- Proposal settings - what criteria must be met to pass a proposal  
  This is betting time, evaluation time, proposal bond amount, quorum, etc..

- Asset Flows - how do we use our assets between elections; where does money flow  
  This is allowances, redemptions/dissolutions, community budgets and grants, taxes, protocol fees, etc..

- Elections - who directs us; which person/people have authority to make tactical decisions; how/when do we vote  
  This is the executive branch, the team, the president, etc…

### Example 1: A decentralized short-term hedge fund

Throughout the whitepaper, we refer to this as “Trading Group”. The treasury is 1 million. The below are the voted values.

- KPI: treasury value increases.  
- Proposal settings: 1 day betting time; 1 week evaluation, bond 1% of quorum, quorum 1% of treasury value, maximum 10% of treasury can be used in one proposal  
- Asset flows: Entire treasury is in the budget. Executive team receives 5% of profit at the end. Dissolution of the exec team after 3 months.  
- Elections: Executive team handles trades that cannot be executed programmatically. Elections need a 51% quorum at any time.

### Example 2: A fishing village

Throughout the whitepaper, we refer to this as “Village”. The population is 1000. The treasury is 10000 gold coins. The below are the voted values

- KPI: increase population  
- Proposal settings: 1 week betting time; 1 year evaluation, bond 1% of quorum, quorum is 10% of treasury value, 10% of citizens betting.  
- Asset flows: Tribe manages 20% of treasury as yearly budget. Tribe leader manages 50% of revenue from fish sales tax. Fish sales tax of 30%  
- Elections: Tribe leader. Elections with 65% quorum once a year.

## Proposing with Purpose

Anyone can create a proposal by selecting the KPI they are targeting, their idea, and submitting a bet (this is the “proposal bond” which is a fixed amount)

- Trading Group: “We should exchange 10% of the USD in our treasury into Bitcoin” - the KPI here would be treasury value going up; the bond is 1000$ (based off of the values voted on). In this quorum, the group requires 10,000$ worth of bets to participate in the betting. If not, the proposal bond is forfeited to the treasury  
- Village: “We should have a lower fish sales tax for families of 5 or more” - the KPI is to increase the population; the bond is 10 gold coins (based off of the values voted on). In this quorum, there is an additional requirement; the tribe requires 10% of the citizens to participate in the betting. If not, the proposal bond is forfeited to the treasury

## Betting on Beliefs

Once a proposal is live, the community places bets to show support or opposition to the idea. A bet cannot be withdrawn, but participants can add more than 1 bet during the betting time.

Payouts are calculated based on how much money has been bet on the opposing side; the earlier you bet, the larger your pro-rata portion of the winnings.

This means that proposals that are highly contentious have the highest return for supporters, and proposals that are highly supported have the highest return for opposers

If by the end of the betting time there are more YES bets than NO bets, the proposal moves to Evaluation and is considered passing.

If there are less YES bets than NO bets, the proposal fails and all bets are off

If the quorum is not met, the first bet (proposal bond) is forfeited and sent to the treasury

- Trading Group: Most think that the proposal “We should exchange 10% of our USD in treasury into Bitcoin” is a good idea and the proposal passes with 90% YES bets and 10% 10% NO bets, with a total exceeding the required quorum. 10% of the treasury is used to purchase Bitcoin. In 1 week, an oracle will be used to see if the decision was a good one and resolve the bets.  

- Village: The proposal “We should have a lower fish sales tax for families of 5 or more” is highly contested, and the proposal passes with 55% YES bets and 45 % NO bets, with more than 10% of the citizens participating to meet quorum. The new tax break is put into effect and the bet will be resolved in 1 year with the new Village census data.

## Observing Outcomes

Bets are settled after a proposal's KPIs are measured by their relevant oracle. An oracle is a “source of truth” that can be considered reliably objective. In the absence of an oracle for a KPI, the organization can default to its elected group to decide the outcomes of proposals.

If the outcome of the proposal has been achieved; the YES bets win the NO bets money. If the outcome of the proposal has not been achieved; the NO bets win the YES bets money.

In both instances; 1% of the loser’s money goes to the treasury

The payouts are calculated based on the amount in the bet and how long the bet was held; they are paid out immediately after the outcome has been confirmed.

- Trading Group: The price of Bitcoin went down after buying it 1 week ago. The No bets win the Yes bets’ money.  
- Village: The census data shows growth of 25% more than last year, with families citing the tax break as a major incentive to growing their families. The Yes bets win the No bets money.

## References

* Sowell, The Vision of the Anointed  
* Sowell, Knowledge and Decisions  
* Hanson, Futarchy: Vote Values, But Bet Beliefs  
* Hanson, The Age of Em
