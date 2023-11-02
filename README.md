# Books Sparkers Apps Analysis for Startup Company
## by _Ayu Bachtiar_

[![Made withJupyter](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)](https://jupyter.org/try)
[![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)

This is my **Final Project** of **_Number Two_**
Follow my Instagram: @shakeilogram
✨Follow aja dulu!

## Features ✨
> The corona virus whose presence shocked the whole world,
> has changed everyone's daily routine.
> Now, city residents no longer spend their free time outside the home,
> such as going to cafes and malls.
> They are more often at home,
> spending time reading books.
> This also encourages startup companies,
> to develop new applications for book sparkers.

## Introduction
From developing this new application, startup companies could open their horizons to the silence of the pandemic and open various opportunities that are offered to all users for a life that continues to grow together.

## Goal
We have been got a database from one of the competing companies in this industry. The database contains data about books, publishers, authors, as well as customer ratings and reviews of related books. We will use this information in making a price quote for a new product.

And we will elaborate and display those discoveries in this project.

## Stages
There are several steps to complete this project, namely:
1. Data Pre-processing (Step 1. Accessing Database and Loading The Data)
In this stage, we will access and load the Database by using the following database code files path:


    import pandas as pd
    from sqlalchemy import create_engine

    db_config = {'user': 'practicum_student',         
             'pwd': 's65BlTKV3faNIGhmvJVzOqhs', 
             'host': 'rc1b-wcoijxj3yxfsf3fs.mdb.yandexcloud.net',
             'port': 6432,              
             'db': 'data-analyst-final-project-db'}          

    connection_string = 'postgresql://{}:{}@{}:{}/{}'.format(db_config['user'],
                                                                     db_config['pwd'],
                                                                       db_config['host'],
                                                                       db_config['port'],
                                                                       db_config['db'])

    engine = create_engine(connection_string, connect_args={'sslmode':'require'})


And the connection is stored in the 'engine' variable. We can run SQL queries using Pandas:

    pd.io.sql.read_sql(query, con = engine)


    But before we load the codes above, we should download the files of 'https://storage.yandexcloud.net/cloud-certs/CA.pem' to the loading folder 'file .ipynb' (which the use is when working with the database).

Here are the data descriptions of the database code files path above:

1) 'books' tables contains the books datas which consisting of:
a. 'book_id' — book ID
b. 'author_id' — author ID 
c. 'title' — title of the books
d. 'num_pages' — number of pages
e. 'publication_date' — publication date (the date the books were published)
f. 'publisher_id' — publisher ID

2) 'authors' tables contains the authors datas which consisting of:
a. 'author_id' — author ID
b. 'author' — authors' name

3) 'publishers' tables contains the publishers datas which consisting of:
a. 'publisher_id' — publisher ID
b. 'publisher' — publishers' name

4) 'ratings' tables contains the user reviews datas which consisting of:
a. 'rating_id' — rating ID
b. 'book_id' — book ID
c. 'username' — the username that rated the books
d. 'rating' — standardized assessment by user reviews (in scale 1-5 points)

5) 'reviews' tables contains the customers reviews datas which consisting of:
a. 'review_id' — review ID
b. 'book_id' — book ID
c. 'username' — the name of the user who reviewed the books
d. 'text' — review text


2. Data Study (Step 2. Studying The Tables)
In this stage, we will check and ensure for the 'books' Tables, 'authors' Tables, 'publishers' Tables, 'ratings' Tables, and 'reviews' Tables. We will study the tables coherently and thorough.


3. Explorative Data Analysis (EDA) (Step 3. Performing SQL Queries for Several Tasks)
In this stage, there are several things that need to be our focus, namely:

    a. Computing the number of books released after January 1, 2000
    b. Computing the number of user reviews and the average rating for each book
    d. Identifying the publisher that has published the most number of books, with more than 50 pages
    - (This will assist us in excluding brochures and similar publications from the analysis).

    e. Identifying authors with the highest average book rating
    - (Finding books with the rating of at least 50).
    
    f. Computing the average number of review texts among users who have rated more than 50 books


4. Presentation (Step 4. Presenting My Project to The Clients)
In this stage, I will present My Project to The Clients.


5. General Conclusions and Recommendations (Step 4. Formulating General Conclusions and Recommendations for Working with Customers)
In this stage, we will draw the conclusions and formulate the recommendations.

## libraries
_pandas_
_numpy_
_create_engine_



