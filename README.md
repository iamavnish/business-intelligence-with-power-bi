# Visualizing Credit Card Defaults using Power BI

## Overview 

This is Proof of Concept for loading, transforming and visualizing data through Power BI.

## Report Screenshot

![image](https://github.com/user-attachments/assets/2b15d145-a7ff-46fc-9ced-457cdeb90bd6)


## Tech Stack

- Power BI Desktop

## Dataset

Credit Card Defaults (UCI Machine Leaarning DataSet Repository). New Column added to original dataset (fake geo-location information for various US states).

## Solution

Lambda function is triggered once a day through CloudWatch Events which extracts data for top 50 global songs on Spotify through Spotify API and stores in S3 bucket in JSON format. Another Lambda function gets triggered whenever a new file is added to S3 bucket (first S3 bucket). This second lambda function does some transformations on the raw data like extracting albums data, artists data and songs data and storing the transformed data into second S3 bucket in CSV format. Schema is inferred from CSV files through Glue Crawlers and corresponding metadata is stored in Glue Data Catalog. Then anaytics can be performed on top of CSV files in second S3 bucket using Athena service. Finally, a dashboard is built using QuickSight to visualize data such as "Top 5 Global Artists on Spotify" using Athena as Data Source.




