# Project: Data Modeling with Postgres

# Introduction

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

They'd like a data engineer to create a Postgres database with tables designed to optimize queries on song play analysis, and bring you on the project. Your role is to create a database schema and ETL pipeline for this analysis. You'll be able to test your database and ETL pipeline by running queries given to you by the analytics team from Sparkify and compare your results with their expected results.

## Project Description

In this project, you'll apply what you've learned on data modeling with Postgres and build an ETL pipeline using Python. To complete the project, you will need to define fact and dimension tables for a star schema for a particular analytic focus, and write an ETL pipeline that transfers data from files in two local directories into these tables in Postgres using Python and SQL.

## Star Schema

A Star Schema was created, it contains a Fact Table `songplays`and 4 Dimension Tables:
1. `users`, user in the app
2. `songs`, songs in music database
3. `artists`, artists in music database
4. `time`, timestamps of records in songplays broken down into specific units

## How it works

This project makes the folowing assumptions:

* Python 3 is available
* `pandas` is available
* A PosgreSQL database is available

## Running the Python Scripts

You have to launch the Terminal and run the `create_tables.py` file and then the `etl.py` file by writing:

1. python create_tables.py
2. python etl.py

## Files

### data

This directory contains two more directories, `data/log_data` and `data/song_data`. It contains the JSON files who we work with.

## create_tables.py

This Python file is used to create the tables to work with.

## etl.ipynb

This Jupyter notebook file is used to extract data and test the ETL process.

## etl.py

This Python file reads the log and song data and processes them into the database.

## README.md

This README file you're already reading.

## sql_queries.py

This Python file contains all the SQL queries.

## test.ipynb

This Jupyter Notebook file tests if all data is used correctly.