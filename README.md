# **Spotify_ETL_Project**
## Introduction
In this project, an ETL pipeline is developed using the Spotify API. The process involves retrieving data from the Spotify API, transforming it into the required format, and then loading it into an AWS data store.

## Architecture
![Architecture(Spotify_ETL_Project)](https://github.com/user-attachments/assets/4e9fd077-8d00-4cbe-aa56-d145ffc4c7dd)

## Dataset/API
The Spotify API will provide information about music artists, albums, and songs.

## AWS Services Used
1) Storage(Amazon S3)

2) Compute(AWS Lambda)

3) Logs/Trigger(Amazon Cloudwatch)

4) Data Crawler(Crawler)

5) Data Catalog(AWS Glue Data Catalog)

6) Analytics Query(Amazon Athena)

## Project Execution Flow

1. **Connecting to Spotify API and Extracting Data**
   - Establish a connection to the Spotify API to obtain data on the Top 100 most streamed songs.

2. **Deploying Code on AWS Lambda for Data Extraction**

3. **Setting Up Automatic Extraction Triggers**
   - Configure an AWS CloudWatch event to automatically trigger the Lambda function every hour.

4. **Creating the Transformation Function**

5. **Automating the Transformation Process**

6. **Properly Storing Files on S3**
   - Store both raw and transformed data in organized Amazon S3 buckets.
   - Implement lifecycle policies to optimize data storage costs.

7. **Creating Analytics Tables with Glue and Athena**
   - Set up AWS Glue crawlers to catalog the data stored in S3.
   - Utilize Amazon Athena to create and query analytics tables for insights.
