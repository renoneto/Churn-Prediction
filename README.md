# Churn Prediction for Telecom Company - The Business Case

I was hired by SyriaTel a Telecom Company to build a classifier to predict whether a customer will ("soon") stop doing business with them ( _note this is a binary classification problem_ ).

Therefore, their goal is to understand why these customers are not sticking very long and help them identify those customers before they churn so they can take action and avoid that from happening.

## The Dataset
I'm using the **Churn in Telecoms dataset** from Kaggle.

Here's the description of the dataset:
>This public dataset is provided by the CrowdAnalytix community as part of their churn prediction competition. The real name of the telecom company is anonymized. It contains 20 predictor variables mostly about customer usage patterns. There are 3333 records in this dataset, out of which 483 customers are churners and the remaining 2850 are non-churners. Thus, the ratio of churners in this dataset is 14%

[You can find more about it here](https://www.kaggle.com/becksddf/churn-in-telecoms-dataset)

## Goals

1. Show some insights about the market.
2. Analyze which features are the most/least valued.
3. Come up with ideas/strategies to enter the market given their commission-based business model.

## True vs False Positives Trade-Off
While trying to find the best model, I always kept in mind that I had to keep a good balance of True and False Positives. Having some False Positives (mistakenly predicting a churn) is okay given the goal of the project. However, causing a lot of work to the company for no reason is a problem.

Since I'm not sure exactly what would happen after the model identifies that a client is about to churn. I'm assuming it would trigger some action for Customer Support/Success to avoid that churn.

Therefore, if the model predicts that a lot of clients will churn that would also mean more time spent on False Positives and that's money lost for the company. Because of that, taking that Trade-Off into consideration is important and identifying the optimal model keeping in mind the balance between True and False Positives should be the goal.

## Navigation

You can find the following files in the repository:

### [`Churn Prediction.ipynb`](https://github.com/renoneto/third_module_project/blob/main/Churn%20Prediction.ipynb)

- **Content:** Main Jupyter Notebook with the whole analysis.

**What I'm doing:**

1. Dataset Exploration and Cleaning
2. Cleaning anda testing for Uniqueness
3. Modeling
    - K-Nearest Neighbors Classifier
    - Address Class Imbalance Problem
    - True vs False Positives Trade-off
    - Logistic Regression
    - Decision Tree
    - Random Forest
    - XGBoost
4. Comparing Models
5. Choosing a Model
6. Model Tuning
7. Model Interpretation
### [`presentation.pdf`](https://github.com/renoneto/third_module_project/blob/main/presentation.pdf)

- **Content:** Non-technical presentation to stakeholders.

#### [Link to Google Slides](https://docs.google.com/presentation/d/1SPkJVTJQiTDg1zk6MLPEP1SCyRKsn67lAQZ1AESXfbM/edit?usp=sharing)

## Conclusions
After choosing the Decision Tree model it's possible to analyze it and get to the following conclusions:

#### What's wrong with High Spenders?
A 94% of churning if the Total Charge is greater than 74.03 USD is a problem. Further research on the group is necessary for further recommendations.

#### What's wrong with the International Plan?
Non-High Spenders have high chances (82%) of churning if they have the International Plan. Maybe there's something wrong with the product. It would be worthwhile to understand what's wrong with it. Read complaints/feedback from users.

#### Reduce the No. of Customer Service Calls:
It's expected that more Customer Service Calls would lead to higher chances of churning. If a client is calling often is because there's something wrong and the company is not fixing it. I guess a good idea would be to understand the reasons of those calls and see if there's anything the Telecom can do in the product to fix those problems and reduce the No. of Calls.

Another suggestion could be to reduce the No. of Calls by providing online solutions to users or create educational materials to teach users how to use the product or a FAQ page. However, it's important to say that No. of Calls should not imply causation, rather, we should understand the reason behind the calls and work on those things.

Another possibility is that the Customer Service team is not doing a great job. Maybe they're taking to long to answer calls or solve problems.
