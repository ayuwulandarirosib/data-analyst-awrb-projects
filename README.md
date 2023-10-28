# Video Game Sales by 'ICE' Online Store from Around the World
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my project Number _Five_.
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Features ✨
> The current project is an analytical case study in a real-life context.
> "Ice" Online Store sells video games from all over the world.

## Introduction
The data related to user and expert reviews of games, genres, platforms (for example: Xbox or PlayStation), and historical data on game sales are available from open sources. We need to take a look the patterns that determine whether a game could be said to be successful or not and find the potential games.

## Goal
In this occasion, we are going to identify the patterns that determine whether a game could be said to be successful or not. From that way, we could find the games with the most potential and plan the advertising campaign. Currently, we have the data from 2016. Let's imagine that it is December 2016 and we are planning a campaign for 2017.

Then, the most important thing for us is to gain experience working with data. It doesn't matter whether we forecast 2017 sales based on data from 2016 or forecast 2027 sales based on data from 2026. This dataset contains abbreviations. ESRB is an abbreviation for Entertainment Software Rating Board, which is an independent regulatory organization that evaluates game content and assigns age ratings such as Teen or Mature.

## Stages
There are several steps to complete this project, namely:
1. Data Overview (Step 1. Opening the Data File and Examining the General Information)
In this stage, we will load and read the dataset from the following file path:

    '/datasets/games.csv'

    Here are the data description of the file path above:

- Name (name)
- Platform
- Year_of_Release (year of release)
- Genre
- NA_sales (sales in North American in millions of USD)
- EU_sales (sales in Europe in million USD)
- JP_sales (sales in Japan in million USD)
- Other_sales (sales in other countries in million USD)
- Critic_Score (review score from critics, maximum 100)
- User_Score (user review score, maximum 10)
- Rating (ESRB)

Data for 2016 might be incomplete.

2. Data Pre-processing (Step 2. Preparing and Ensuring the Data Quality, Data Type, Array Form, Missing Values, and Duplicate Data)
In this stage, we will prepare and ensure the dataset.

3. Data Reconstructing (Step 3. Rectifying the Data)
In this stage, we will rectify the dataset, namely:
    a. Renaming the columns (making all in lowercase).
    b. Converting the data to the required data type.
    c. Describing which columns have their data types changed and explaining why.
    d. Determining how to handle missing values:
        - Explaining the reason for filling in missing values in the way that was done or the reason for leaving them blank.
        - Why are the values missing? Providing possible reasons.
        - Paying attention to the abbreviation TBD (to be determined). Determining how to handle such cases.
    e. Calculating total sales (sum of sales across all regions) for each games and enter these values into separate columns.

4. Explorative Data Analysis (EDA) (Step 4. Performing Several Focus Things to be Analyzed)
In this stage, we are going to perform several focus things to be analyzed, namely:
a. Reviewing how many games were released in different years.
b. Seeing how sales vary from one platform to another.
c. Determining the time period for data collection.
d. Working only with relevant data.
e. Which platform has the most sales.
f. Creating a boxplot for global sales of all games grouped by platform.
g. Seeing how user and professional reviews impact sales on one of the popular platforms.
h. Comparing sales of the same game on other platforms.
i. Observing the general distribution of games by genres.

5. Profiling (Step 5. User Profiling for Each Regions)
In this stage, we will perform the user profiling for each regions.
For each regions (NA, EU, JP), determining:
a. Top 5 platforms. Explaining variation in market sharing from one region to another.
b. Top 5 genres. Explaining the differences.
c. Does the ESRB rating affect sales in each regions?

6. Hypothesis Testing (Step 6. Doing Tests on The Hypothesis)
In this stage, we will do the tests on the Hypothesis.
- The average user rating for Xbox One and PC platform is the same.
- The average user rating for the Action and Sports genre is different.

Set our own alpha threshold value.

Explaining:
- How do we formulate the null hypothesis and alternative hypothesis.
- What level of significance would we choose to test our hypothesis, and explain why we choose that number.

7. Presentation (Step 7. Presenting My Project to The Viewers)
In this stage, I will present for my Project Presentation related to 'Video Game Sales by 'ICE' Online Store from Around the World' analysis.

8. General Conclusions (Step 8. Formulating General Conclusions)
In this stage, we will draw the whole of general conclusions.

## libraries
_pandas_
_numpy_
_scipy_
_matplotlib.pyplot_
_seaborn_
