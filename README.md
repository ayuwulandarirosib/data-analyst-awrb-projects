# An International Online Store Analytical Project by Using The A/B Testing
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my **Final Project** of **_Number One_**
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Features ✨
> We have received an analytical task,
> from an international online store.
> Our predecessor failed to complete the project:
> the report is they launched an A/B test and then quit.

## Introduction
Based on the information we have received, they start watermelon farm in Brazil. And what do we get is the technical specifications and the test results cause they left only both things.

## Goal
As previously clarified above, that our predecessor failed to complete the analytical project, and their endeavor stopped at launched an A/B test and then quit cause starting watermelon farm in Brazil. Fortunately, they left several things, those are the technical specifications and the test results. Therefore, the technical description that we could obtain are:

- The Test Name: recommender_system_test
- Groups: А (control), B (new payment funnel)
- Launch date: 2020-12-07
- The date when they stopped taking up new users: 2020-12-21
- End date: 2021-01-01
- The Audience: 15% of the new users from the EU region
- The Purpose of The Test: testing changes related to the introduction of an improved recommendation system
- The Expected Result: within 14 days of signing up, users will show better conversion into product page views (the product_page event), product card views (product_card) and purchases (purchase). At each of the stage of the funnel product_page → product_card → purchase, there will be at least a 10% increase.
- The Expected Number of Test Participants: 6000

In a nutshell, we have already a short overview which we could make materials and directions or instructions to continue this project.

## Stages
There are several steps to complete this project, namely:
1. Data Pre-processing (Step 1. Downloading and Loading The Data)
In this stage, we will load and read datasets from the following file path:

    a) _**'/datasets/ab_project_marketing_events_us.csv'**_   — the calendar of marketing events for 2020
    b) _**'/datasets/final_ab_new_users_upd_us.csv'**_        — all users who signed up in the online store from December 7 to 21, 2020
    c) _**'/datasets/final_ab_events_upd_us.csv'**_           — all events of the new users within the period from December 7, 2020 to January 1, 2021
    d) _**'/datasets/final_ab_participants_upd_us.csv'**_     — table containing test participants

    Here are the data descriptions of the files path above:

1) _'/datasets/ab_project_marketing_events_us.csv'_ structures contain:
- name — the name of the marketing event
- regions — regions where the ad campaign will be held
- start_dt — campaign start date
- finish_dt — campaign end date

2) _'/datasets/final_ab_new_users_upd_us.csv'_ structures contain:
- user_id
- first_date — sign-up date
- region
- device — device used to sign up

3) _'/datasets/final_ab_events_upd_us.csv'_ structures contain:
- user_id
- event_dt — event date and time
- event_name — event type name
- details — additional data on the event (for instance, the order total in USD for 'purchase' events)

4) _'/datasets/final_ab_participants_upd_us.csv'_ structures contain:
- user_id
- ab_test — test name
- group — the test group the user belonged to


2. Explorative Data Analysis (EDA) (Step 2. Performing Several Focus Things to be Analyzed)
In this stage, there are several things that need to be our focus, namely:
    a. Learning Conversion at Different Funnel Stages
    b. Learning Whether The Number of Events Per User Distributed Equally in The Samples
    c. Learning Whether The Users who Enter Both Samples
    d. Learning How Is The Number of Events Distributed by Days
    e. Learning The Possible Details in The Data that We have to take into Account before starting The A/B Test


3. Evaluation The A/B Test Results (Step 3. Evaluating The A/B Test Results of The Project)
In this stage, we will evaluate the A/B test results with a few things to focus on:
    a. Several Things that We Get about The A/B Test Results
    b. The Use of Z-Criterion to Check The Statistical Difference between The Proportions

    For our some experiments:
- By Using The Significance Level / "Alpha" Value = 0.01
- By Using The Significance Level / "Alpha" Value = 0.05


4. Presentation
In this stage, I will present My Project to The Clients.

5. General Conclusions and Recommendations (Step 4. Formulating General Conclusions and Recommendations for Working with Clients)
In this stage, we will draw the conclusions and formulate the recommendations.

## libraries
_pandas_
_numpy_
_matplotlib.pyplot_
_seaborn_
_graph_objects_
_stats_
_warnings_


