---
title: "eToro Machine Learning Portfolio"
date: 2018-01-29
tags:
  - Trading
---

# Project Overview

![eToro](https://steemit-production-imageproxy-upload.s3.amazonaws.com/DQmQu927Ej6CW9mamZfZGj5z6kA1rXruJW2JQt5vtKqsrSb)

eToro is a social trading investment network that enables users to watch the financial trading activities of other users, 
copy them, and make their own trades **using CFDs**. eToro allows traders to  learn from each other, share live trading 
information, and capitalize on their collective power. 

Users can also view the portfolio allocation and performances of other traders and choose who to "copy"

![Copy](/Users/jasonchan/PycharmProjects/jasonchanhku.github.io/assets/new_images/copypeople.png)

With so many traders to learn and "copy" from, how does one make the decision to copy and how much should one allocate?

The motivation for this project is the answer to the question above. The projects aims to apply machine learning to
data that can be scraped from the platform and re-balance the portfolio frequently to achieve the ***optimum eToro portfolio.*** 

## Caveats

Below are some of the caveat that needs to be acknowledged as it may have significant impact to the project:
* eToro allows traders to invest in stocks using **CFDs**
* This means there are **overnight fees** associated with holding positions overnight
* The [full overnights fees](https://www.etoro.com/en/customer-service/fees/) needs to be researched

# Implementation

There are two ways the implementation of the can play out:
* Make this into a clustering problem and segment the "outstanding" traders to copy from at least for the week/month using the predictors below
* Make this into an unsupervised learning problem where copy selection is done to autoencode a performance of a good index/underlying


## Potential Features

These are the potential features identified from availability on the platform:
* returns (1m, 3m, 6m, 1y)
* portfolio allocation 
* volatility
* sharpe ratio
* risk rating
* trades per week
* active since
* profitable weeks
* average holding time  

## Process

The following are the high level steps for implementation:

* Scrape the data from eToro using **selenium and scrapy**
* Cleanse and blend any useful data available
* Collect results in an organized way and visualize them
* Machine learn from predictors to determine the optimum copying portfolio 
* Backtest the strategy and evaluate the outcome

# Outcome and Results

The outcome and effectiveness of this project can be tested using **virtual equity** of a $100,000 using the new machine learning
portfolio strategy. Over a period of 1 - 3 months, the effectiveness can be gauged and measured.

