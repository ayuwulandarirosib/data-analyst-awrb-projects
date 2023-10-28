# Trending Video Analysis Dashboard on YouTube
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my project Number _Eleven_.
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Arrangements ✨
> This project is packaged in a ZIP archive file format,
> with an archive size not exceeding 9 megabytes.
> File with data uploaded to dashboard _(trending_by_time.csv)_.
> Link to dashboard on Tableau Public server.
> Link to dashboard on Tableau Public server.
> Instructions on how to run all files (readme.txt).

## Introduction
It is about Dashboard, steps need to be taken to design and create a dashboard. The necessity is by discussing the content of it, its layout, and the data that should be displayed. Then, converse to database administrators and data engineers to find out where and how to collect the needed data, including how to change it. Also ask them where the aggregate table is stored. Finally, develop the pipeline and dashboard.

## Goal
Yes, we need to discuss the dashboard draft and technical requirements with managers. After that, we will meet the administrator. Compiling the code for the dashboard is the last thing that needs to be done.

## Technical Guidelines
- Business objective: analyzing the history of trending videos on YouTube
- Targeted dashboard users: video ads planning managers
- Dashboard data content:
    a. Videos that have been trending, grouped by day and category
    b. Trending videos, grouped by country
    c. Table linking categories and countries

## Parameters used to group data
- Trending date and time
- Video category
- Country

## Data
- Trending history — absolute values ​​divided by days (two charts: absolute value and percentage ratio)
- Sessions, grouped by country — relative value (% of sessions)
- Relationship between categories and countries — absolute values ​​(table)
- Significance: all charts are equally important
- Data source for the dashboard: the data engineer will create an aggregate table named trending_by_time. Here is the structure:
    a. _record_id_ — primary key
    b. _region_ — country/geographical area
    c. _trending_date_ — date and time
    d. _category_title_ — video category
    e. _videos_count_ — number of videos in the trending segment
- Graphics, dashboard controls, and their layout

## libraries
_dashboard_
_pipeline_

