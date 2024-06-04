# Home_Sales

Overview

This project utilizes Apache Spark and Spark SQL to perform data analysis on a dataset of home sales. The analysis includes various SQL queries to derive insights such as average prices based on different criteria.

Requirements

Apache Spark 3.x

Java 11

- Setup
  
-the desired Spark version was set by updating the spark_version variable in the script.
-the provided script was run to install Spark, Java, and other necessary packages.
-a SparkSession was started to interact with Spark SQL.
-the dataset was read from AWS S3 bucket and created a temporary view of the DataFrame.
-SQL queries to analyze the data was performed.

- Queries
  
-Average Price for Four Bedroom Houses per Year: Calculated the average price for four-bedroom houses sold per year.

-Average Price of Homes Built per Year: Determined the average price of homes for each year they were built, with specific bedroom and bathroom configurations.

-Average Price of Homes Built per Year with Additional Criteria: Calculated the average price of homes per year they were built, considering additional criteria such as floors and square footage.

-Average Price of Homes per View Rating: Computed the average price of homes per view rating, filtering for prices greater than or equal to $350,000. Also measures the runtime for the query.

-Caching and Performance Comparison: Demonstrated caching of the dataset and compares the runtime of a query with and without caching.

-Partitioning and Parquet Data: Partitioned the data by date_built and saves it in Parquet format. Reads the Parquet data, creates a temporary table, and performs a query similar to the previous one to compare runtime with cached data.

- Usage
-Executed the provided script in a Spark environment.

-Reviewed the output of each SQL query to gain insights into the dataset.

-Experimented with additional queries or modifications to suit specific analytical needs.
