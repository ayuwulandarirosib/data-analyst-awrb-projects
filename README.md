# Contagious Elements in Encashing A Car Analysis
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my project Number _Three_.
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Features ✨
> Advertisements are an effective medium in marketing goods,
> especially in marketing four-wheeled vehicle advertisements.

## Introduction
On the following occasion, I will analyze the dataset in the car sales file. Hundreds of free vehicle advertisements appear on company's website every day. We need to study data sets over the past few years and determine the factors that influence the price of a vehicle.

## Goal
This project deals with factors that could influence the sales of a car, especially on the Crankshaft List. This analysis was conducted by using data collected from the hundreds of free vehicle advertisements that are displayed on websites every day. This greatly affects the number of sales that occur. So, this project was made to find out the influencing factors and determine the right steps in the car sales process.

## Stages
There are several steps to complete this project, namely:
1. Data Overview (Step 1. Downloading Database and Loading The Data)
In this stage, we will load and read the dataset from the following file path:

    '/datasets/vehicles_us.csv'

    Here are the data descriptions of the file path above:

- 'price'
- 'model_year'
- 'model'
- 'condition'
- 'cylinders'
- 'fuel' — gas, diesel, etc.
- 'odometer' — vehicle mileage when the advertisement is shown
- 'transmission'
- 'paint_color'
- 'is_4wd' — whether the vehicles has 4 wheels drive (Boolean type)
- 'date_posted' — the date the advertisement was shown
- 'days_listed' — number of days the advertisement is displayed until it is removed

2. Data Pre-processing (Step 2. Ensuring the Data Quality, Data Type, Array Form, Missing Values, and Duplicate Data)
In this stage, there are several things that need to be our focus in ensuring for the data, namely:

    a. Data Quality
    b. Data Type
    c. Array Form
    d. Missing Values
    e. Duplicate Data

3. Data Reconstructing (Step 3. Calculating and Adding some Matters to the Table)
In this stage, we are going to calculate and add some matters below:

    a. day of the week, month, and year the advertisement was shown
    b. the age of the vehicle (in years) when the advertisement was shown
    c. average vehicle mileage per year

    In the condition column, replacing the string value with a numeric scale:

- new = 5
- like new = 4
- excellent = 3
- good = 2
- fair = 1
- salvage = 0

4. Explorative Data Analysis (EDA) (Step 4. Performing Several Focus Things to be Analyzed)
In this stage, we are going to perform the exploratory data analysis, following the instructions below:

- Study the following parameters: price, age of the vehicle when the advertisement was shown, mileage, number of cylinders and condition. Make a histogram for each of these parameters. Study how outliers affect the shape and readability of a histogram.

- Define the upper bound of the outliers, remove the outliers, and store them in a separate DataFrame, then continue working with the filtered data.

- Use the filtered data to create a new histogram. Compare it with the previous histogram (the histogram that contains outliers). Draw the conclusions.

- Study how many days the advertisement was served (days_listed). Make a histogram. Calculate the mean and median. Describe how long an advertisement is generally displayed. Decide when advertisement are removed quickly, and when advertisement are served for a very long time.

- Analyze the number of advertisements and the average price for each type of vehicles. Make a graph showing the dependence number of advertisement on the type of vehicles. Choose the two types of vehicles with the most number of advertisement.

- What are the factors that most influence the price of a vehicle? Take each of the popular vehicles types we found in the previous stages and study if their prices depend on their age, mileage, condition, transmission type, and color. Make a boxplot graph for the categorical variables (transmission type and color), then make a scatterplot for the rest. When analyzing categorical variables, remember that a category must have at least 50 advertisements. Otherwise, the parameters will not be valid for use during analysis.

5. Presentation (Step 5. Presenting My Project to The Viewers)
In this stage, I will present for my Project Presentation related to Contagious Elements in Encashing A Car Analysis.

6. General Conclusions (Step 6. Formulating General Conclusions)
In this stage, we will draw the whole of general conclusions.

## libraries
_pandas_
_matplotlib.pyplot_
_seaborn_
