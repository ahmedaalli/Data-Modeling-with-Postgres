# Data-Modeling-with-Postgres
## introduction
In this project, we'll apply data modeling with Postgres and build an ETL pipeline using Python to help startup called Sparkify that wants to analyze the data they've been collecting on songs and user activity on their new music streaming app,The analytics team is particularly interested in understanding what songs users are listening to Currently, but there is a problem which is the data is in directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app,so we are going to make etl process to get that data and insert it in database in 

## analytical goals
is to easy access what songs users are listening to Currently

## How to run the Python scripts
by opening terminal and execute python file script, example(python create_tables.py)

## An explanation of the files in the repository
* sql_queries.py :have all queries of drop ,create,insert tables that we will use in create_tables.py and etl.py
* create_tables.py :this file create the database and make connection then make functions to drop all tables uses drop tables queries in sql_queries.py ,and make functions to   create all tables uses creates queries in sql_queries.py 
* etl.pynb : this file is like tutorial to helps you make etl process and complete etl.py
* etl.py :makes functions to make etl process like extract data from directories and insert it in database uses inserts queries in sql_queries.py### Song Dataset

## Song Dataset
The first dataset is a subset of real data from the Million Song Dataset. Each file is in JSON format and contains metadata about a song and the artist of that song. The files are partitioned by the first three letters of each song's track ID. For example
```
song_data/A/B/C/TRABCEI128F424C983.json
song_data/A/A/B/TRAABJL12903CDCF1A.json
```

![songdata](https://github.com/ahmedaalli/Data-Modeling-with-Postgres/blob/main/images/songdata.png)


## log Dataset
The second dataset consists of log files in JSON format generated by this event simulator based on the songs in the dataset above. These simulate activity logs from a music streaming app based on specified configurations.

The log files in the dataset you'll be working with are partitioned by year and month. For example
```
log_data/2018/11/2018-11-12-events.json
log_data/2018/11/2018-11-13-events.json
```

![logdata](https://github.com/ahmedaalli/Data-Modeling-with-Postgres/blob/main/images/logdata.png)

## Schema Design ERD
![ERD](images/ERD.png)
