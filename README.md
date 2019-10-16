# Data Modelling with Postgres
> 
In this project I am taking on the role of a Data Engineer to create a database schema and an ETL pipeline for a fictional startup called Sparkify. The database schema is created on Postgres database for optimal queries on song plays. The ETL pipeline consists of functions to load JSON logs and metadata related to app user activity as well as information about songs in the app, to a Fact table and several Dimension tables in the Postgres Database.

The project tasks involved the design of fact and dimension tables for a star schema and the development of Python and SQL scripts to create an ETL pipeline that transfers data from files in two local directories into tables in Postgres.

## Table of contents

* [Database design](#summary-of-results)
* [Data and Code](#data-and-code)
* [Prerequisites](#prerequisites)
* [Instructions on running the application](#instructions-on-running-the-application)

## Schema for Song Play Analysis
Using the song and log datasets, a star schema optimized for queries on song play was analysis was created based on the following entity relationship diagram:
![ERD image](/songplays erd.png)

## Data and Code
* The main analysis is contained in the 2019 Stack Overflow Survey Analysis.ipynb jupyter notebook. All the functions and code, as well as the rationale behind decisions taken is contained in this notebook.

Data for the analysis is available at: [survey datasets](https://insights.stackoverflow.com/survey)
## Prerequisites
* Numpy
* Pandas
* seaborn
* Matplotlib

Jupyter notebook and python 3.6 are needed to run the notebooks and python scripts.

## Instructions on running the application
1. Download the required data sets and if required modify the directory paths.

