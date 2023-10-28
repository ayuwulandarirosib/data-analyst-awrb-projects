# Understanding Passenger Preferences and The Impact of Trips External Factors on Zuber Ride-Sharing Company
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my project Number _Six_.
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Features ✨
> Zuber is a recently launched ride-sharing company in Chicago.
> As an analyst at the company, I would analyze to find
> patterns in the available information.

## Introduction
The aim of this project is to understand passenger preferences and the impact of external factors on trips. The following is a Data Description regarding the database containing information on taxi trips in Chicago:

Table 'neighborhoods': data related to the area in the city of Chicago
- 'name': region name
- 'neighborhood_id': area code

Table 'cabs': data related about taxi data
- 'cab_id': vehicle code
- 'vehicle_id': Vehicle technical ID
- 'company_name': the name of the company that owns the vehicle

Table 'trips': data related about trip
- 'trip_id': trip code
- 'cab_id': operating vehicle code
- 'start_ts': date and time the trip started (time rounded off in hours)
- 'end_ts': end date and time of trip (time rounded to hours)
- 'duration_seconds': trip duration in seconds
- 'distance_miles': distance tripped in miles
- 'pickup_location_id': pickup area code
- 'dropoff_location_id': delivery area code

Table 'weather_records': data related about weather 
- 'record_id': weather code
- 'ts': date and time when the weather record was made (time rounded to hours)
- 'temperature': the temperature at which the weather record was made
- 'description': a brief description of the weather conditions, such as "light rain" (drizzle) or "scattered clouds" (cloudy).

## Goal
By using the database, I will analyze the data from competitors and test hypotheses regarding the effect of weather on trip frequency. In working on this project, it was divided into two stages, namely by using SQL and Python on Jupiterhub. And in this section, I will elaborate on working with Python on Jupiterhub.

- Description of the hypothesis that needs to be tested is as follows:
"The average trip duration from the Loop to O'Hare International Airport changes on rainy Saturdays."

- Using the last query result data file of:
'project_sql_result_07.csv'

- The file contains the trips data from the Loop to O'Hare International Airport. Followings are the values of the columns in this table are:
    a. 'start_ts'- pick-up date and time
    b. 'weather_conditions'- weather conditions when the trip begins
    c. 'duration_seconds'- trip duration in seconds

- The followings are the points in testing this hypothesis:
    a. Formulate null hypothesis and alternative hypothesis.
    b. Default alpha value is 5%.
    c. Statistical test (student t-test independent 2 samples).
    d. Comparing the p-value of statistical test results with the alpha value.

## Stages
Furthermore, as data material I obtained above, I have been given a second files where the following files consist of two CSV files:

1. 'project_sql_result_01.csv'. This file contains the following data:
- 'company_name': Taxi company name.
- 'trips_amount': number of trips for each taxis company on 15-16 November 2017.

2. 'project_sql_result_04.csv'. This file contains the following data:
- 'dropoff_location_name': the name of the Chicago area where the trip ended.
- 'average_trips': the average number of trips ending in each regions in November 2017.

There are several steps to complete this project, namely:
1. Data Overview (Step 1. Opening the Data File and Examining the General Information)
In this stage, we will load and read the dataset from the following files path that which have been mentioned above:

    'project_sql_result_01.csv'
    'project_sql_result_04.csv'

2. Data Preprocessing (Step 2. Ensuring the Data Type, Array Form, Missing Values, and Duplicate Data)
In this stage, we will check and ensure the dataset.

3. Identifying the top 10 regions (Step 3. Identifying the Top 10 Regions)
In this stage, we will identify the dataset for the top 10 regions.

4. Graph Analysis (Step 4. Making Graph for Analysis)
In this stage, we will create the graphs  for analysis the dataset.

5. Hypothesis Testing (Step 5. Doing Tests on The Hypothesis)
In this stage, we will do the tests on the Hypothesis.
    
    We are going to test the following hypothesis:
    _"The average trip duration from the Loop to O'Hare International Airport changes on rainy Saturdays."_

    we will determine the level of significance (alpha) = 5%.

Then, we will explain:
- How do we formulate the null hypothesis and alternative hypothesis.
- What criteria we used to test our hypothesis and why we used them.

6. Presentation (Step 6. Presenting My Project to The Viewers)
In this stage, I will present for my Project Presentation related to 'Understanding Passenger Preferences and The Impact of Trips External Factors on Zuber Ride-Sharing Company' analysis.

7. General Conclusion (Step 7. Formulating General Conclusions)
In this stage, we will draw the whole of general conclusions.

## libraries
_pandas_
_numpy_
_scipy_
_matplotlib.pyplot_
_seaborn_
