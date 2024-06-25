# Building an ETL Pipeline with Pandas and SQLite

This problem set is designed to introduce aspiring data engineers to the pandas library and its application in building an ETL (Extract, Transform, Load) pipeline.
The goal is to load video game data from a CSV file into a SQLite database. The challenges progress from basic data manipulation to more advanced techniques.

The video game sales dataset you're working with contains information on over 55,000 video games (as of April 2019). Here's a quick rundown:
Source: Scraped from vgchartz.com

Number of Records: 55,792

3 Problem Description
Imagine you're working for a video game market analysis company. Your company helps game developers and publishers understand sales trends, market demands, and the reception of their games across different regions. Your task is to build a robust ETL pipeline that can process large datasets, transform them into meaningful insights, and store them in a database for easy querying and analysis.

For instance, a game developer wants to know how their games have performed in different regions over the years and whether critic and user scores correlate with sales figures. By building this ETL pipeline, you enable the company to quickly answer such questions, aiding in strategic decision-making and improving the development of future games.
Basic Data Exploration (Easy)
Import libraries and load data:

Import pandas and sqlite3 libraries.

Load the video game data from the CSV file using pandas.read_csv.

Print the first few rows of the data to get a sense of its structure.

Data summary:

Get basic information about the data using df.info().

Describe the numerical columns using df.describe().

Check for missing values using df.isnull().sum().

Clean the data with diffrent pandas functions.

Data cleaning:

removing rows, imputing values 

Handle duplicates.

Check for and fix typos.

# Data Transformation 
Get Total Sales by summary of all region sales.
Data filtering:

Filter the data to include only games released after a specific year (e.g., 2010).

Filter the data to include only games with a Critic Score greater than a certain threshold (e.g., 8).

Data type conversion:

Convert the "Year" column from string to integer format.

Set column data types to appropriate formats.

# Building the ETL Pipeline
Establish connection to SQLite database using SQLAlchemy
Define a function for data loading
Create a function that takes the pandas DataFrame as input and establishes a connection to the SQLite database.
Use the to_sql method from pandas to write the DataFrame to a table named "games" in the database.
Load data into the database:
Call the data loading function with the prepared DataFrame.
Bonus: Enhance the pipeline with error handling and logging capabilities.

This ETL pipeline extract, clean and load the data to SQlite Database 
