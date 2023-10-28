# Increasing Revenue of Big Online Store Alpha by Prioritizing Hypothesis and Analysis A/B Testing
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my project Number _Eight_.
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Features ✨
> I have recently found a new project,
> in a large online store as an analyst.

## Introduction
My marketing team and I have put together a list of hypotheses to help increasing the revenue.

## Goal
The purpose of the current project analysis is prioritizing the hypotheses that have been described slightly above, running A/B testing, and analyzing the results.

## Stages
There are several steps to complete this project, namely:
1. Data Overview (Step 1. Opening the Data File, Prioritizing Hypotheses Framework ICE and Framework RICE, A/B Testing Analysis, and Examining Data General Information)
In this stage, we will open the data file, then making prioritize Hypotheses for Framework ICE and Framework RICE, A/B Testing Analysis, and examining data general information.

    A. The data used in the first part of the project is: /datasets/hypotheses_us.csv with details:
    - Hypotheses — a brief description of the hypothesis
    - Reach — user reach, on a scale of one to ten
    - Impact — the impact on users, on a scale of one to ten
    - Confidence — confidence in the hypothesis, on a scale of one to ten
    - Effort — the resources needed to test the hypothesis, on a scale of one to ten. The higher the Effort value, the more resource intensive the test is.

    B. The data used in the second part of the project are:
    - /datasets/orders_us. csv
    - /datasets/visits_us.csv


    The file path: _/datasets/orders_us.csv_ contains details:
- transactionId — order ID
- visitorId — ID of the user who made the order
- date — the date the order was created
-revenue — revenue from orders
- group — the A/B test group to which the user belongs


    The file path _/datasets/visits_us.csv_ contains details:
- date — date
- group — A/B test group
- visits — the number of visits on the specified date for the specified group of A/B test

    ###### Part 1. Prioritizing Hypotheses
    The 'hypotheses_us.csv' file contains nine hypotheses for increasing online store revenue with Reach, Impact, Confidence and Effort defined for each.

    The stages are as follows:
    - Implement the ICE framework to prioritize hypotheses.
    - Implementing the RICE framework to prioritize hypotheses.
    - Shows hypothetical priority changes when RICE is implemented to replace ICE. Provide an explanation regarding the change.

    ###### Part 2. A/B Testing Analysis
    We have done A/B testing and got the results as described in the 'orders_us.csv' and 'visits_us.csv' files.    

2. Data Preprocessing and Graph Analysis (Step 2. Ensuring for Missing Values, Duplicate Data, and Analyzing A/B Testing.)
At this stage, we will review and analyze several questions regarding A/B testing analysis as follows:

    a. Drawing a graph of cumulative income by group. Following the conclusions and assumptions.
    b. Drawing a graph of the cumulative average order size by batch. Following the conclusions and assumptions.
    c. Drawing a graph of the relative differences for the cumulative average order size of group B compared to group A. Following the conclusions and assumptions.
    d. Calculating the conversion rate of each batches as the ratio of orders to the number of visits each days. Under far below is a graph of the daily conversion rates of the two groups and an explanation of the differences. As well as conclusions and assumptions.
    e. Creating a scatter plot for the number of orders per user. Following the conclusions and assumptions.
    f. Calculating the 95th and 99th percentiles for the number of orders per user. Determining the point when a data point turns into an anomaly.
    g. Creating a scatter plot for the price of the order. Following the conclusions and assumptions.
    h. Calculating the 95th and 99th percentiles for the order price. Determining the point when a data point turns into an anomaly.
    i. Finding the statistical significance of conversion differences between groups using the raw data. Following the conclusions and assumptions.
    j. Finding statistical significance of differences in mean order size between groups using raw data. Following the conclusions and assumptions.
    k. Finding the statistical significance of conversion differences between groups using filtered data. Following the conclusions and assumptions.
    l. Finding the statistical significance of differences in average order size between groups using filtered data. Following the conclusions and assumptions.
    m. Making a decision based on the test results. Possible decisions are: 1. Stopping testing, and consider one of the groups as the leader. 2. Stopping testing, and concluding that there is no difference between the two groups. 3. Resuming testing.


3. Presentation (Step 3. Presenting My Project to The Viewers)
In this stage, I will present for my Project Presentation related to 'Increasing Revenue of Big Online Store Alpha by Prioritizing Hypothesis and Analysis A/B Testing' analysis.

4. General Conclusion (Step 4. Formulating General Conclusions)
In this stage, we will draw the general Conclusions of the project and our project will be assessed based on the following criteria:
- How we prepare the data for analysis
- How do we formulate hypotheses
- How do we interpret the resulting graph
- How do we calculate statistical significance
- What conclusions do we make based on the results of the A/B testing obtained
- Do we follow the project structure and keep the code tidy
- The conclusion we made
- Do we make comments at every step

## libraries
_datetime_
_pandas_
_matplotlib.pyplot_
_numpy_

