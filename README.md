# Interaction and Retention Strategies Analysis through Digitizing Customer Profiles
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my project Number _Twelve_.
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Features ✨
> The latest information regarding a fitness center franchise named,
> 'Model Fitness' is developing a customer engagement strategy based on analytical data.
> One of the most common problems encountered by fitness center services,
> and even other services is customer turnover or customer churn.
> How do we know when a customer has stopped using our service?
> We could indeed calculate the churn rate,
> based on the number of people who
> delete accounts or do not renew their subscriptions.
> But sometimes, we could not know for sure,
> whether a client has actually quit: they may have left us without our knowledge.

## Introduction
Churn indicators could vary from one field to another. If a user makes purchases from an online store on an irregular but regular basis, we could not say that the user has left our store. However, if for two weeks a user does not open an online shop channel which is updated daily, then we could worry: our followers may get bored and decide to leave us.

For fitness center businesses, it will be considered a customer to leave if they do not return for one month. In fact, it is not necessarily true. A customer may not visit the fitness center for a month because he or she is on vacation, for example to Bali, and will return to visit the fitness center after his or her vacation is over. However, cases like this are rare. Usually if a customer decides to join, then comes a few times and then disappears, the chances are that customer will not come back.

## Goal
From the explanation above, to reduce the churn rate, 'Model Fitness' has digitized a number of its customer profiles. Our task is to analyze the profiles of these customers and develop customer retention strategies (customer retention).

For that, we have to:
    - Learn how to predict the churn probability (for the next month) for each customer
    - Create user segmentation by selecting the most dominant group and describing its main features
    - Analyze the factors that most influence churn
    - Draw basic conclusions and provide recommendations on how to improve customer service
        
        a. Identify the target group
        b. Recommend steps to reduce churn
        c. Describe any other patterns we have encountered with customer interactions

## Stages
There are several steps to complete this project, namely:
1. Data Overview and Preprocessing (Step 1. Downloading Database and Loading The Data)
In this stage, we will load and read datasets from the following file path:

    _/datasets/gym_churn_us.csv_

Here are the data descriptions of the file path above:

- 'Churn' — actual churn for the month
- 'gender'
- 'Near_Location' — whether the user lives or works near the gym location
- 'Partner' — whether the user is an employee of the partner company (this gym has a partner company and their employees are eligible for discounts; in this case, the gym stores information about the company their customer works for)
- Promo_friends — whether the user initially signed up via a "refer a friend" offer (they used a friend's promo code when paying for their first membership)
- 'Phone' — whether the user provided their phone number
- 'Age'
- 'Lifetime' — time (in months) since the customer's first visit to the fitness center
- 'Contract_period' — 1 month, 3 months, 6 months or 1 year
- 'Month_to_end_contract' — the remaining months before the contract expires
- 'Group_visits' — whether the user is taking part in group sessions
- 'Avg_class_frequency_total' — average frequency of visits per week over the customer's lifetime
- 'Avg_class_frequency_current_month' — average frequency of visits per week for the current month
- 'Avg_additional_charges_total' — the total amount of money spent to pay for other services at the gym: cafe, athletic goods, cosmetics, massage, etc.


2. Data Processing (Step 2. Performing Explorative Data Analysis (EDA))
In this stage, there are several things that need to be our focus, namely:

    1. Taking a look at the dataset, are there any missing features?
   - learning its average value and standard deviation (by using 'describe()' method).
    2. Seeing the average feature value in two groups.
   - namely for those who left (churn) and for those who stayed (by using 'groupby()' method).
    3. Creating a histogram and feature distribution for those who left (churn) as well as those who stayed.
    4. Creating a correlation matrix and display of the results.


3. Building Model of Machine Learning (Step 3. Building a Model to Predict User Churn)
In this stage, we will create a binary classification for customers, where the target feature will be users who will leave next month. During the process, we will do the following matters: 

    1. Splitting the data into a 'train set' and a 'validation set' by using the 'train_test_split()' function.
    2. Instructing a model on a 'train set' with the following two methods:
   - logistic regression
   - random forest
    3. Evaluating the 'accuracy', 'precision' and 'recall' for both models by using 'validation set'. We will use those metrics to compare the models. Which model gives the best results?

    Next, we will indicate the 'random_state' parameter when dividing the data and specifying the algorithm.


4. User Cluster (Step 4. Creating A User Cluster)
In carrying out this stage, we will select the column that contains the churn data and define the cluster of objects (users) by doing the following:

    1. Standardizing the data.
    2. Using the 'linkage()' function to create a distance matrix based on a standardized feature matrix and graph of the dendrogram.
   - For Note: The dendrogram creation may take some times.
   - We will use the resulting graph to estimate the number of clusters we can choose from.
    3. Instructing a clustering model with the 'K-means' algorithm and predict its customer clusters.
   - Make it until the number of clusters is n = 5, so that it will be easier to compare the results we get with the results obtained by other students.
   - However in real life, no one would ever give us such a hint.
   - Therefore, going forward, we must make a decision based on the graph from the previous step.
    4. Looking at the feature values average for all the clusters. Is there anything catches our attention?
    5. Making a distribution feature graph for each clusters. Did we notice anything?
    6. Calculating the churn rate for each clusters (by using the 'groupby()' method).
   - Do the clusters differ in terms of churn rates?
   - Which customer clusters are likely to leave, and which will remain loyal?


5. Presentation (Step 5. Presenting My Project to The Viewers)
In this stage, I will present for my Project Presentation related to 'Interaction and Retention Strategies Analysis through Digitizing Customer Profiles' analysis.


6. General Conclusions and Recommendations (Step 6. Formulating General Conclusions and Recommendations for Working with Customers)
    In this stage, we will draw the conclusions and formulate recommendations regarding customer interaction and retention strategies.

## libraries
_pandas_
_numpy_
_matplotlib.pyplot_
_seaborn_
_spearmanr_
_train_test_split_
_StandardScaler_
_LogisticRegression_
_RandomForestClassifier_
_KMeans_
_dendrogram, linkage_
_accuracy_score, precision_score, recall_score_
_warnings_


