# 'Surf' and 'Ultimate' Package Prepaid Plan Analysis: Which one is better for generating more profit?
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my project Number _Four_.
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Features ✨
> Megaline is one of the Telecommunications Operator Company
> and on this occasion I have the credence to analyze Megaline's products.

## Introduction
The company offers its clients two prepaid plans, Surf and Ultimate. The advertising department wants to know which prepaid plan generates more profit to adjust the advertising budget.

## Goal
I am going to conduct an initial analysis of the prepaid plans based on a relatively small sample of clients. I will have the datas on 500 Megaline clients: who they are, where they are from, what type of plan they use, and the number of calls and messages they sent in 2018. My job is to analyze client behavior and determine which prepaid plan brings in more profit.

Megaline rounds seconds to minutes, as well as megabytes to gigabytes. For calls, each individual calls is rounded up: even if the call lasts only one second, it will count as one minute. For web traffic, each web sessions is not rounded up. However, totals for a month are rounded up. If a user spends 1025 megabytes this month, then he will be charged for 2 gigabytes.

'Surf'
1. Monthly fee: $20
    2. 500 minutes of call duration per month, 50 SMS, and 15 GB data
    3. After exceeding the package limit, customer will be charged:
        - 1 minute: 3 cents
        - 1 SMS: 3 cents
        - 1 GB data: $10

'Ultimate'
1. Monthly fee: $70
    2. 3000 minutes of call duration per month, 1000 SMS and 30 GB data
    3. After exceeding the package limit, customer will be charged:
        - 1 minute: 1 cent
        - 1 SMS: 1 cent
        - 1 GB data: $7

## Stages
There are several steps to complete this project, namely:
1. Data Overview (Step 1. Downloading and Loading The Data)
In this stage, we will load and read datasets from the following file path:

    '/datasets/megaline_calls.csv'
    '/datasets/megaline_internet.csv'
    '/datasets/megaline_messages.csv'
    '/datasets/megaline_plans.csv'
    '/datasets/megaline_users.csv'

    Here are the data descriptions of the files path above:

    a. megaline_calls.csv contains:
    - id — Unique web session ID
    - call_date — call date
    - duration — call duration (in minutes)
    - user_id — ID of the user making the call

    b. megaline_internet.csv contains:
    - id — Unique web session ID
    - mb_used — volume of data consumed during the session (in megabytes)
    - session_date — web session date
    - user_id — User ID

    c. megaline_messages.csv contains:
    - id — Unique SMS ID
    - message_date — date the SMS was sent
    - user_id — ID of the user who sent the SMS

    d. megaline_plans.csv contains:
    - plan_name — phone plan name
    - usd_monthly_fee — monthly fee in US dollars
    - minutes_included — monthly call minute allocation
    - messages_included — monthly SMS allocation
    - mb_per_month_included — monthly data volume allocation (in megabytes)
    - usd_per_minute — price per minute if the package allocation limit has been exceeded (for example, if the package has an allocation of 100 minutes, then usage starting from the 101st minute will be charged)
    - usd_per_message — price per SMS if the package allocation limit is exceeded
    - usd_per_gb — price per extra gigabyte of data if the package allocation limit is exceeded (1 GB = 1024 megabytes)

    e. megaline_users.csv contains:
    - user_id — User ID
    - first_name — user's first name
    - last_name — user's last name
    - age — user's age (years)
    - reg_date — subscription start date (dd, mm, yy)
    - churn_date — the date the user stopped using the service (if the value is missing, it means the service plan was in used when this data was generated)
    - city — the city where the user lives
    - plan — name of phone plan

2. Data Pre-processing (Step 2. Exploring and Rectifying the Data)
In this stage, we will explore and rectify the dataset.

3. Explorative Data Analysis (EDA) (Step 3. Performing Several Focus Things to be Analyzed)
In this stage, we are going to study the terms and conditions related to prepaid packages, aggregating data per user, and describe the consumers behavior and there are several things that need to be our focus on, namely:

    - Calls
    - Messages/SMS
    - Internet

    Also we will study about the Profit.

    We will find out the minutes, messages, and volume of mobile data usage that users of each plans require per month. Then, we calculate the mean, variance, and standard deviation. Also, make a histogram and describe the distribution.

4. Hypothesis Testing (Step 4. Doing Tests on The Hypothesis)
In this stage, we will do the tests on the Hypothesis.

    a. The average profit of Surf and Ultimate phone plan users is different.
    b. The average users profit in the NY-NJ area is different from the users profit from other areas.

    We are going to determine how large the "alpha" value to use and explaining:
- How do we formulate the null hypothesis and alternative hypothesis.
- What criteria do we use to test the hypothesis and the rationale for using them.

5. Presentation (Step 5. Presenting My Project to The Viewers)
In this stage, I will present for my Project Presentation related to 'Surf' and 'Ultimate' Package Prepaid Plan Analysis: Which one is better for generatnig more profit? analysis.

6. General Conclusions (Step 6. Formulating General Conclusions)
In this stage, we will draw the whole of general conclusions.

## libraries
_pandas_
_numpy_
_scipy_
_matplotlib.pyplot_
_seaborn_
