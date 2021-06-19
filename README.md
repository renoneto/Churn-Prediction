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

You can find the following files/folders in my repository:

### [`Real Estate Market Analysis.ipynb`](https://github.com/renoneto/second_module_project/blob/main/Real%20Estate%20Market%20Analysis.ipynb)

- **Content:** Main Jupyter Notebook with the whole analysis.

- **What I'm doing:**

1. Dataset Exploration and Cleaning.
2. Asking Questions to understand the Housing Market.
3. Running Revenue Simulations given the Business Model, trying to find the best combination of No. of Agents and Zip Codes that will increase Net Income/ROI.
4. Creating a Linear Regression Model to predict the Sale Price of Houses.
5. Analyzing the final model, understanding the weights given to each feature.
6. Presenting Conclusions/Recommendations.

### [`presentation.pdf`](https://github.com/renoneto/second_module_project/blob/main/presentation.pdf)

- **Content:** Non-technical presentation to stakeholders.

#### [Link to Google Slides](https://docs.google.com/presentation/d/1bBNCAuONw2pTGlWJGgOkkmau2-aE26REFldoL6vYWwo/edit?usp=sharing)

## Market Insights

## Revenue Simulation

## Linear Regression Model to estimate Sold Price



## Conclusions

## Next Steps

