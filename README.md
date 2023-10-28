# Finding Out The Users Behavior of Food Product Company Application
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my project Number _Ten_.
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Features ✨
> I am currently working at a startup company,
> that sells food products.
> I need to find out the behavior of the company's app users.

## Introduction
First, we will explore the sales funnel by figuring out the path a user has to go through to get to the purchase stage. How many users actually made it to the purchase the stage. How many users have stalled in the previous stages. At what stage exactly did this happen?

Then, we will see the results of A/A/B testing. Next, the web designer team wanted to change the font for the entire app, but the product manager was worried that users would find the new design distracting. They also decided to make a decision based on the results of A/A/B testing.

The users were divided into three groups: two control groups were shown with the old font version and one test group was shown with the latest font version. My job was to find out which font would give the best results.

## Goal
Making two groups A (control) does provide certain advantages. We could lay down the rule that the accuracy of the test is acceptable only if the two control groups give similar results. If there is a significant difference between the two groups A, this could help us to identify factors that might be distorting our results. Comparing the control group will also give us an idea of how much time and data is needed when running the next process.

Throughout this project, I will be using the same dataset to do regular analysis and to do A/A/B analysis.

## Stages
There are several steps to complete this project, namely:
1. Data Overview (Step 1. Opening the Data File and Learning the General Information)
In this stage, we will load and read dataset from the following file path:

    _/datasets/logs_exp_us.csv_

    For each log entries is a record of a user action or an event. Here is the data description of the file path above:

- EventName — event name
- DeviceIDHash — User's unique ID
- EventTimestamp — event time
- ExpId — experimental numbers: 246 and 247 for the control group, 248 for the test group


2. Data Preprocessing (Step 2. Preparing Data for Analysis)
In this stage, we will analyze the data for:
- Renaming The Columns
- Checking for Data Type, Array Form, Missing Values, Duplicate Data and Correcting The Datas
- Adding Date and Time Column and A Separate Column for Dates


3. Learning and Examining The Data (Step 3. Learning and Examining the Data)
In this stage, we will administer for some cases:
- How many events are logged?
- How many users are logged in?
- What is the average number of events per user?
- What time period does the datas cover?
- Did we lose a lot of events and users when we got rid of old data?
- Making sure we have users from all three experimental groups


4. Event Funnel (Step 4. Learning the Event Funnel)
In this stage, we will learn the event funnel of:
- Checking what events are in the log and how many times they occur
- Finding the number of users who performed each action
- In what order do we think the actions took place?
- Using the event funnel to find the percentage of users who persist from one stage to the next
- At what stage did we lose a lot of users?
- What percentage of users successfully complete all stages, from first event to checkout?


5. Learning Experimental Results (Step 5. Learning the Results of Our Experiment)
In this stage, we will learn the results of our experiment by reaching some cases of:
- How many users are there in each group?
- We have two control groups in A/A testing, where we check our mechanics and calculations
- Select the most popular events
- Do the same for the group of users shown the latest font version
- Level of Significance


6. Presentation (Step 6. Presenting My Project to The Viewers)
In this stage, I will present for my Project Presentation related to 'Finding Out The Users Behavior of Food Product Company Application' analysis.

7. General Conclusions (Step 7. Formulating General Conclusions)
In this stage, we will draw the whole of general conclusions.



    In this Final of the Project, I intend to say no giving up for my skills efforts in:
    1. Data Pre-processing
    2. Explorative Analysis
    3. Statistic Analysis
    4. Business Analysis
    5. Data Storytelling

## libraries
_pandas_
_numpy_
_matplotlib.pyplot_
_seaborn_
_math_
_warnings_

