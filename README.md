# Bank Telemarketing Optimizaation
This project analyzes a dataset related with direct marketing campaigns of a Portuguese banking institution. The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required, in order to access if the product (bank term deposit) would be ('yes') or not ('no') subscribed.

Dataset source: UCI Machine Learning Repo Bank Marketing
https://archive.ics.uci.edu/dataset/222/bank+marketing

## Problem Statement
Telemarketing campaigns often suffers from low conversion rates and high operational costs due to uninterested leads. Contacting every customer in the database also might be not an effective approce with the limited resources. There is a need to identify the profile of custommer who likely to subscribe to the product.

## Objective
To predict whether a client will subscribe to a term deposit. By identifying several indicators, this project aims to:
- Increase conversion rate, by focusing marketing efforts on high probability lead.
- Optimize resource allocation, reduce the number of unnecessary calls or low probability client, so it can lowering the operational cost.
- Understand which factors that most significantly influence client decision

## Insights from EDA
### Overall Conversion Rate
![Overall Campaign Conversion Rate](overall-conversion-rate.png)
There is a significant rejection rate of 88.3% compared to 11.7% conversion rate which suggest that the current calling strategy is still inefficient. This indicates a clear need a more targeted client, data driven approach  rather than contacting every client from the database.

### Annual Account Balance Distribution
![Account Balance Distribution](account-balance-distribution.png)
Clients who chose to subscribe the offer have a higher median balance compared to those who rejected it. It indicates that clients with high liquidity tend to prefer using deposits.

### Conversion Rate based on Number of Calls
![Conversion Rate vs Nummber of Calls](conversion-rate-on-attempt.png)
Conversion rates reached the peak at the first contact, remain stable through the second and third attempts before decreasing significantly in subsequent calls. It suggest that a threshold of three attempts per campaign should be more effective to prevent customer fatigue. p.s the maximum 6 attemps in this graph is the result of capping to reduce the outliers. 

### Client Demographic Distributon
![Client Age Distributon](client-age-dist-and-subs.png)
The campaign primarily reaches clients in the 30–40 age bracket, representing the highest volume of contacts. However, this demographic also yields the highest rejection.
![Client Job Distribution](conversion-rate-by-job.png)
From the occupation, students and retired clients show the highest conversion rates compared to others. This can be an indication that groups with specific financial life stages are a good target for this product.
![Client Education](conversion-rate-based-education.png)
Clients with tertiary education demonstrate a higher conversion rate compared to others. This might suggest that higher financial literacy or more stable professional income levels contribute to decision making for long term investment. 

From this three indicators, while high education levels positively correlate with higher conversion rates, this effect still influenced by client's life stage. The 30-40 age group, despite being well-educated, they often faces the middle-age financial squeeze that might override their will to save. But, for the student and retired segments, they represent high-conversion due to lower debt or loan burdens and probably have more specific financial goals.

The assumption of loan burdens indicated in this graph below where client that has housing loan and/or personal loan tend to reject the subscription. 
![Client Education](conversion-rate-based-on-load.png)








