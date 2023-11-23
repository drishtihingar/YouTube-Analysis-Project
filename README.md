# YouTube-Analysis-Project
YouTube Analysis Project - End-to-End Data Engineering utilizing AWS Cloud and Python


**Project Title:** YouTube Analysis Project - End-to-End Data Engineering utilizing AWS cloud and Python

**Project Overview:**
This project is designed to securely handle, streamline, and analyze structured and semi-structured data from YouTube videos. It focuses on categorizing videos and assessing trending metrics to derive meaningful insights.

**Project Objectives:**
📌 Data Ingestion
📌 ETL System
📌 Data Lake Implementation
📌 Scalability Assurance
📌 Cloud Integration (AWS)
📌 Reporting Dashboards

**Pipeline Phases:**
The project unfolds in three key phases:

**📌 Extract:**
- Data extraction from Kaggle, featuring daily statistics of popular YouTube videos.
- AWS Lambda deployment for extraction function.
- Automated extraction triggered by AWS CloudWatch at regular intervals.
- Raw data stored in AWS S3 Bucket under "de-on-youtube-raw-ind-dev."

**📌 Transform:**
- S3 triggers activating a Lambda function for data transformation.
- Categorized data by region, moved from "de-on-youtube-raw-ind-dev" to "de-on-youtube-cleansed-ind."

**📌 Load:**
- Glue Crawler for schema inference upon new data addition.
- Amazon Athena renders the final dataset queryable and analyzable.
