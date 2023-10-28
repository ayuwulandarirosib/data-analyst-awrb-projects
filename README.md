# Market Research from Open Source Datas Related Eateries Types in Los Angeles
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my project Number _Nine_.
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Features ✨
> I have decided to open a small 'Cafe' in Los Angeles.
> This 'Cafe' could be said to be quite unique,
> because I "employ" a robot as a waiter or waitress.

## Introduction
This project is indeed promising, but requires large capital. Therefore, my partners and I decided to attract investors. We are interested in the current state of the market. However, there is little concern about sustaining success as the robot's appeal begins to wane. Could this business be handled and given solutions.

In this project, I will try to prepare some market researches to analyze, consider and predict the factors that affect the 'Cafe' business that we will build.

## Goal
As we discussed earlier, the partners asked me to prepare some market researches. I have open source datas related Eateries Types in Los Angeles.

Next, I will prepare a research presentation to share with investors. I'll use any tools to make it, and I'll convert it into PDF format to make the presentation that I present later easier to judge. I'll also include a link to the presentation in the markdown cells below in the format:

Presentation: <link to cloud storage>.

## Stages
There are several steps to complete this project, namely:
1. Data Overview (Step 1. Downloading and Preparing the Datas for Analysis)
At this stage, we will load and read dataset from the following file path:

    _/datasets/rest_data_us.csv_

    Here is the data description of the file path above:

    _'rest_datas'_ Table:
    - object_name — business name
    - chain — franchise based business (TRUE/FALSE)
    - object_type — type of business
    - address — address
    - number — number of chairs

    Also, we will check the data quality in each columns of 'id', 'object_name', 'address', 'chain', 'object_type', and 'number' by utilizing:
    
    a. For 'id':
rest_datas['id'].sort_values()

    b. For 'object_name':
rest_datas['object_name'].value_counts()

    c. For 'address':
rest_datas['address'].value_counts()

    d. For 'chain':
rest_datas['chain'].unique()

    e. For 'object_type':
rest_datas['object_type'].unique()

    f. For 'number':
rest_datas['number'].sort_values()

    - Then, we will convert the data type 'id' column from "int" to "string" by using: rest_datas['id'] = rest_datas['id'].astype('str').

    - And converting data type 'chain' column from "object" to "boolean" by using: rest_datas['chain'] = rest_datas['chain'].astype(bool).

    - After that, we check for missing values and data duplicate by using: rest_datas.isna().sum() and rest_datas.duplicated().sum(). 

2. Data Preprocessing (Step 2. Data Analysis)
First, we will ensuring the datas before processing by making sure for data type, array form, and missing value.

    After that, we have some mission tasks to be processed and analyzed, they are:

    a. Examining the proportions of the businesses various types - And Showing The Graph.
    b. Examining the proportions of chain-based and non-chain based businesses - And Showing The Graph.
    c. Which type of business is usually a chain-based business?
    d. Which are the characteristics of a chain-based business:
    - Having many places with a small number of seats or having several places with a large number of seats?

    e. Determining the average number of seats for each type of eateries business.
    - On average, which type of eateries have the highest number of seats?

    f. Moving the street name data from the address column to a separate column.
    g. Making a Graph showing the top ten street names by number of establishments (eateries).
    - The top ten street names by number of eateries.
    - The top ten street names based on the most number of cafes.

    h. Finding the number of street names that have only one establishment (eateries).
    i. For a street occupied by many eateries, pay attention to the distribution of the number of seats.
    - What trends could we observe?

3. Presentation (Step 3. Preparing the Presentation)
At this stage, we will prepare the presentation with the following instructions:
- Preparing research presentation for distribution to investors.
- Tools in making presentation.
- Converting presentation into PDF format.
- Including a link to the presentation in markdown cells in the format of:


    Presentation: <link to cloud storage>

_Format (Additional note):_
- Completing tasks in Jupyter Notebook.
- Entering code in code cell and explanatory text in markdown cell.
- Applying formatting and add titles.

4. General Conclusions
General conclusions and provide recommendations on the type of business and the number of seats. Provide comments on franchise-based business development opportunities.

    This project will be assessed based on the criteria below:
- How do we prepare the datas for analysis.
- The type of graphs we created.
- Our precision in selecting the graphs type for the datas.
- Do we use the Seaborn library to work with graphics.
- How do we interpret the generated graphs.
- How do we calculate and interpret each parameters.
- Do we prepare structured presentation.
- How well do we adhere to the principles given in this course for making presentation.
- How do we convey the main message of our presentation.
- Did we follow the project structure and how well did we keep our code tidy.
- The conclusion we made.
- Did we comment for each steps.

## libraries
_pandas_
_matplotlib.pyplot_
_seaborn_
_plotly.express_
_graph_objects_
_warnings_

