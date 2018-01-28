---
title: "Selective Martingale Betting in Sic-Bo (大小)"
date: 2018-01-24
tags:
  - Gambling
---

# Project Overview

![Sic_Bo](http://www.casinoreviewsquad.com/wp-content/uploads/2011/06/sicbolit.jpg)

This project was inspired by a [past project](http://nbviewer.jupyter.org/github/jasonchanhku/jupyternotebooks/blob/master/Macau%20%E5%A4%A7%E5%B0%8F%20simulation.ipynb) where I developed a Martingale
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
we might be able to have a high chance of profit on the next bet, but for Big/Small to occur 10 consecutive times,
it is unlikely and much less frequent.

Given the trade-off explained above, the expected profit can only be calculated using Monte-Carlo simulation of ***N*** trials.

## Assumptions and Constraints

* The dice outcome is random and unbiased
* Casino systems are fair and not rigged
* Finite wealth of HKD 3,000

Note that with only 3,000 in hand, 4 losses is the maximum consecutive losses before bankruptcy. 

# Implementation

A python script will be written implement the ***Selective Martingale*** betting strategy in a Macau casino. Based on my last visit,
these are some of my observations that could be key to the implementation:
* There are 4 tables playing Sic-Bo
* A screen is present on each table with the historical of Big/Small outcomes

Based on the 2 observations above, I do not have to just wait at a particular table for ***X*** consecutive outcomes but rather
jump from one table to another shall ***X*** consecutive outcomes occur at any table. 


## Process

The following are the high level steps to implement the betting strategy:
* Write simulation function
* Write and code out betting strategy
* Collect results in an organized way and visualize them
* Tune for optimum parameters value ***X***
* Evaluate if optimum ***X*** makes sense in the real scenario

# Outcome and Results

The outcome and effectiveness of this strategy and be tested by making a trip to Macau with the assumptions stated in hand. 
Regardless of the outcome, I will update the blog with my results.

