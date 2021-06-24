# MOVIES_ETL

## Overview

The purpose of this analysis was to create an automated pipeline that takes in new data, performs the appropriate transformations, and loads the data into existing tables. This pipeline is being created for the purposes of an Amazing Prime Hackathon event. Tne function was created that takes in the three files. The Wikipedia data was in a json format. The Kaggle metadata and the MovieLens rating data were in a csv format. The ETL process was perfomed that resulted in the addition of the data to a PostgreSQL database to later be used for analysis.

## Process and Results

### Write an ETL function to read the three data files 
This function takes the Wikipedia JSOn, the Kaggle metadata and the MovieLens csv files and creates three different DataFrames. 

### Extract and Transform the Wikipedia data 
The TV shows were filtered out, the redundant data was consolidated, and the rest of the data was formatted and grouped. 

### Extract and Transform the Kaggle and Rating data 
The rudundant data was consolidated, duplicates were removed, and the rest of the data was formatted and grouped. After these processes, the Kaggle and Rating data were merged with the Wikipedia movies DataFrame. 

### Load the data to a PostgreSQL Movie Database 
![ETL_process](/ETL_process.png)

## Summary 
An ETL function was created that collects and cleans movie data from various sources. It transforms and and merges the data. It then loads this data into two updatable PostgreSQL dataset tables. These tables achieve the goal of usage by hackathon participants for analysis. 


 
