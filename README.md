# Market Basket Analysis Using Association Rules

## Project Overview

This project aims to perform Market Basket Analysis (MBA) using Association Rules to understand and leverage customer purchase behavior. By identifying patterns in customer browsing sessions, we can make informed recommendations for cross-selling and up-selling products. The insights from this analysis can be utilized in various business strategies, including sales promotions, loyalty programs, and store design.

## Problem Statement

Retailers frequently use Market Basket Analysis to comprehend the purchasing behavior of their customers. This information can be applied to numerous strategies, such as cross-selling, up-selling, sales promotions, loyalty programs, store design, and discount plans.

The project involves evaluating item sets to choose a subset of them for recommendations. The metrics used to measure the significance and interest of rules for recommendations include:

1. **Confidence (conf(A → B))**: Probability of occurrence of B given A.
2. **Lift (lift(A → B))**: Measure of how much more A and B occur together than expected if they were independent.
3. **Conviction (conv(A → B))**: Compares the probability that A appears without B if they were independent with the actual frequency of A without B.


## Methodology

We use the A-priori algorithm, implemented using PySpark and Python, to find frequent itemsets in the browsing sessions dataset. The support is fixed at 100, meaning product pairs must occur together at least 100 times to be considered frequent. We will find item sets for sizes 2 and 3.

## Dataset

The dataset `browsing.txt` contains online browsing sessions. Each line represents a browsing session of a customer, where each string of 8 characters is the ID of an item browsed during that session. Items are separated by spaces, and duplicate items in a session do not affect the results.


