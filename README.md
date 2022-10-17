# Data-Modeling-with-Postgres
## introduction
In this project, we'll apply data modeling with Postgres and build an ETL pipeline using Python to help startup called Sparkify that wants to analyze the data they've been collecting on songs and user activity on their new music streaming app,The analytics team is particularly interested in understanding what songs users are listening to Currently, but there is a problem which is the data is in directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app,so we are going to make etl process to get that data and insert it in database in 

## analytical goals
is to easy access what songs users are listening to Currently

## How to run the Python scripts
by opening terminal and execute python file script, example(root@2f19dda6469b:/home/workspace# python create_tables.py)

## An explanation of the files in the repository
* sql_queries.py :have all queries of drop ,create,insert tables that we will use in create_tables.py and etl.py
* create_tables.py :this file create the database and make connection then make functions to drop all tables uses  drop tables queries in sql_queries.py ,and make functions to create all tables uses creates queries in sql_queries.py 
* etl.pynb : this file is like tutorial to helps you make etl process and complete etl.py
* etl.py :makes functions to make etl process like extract data from directories and insert it in database uses inserts queries in sql_queries.py
## ERD of the database
![ERD](https://github.com/ahmedaalli/Data-Modeling-with-Postgres/blob/main/sparkify%20ERD.png)
