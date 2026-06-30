# Practical-Application-3
Bank Term Deposit; Classifiers - Berkeley ML-AI - June 29, 2026, by Timothy Vermette

# Prediciting whether customers will subscribe to a bank term deposit

## Link to Jupyter Notebook on GitHub

## Overview
The objective is to analyze approximately 5 years worth of phone marketing campaign data from a Portuguese Banking Institution to determine whether customers are likely to subscribe to a Term Deposit. Our goal is to explore what features are most important in regards to determining whether a customer will subscribe to a term deposit, including customers' existing relationships with banks, broad economic factors, marketing campaign strategies, and customer demographics. We will utilize our results to identify the most influential drivers of customer behavior regarding subscriptions, provide analytics of ideal target customers, and make recommendations on future marketing campaigns, with the aim of maximizing efficacy and subscription rates.

## Methods
- EDA
- Feature Engineering
- Train/Test Split
- Logistic Regression
- K Nearest Neighbors
- Decision Tree
- Support Vector Machines
- Model comparisons, hyperparameter tuning
- Exploring Coefficients
- Classification Reports
- Dummy Classifier

## Key Findings and Business Recommendations

### What our models tell us.

Based on our primary objective of analyzing approximately 5 years worth of phone marketing campaign data from a Portuguese Banking Institution in order to determine whether customers are likely to subscribe to a Term Deposit, we have found that utilizing bank-related features from this dataset, our models were able to achieve high accuracy, in the range of 89%, but our models were not effective at identifying customers who subscribed, as indicated by low Recall. This is due to the fact that only about 11% of customers in our dataset subscribed ('yes'), versus 89% that did not subscribe. Our models struggled to identify customers that subscribed, based on the selected features and the imbalanced data.¶

### Business Recommendations
In order to obtain potentially more accurate predictions and higher recall, bank-only features should not be solely relied upon. We should attempt to incorporate other features from our dataset, including data points from previous marketing campaigns, and broader economic factors.

What we can glean from our findings are features that are associated to a higher or lower liklihood of subscription.

Features associated with a higher liklihood of subscription include job status of 'student', 'retired', and 'unemployed'. Next is age, then an 'unknown' status of education.

The top feature associated with lower liklihood of subscription is default status of 'unknown'. This is interesting, since the unknown status does not inform us whether the customer has defaulted or not, but the weight of this variable is significant in terms of not subscribing. This poses several questions: Why is default status unknown? Is it a data error? Did the customer not provide factual information? Does unknown here indicate a higher rate of actual default, which might enlighten us as to the customer's financial standing, possibly informing us that they do not have funds for term deposit? Or is this completely arbitrary and unrelated?

The following features associated with a liklihood of not subscribing include 'divorced', 'blue collar job', 'entrepreneur', 'services job', 'education basic 9y', 'married', 'no housing', 'loan status yes', 'technician job'.

In addition to further exploration while including exempted features (marketing campaign status and economic factors), more research would be valuable regarding effectiveness of demographics to target with marketing, particularly students and retired professionals. What would make a student more likely to subscribe? Are they inclined to deposit student loan money? Are they more likely to take financial risks? As for retired professionals, perhaps they've already acquired their nest egg and are more willing to subscribe to a term deposit with a goal of diversifying.
  
## Tools Used
- Jupyter Notebook
- Python
- pandas
- seaborn
- matplotlib
- sklearn
- numpy
