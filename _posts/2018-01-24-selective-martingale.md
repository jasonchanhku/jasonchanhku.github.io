---
title: "Selective Martingale Betting in Sic-Bo (大小)"
date: 2018-01-24
tags:
  - Gambling
---

# Project Introduction

![Sic_Bo](http://www.casinoreviewsquad.com/wp-content/uploads/2011/06/sicbolit.jpg)

This project was inspired by a past project where I developed a Martingale
betting strategy to ensure profits in the long term of betting **Big or Small.** 

However, the downside of that strategy was that one must have infinite wealth to avoid bankruptcy
as there is only so much of consecutive wrong bets one can get.

The downside of this strategy hence creates the need of a more selective and cautious strategy which is
***less volatile in terms of profit fluctuations.***



## Rules

This strategy is only interested in betting in either **Big or Small.** The other bets such as odd, even, etc are
irrelevant in this project. 

The following are the ground rules for betting on either **Big or Small:**
* Big: total of 3 dices must be 11-17 
* Small: total of 3 dices must be 4-10
* Any triples will be considered as a loss
* Payout is 1 to 1, i.e. you win what you bet
* Minimum bet is HKD 200            


## Betting Facts

The following betting facts are acknowledged for this betting project:

| Outcome       | Probability   | House Edge  |
| ------------- |:---------------:| :----:|
| Big      | 48.6% | 2.8% |
| Small      | 48.6%      |   2.8% |
| Triples | 2.8%      |   13.9%  |

## Betting Strategy

The **Selective Martingale** strategy works as follows:
* Say we pick Big, do not bet Big until Small appears ***X*** consecutive times
* If we do not win, apply Martingale ***until profit is gained***
* If or until we win, hold the profits until the next ***X*** appearances of Big or Small occur
again and then bet the opposite outcome

For example, if X = 4,

`B,B,B,B -> Bet S -> wait until S,S,S,S -> Bet B`

### Optimum Value of X

The optimum value of X will be a trade-off between profit likelihood and occurrences. For instance, if we set X = 10,
we might not be able to have a high chance of profit on the next bet, but for Big/Small to occur 10 consecutive times,
it is unlikely and much less frequent.

Given the trade-off explained above, the expected profit can only be calculated using Monte-Carlo simulation of ***N*** trials.

### Assumptions and Constraints

* The dice outcome is random and unbiased
* Casino systems are fair and not rigged
* Finite wealth of HKD 3,000

Note that with only 3,000 in hand, 4 losses is the maximum consecutive losses before bankruptcy. 

# Implementation

## Skills Needed

## Logistics

## Time to completion

