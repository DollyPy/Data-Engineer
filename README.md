# Data Engineer Test

This repository was created to answer the  data engineer test questions.

## Introduction

Inorder to achieve the set objectives for this project, the following processes were duely followed
## Data Extraction
Different Data were extracted from the given repository which represents the following 
- Countries
- Languages
- Continents

The files are in JSON format, however, they were converted into DataFrame with the use of pandas

## Data Transformation
The collected data were transformed as follows:
- Name column in countries was changed to country
- Continents column in countries was dropped as only a few rows contained that data
- Continent name was transformed from abbreviation to Full name
- An extra column was added to show the number of languages spoken in each country
- From Countries dataset, language coloumn was extracted to create new Dataset which included only language and Countries Speaking the language
- The data from the languages dataset was used to give the full name of each language from the new Language dataset

## Loading of Data to postgreSQL database
- A new database with the name `DataEngineer` was created in postgres
- A user user named `sample` was also included for the purpose of this
- Connection was made to the postgresql db via `sqlalchemy` after supplying the necessary login credentials
- Two tables were created in the database `countries` and `languages` using the dataset from the data transformation phase

## Querying Data from the database
- Connection to the database was done using `psycopg2`
- Queries were written with reqular python strings
- The execute function was called and the results were displayed thereafter
## Reporting Result 
- The answers from the queries were documented using excel
- screenshots of snippets and results were taking

## Tools/Resources Used
- Jupyter Notebook (Anaconda)
- Python Programming language
- PostgreSQL database
- Pandas
- Sqlalchemy
- psycopg2
- Microsoft Excel