# Marketing Budget Optimization: Y.Afisha Company
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my project Number _Seven_.
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Features ✨
> Achieving brilliant performance requires effort,
> and hard work in carrying out the process.
> Now is the opportunity where I was entrusted
> to undergo an internship program
> in the analytics department at Y.Afisha company.

## Introduction
The first task given to me in this opportunity is to help optimize marketing costs. Then here I have some datas:

- Server logs/records containing data on visits to the Y.Afisha site from January 2017 to December 2018
- Dump file containing all orders for the period
- Statistics on marketing costs

## Goal
Some of the datas that have been explained before, I will also learn the following things:
- How users use Y.Afisha products
- When did they start making purchases
- How much money each users contribute
- When all marketing costs are paid

## Stages
There are several steps to complete this project, namely:
1. Data Overview (Step 1. Opening the Data File and Examining the General Information)
visits, orders and costs data in variables will be stored. Then optimizing the data I have for analysis purposes by ensuring each columns is presented in the correct data type. The data is presented in the following file path:

    a. /datasets/visits_log_us.csv
    b. /datasets/orders_log_us.csv
    c. /datasets/costs_us.csv

Here are the data descriptions of the files path above:

    a. Visits table (server logs/records that contain website visit data):
        - Uid — User ID
        - Device — user device
        - Start Ts — session start date and time
        - End Ts — session end date and time
        - Source Id — advertising source ID, the source by which the user came to the website

All dates in this table use the YYYY-MM-DD format.

    b. Orders table (data related to orders):
        - Uid — ID of the user who made the order
        - Buy Ts — the date and time the order was made
        - Revenue — Y.Afisha's income from the order

    c. Costs table (data related to marketing expenditure):
        - source_id — ad source ID
        - dt — date
        - costs — expenses for advertising sources on that date

2. Data Preprocessing (Step 2. Ensuring the Missing Values, Duplicate Data, Array Form, Data Type, and other Data Preprocessing Needed)
    At this stage, I'll check the missing values, duplicate data, array form, and data type. Also, I'll build a report and calculate the metrics:

    a. Product
    - How many people use the product each days, weeks, and months?
    - How many sessions per day? (One user may have more than one session).
    - How long is the duration for each sessions?
    - How often do users return to using the product?

    b. Sale
    - When did people start making purchases? (In KPI analysis, we are usually interested in knowing the time that elapses from registration until conversion occurs or when an authorized user turns into a customer. For example, if registration and first purchase occur on the same day, that user could be placed in the conversions category H0 If the first purchase occurs the following day, the category will also be H1 conversions. I am welcome to use any approach that allows me to compare conversions from different cohorts, so I could determine which cohort or marketing channel was most effective.).
    - How many orders did they make during a given time period?
    - What is the average purchase size?
    - How much money did they contribute? (LTV)

    c. Marketing
    - How much money was spent? Overall/per source/for time to time
    - What are the customer acquisition costs from each sources?
    - How profitable is the investment? (ROI)


3. Graph Review Analysis (Step 3. Making Graphs for Analysis)
In this stage, I'll create a graph showing how these metrics differ across devices and ad sources, and how they change over time.

4. Presentation (Step 4. Presenting My Project to The Viewers)
In this stage, I will present for my Project Presentation related to 'Marketing Budget Optimization: Y.Afisha Company' analysis.

5. General Conclusion (Step 5. Formulating General Conclusions)
And finally, at this stage I will write a conclusion to tell marketing specialists how much money to invest and where to invest it.
What sources/platforms would I recommend giving reasons to support my choice:

- What metrics do I focus on and why.
- What conclusions did I draw after discovering the values of these metrics.

## libraries
_pandas_
_matplotlib.pyplot_
_scipy_
_seaborn_
_numpy_
_warnings_
_datetime_
_matplotlib.ticker_
