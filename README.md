# Data Modelling with Postgres
> 
In this project I am taking on the role of a Data Engineer to create a database schema and an ETL pipeline for a fictional startup called Sparkify. The database schema is created on Postgres database for optimal queries on song plays. The ETL pipeline consists of functions to load JSON logs and metadata related to app user activity as well as information about songs in the app, to a Fact table and several Dimension tables in the Postgres Database.

The project tasks involved the design of fact and dimension tables for a star schema and the development of Python and SQL scripts to create an ETL pipeline that transfers data from files in two local directories into tables in Postgres.

## Table of contents

* [Database design](#Schema-for-Song-Play-Analysis)
* [Data and Code](#data-and-code)
* [Prerequisites](#prerequisites)
* [Instructions on running the application](#instructions-on-running-the-application)

## Schema for Song Play Analysis
Using the song and log datasets, a star schema optimized for queries on song play analysis was created based on the following entity relationship diagram:
![ERD image](/songplays_erd.png)

## Data and Code
In addition to the data files, the project workspace includes six files:
* **test.ipynb** displays the first few rows of each table to let you check your database.
* **create_tables.py** drops and creates database tables. This file is run on the command line to reset tables prior to running the ETL scripts.
* **etl.ipynb** reads and processes a single file from song_data and log_data and loads the data into database tables. This notebook contains detailed instructions on the ETL process for each of the tables.
* **etl.py** reads and processes files from song_data and log_data and loads them into the fact and dimension tables.
* **sql_queries.py** contains all the projects sql queries, and is imported into the last three files above.

## Prerequisites
* psycopg2
* Pandas
* glob
* os

Jupyter notebook and python 3 are needed to run the notebooks and python scripts.

## Instructions on running the application
1. Download the required data sets and if required modify the directory paths.

