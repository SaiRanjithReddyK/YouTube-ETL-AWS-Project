# Data Engineering YouTube Analysis Project with AWS

## Overview

This project explores how to build a real-world, cloud-based data engineering pipeline to process and analyze structured and semi-structured YouTube data. The goal is to simulate a scalable architecture that can handle growing datasets, automate transformations, and provide insights through querying and visualization. It brings together multiple AWS services to create an end-to-end workflow, from raw ingestion to reporting.

## Project Objectives

1. **Data Ingestion** – Design a mechanism to collect YouTube data from external sources (e.g., public datasets).
2. **ETL Processing** – Clean and transform raw CSV and JSON data into a usable format using automated scripts and serverless functions.
3. **Data Lake** – Store raw and processed data in a centralized and durable S3-based data lake.
4. **Scalability** – Build a solution that adapts easily to increasing data volume without requiring infrastructure changes.
5. **Cloud-Based Execution** – Use AWS tools to eliminate dependency on local machines and enable high-availability, serverless processing.
6. **Visualization & Reporting** – Deliver dashboards that provide insights into YouTube trends, user engagement, and category-level performance.

## AWS Services Used

- **Amazon S3** – Stores raw and transformed datasets in a structured format.
- **AWS IAM** – Manages secure permissions for accessing AWS resources within the pipeline.
- **AWS Glue** – Automates data discovery, transformation, and schema creation for downstream querying.
- **AWS Lambda** – Runs lightweight ETL scripts triggered by events without needing servers.
- **Amazon Athena** – Enables querying the processed data directly from S3 using SQL.
- **Amazon QuickSight** – Provides a business intelligence layer for visualizing YouTube metrics and engagement trends.

## Dataset Source

We use the popular [YouTube Trending Videos Dataset on Kaggle](https://www.kaggle.com/datasets/datasnaek/youtube-new), which contains daily records of trending YouTube videos from multiple regions.

Each record includes:
- Video metadata (title, channel, publish time)
- Engagement metrics (views, likes, dislikes, comment count)
- Category and region information
- Tags and video descriptions

The dataset also includes a JSON file mapping `category_id` to human-readable names per region.

## Architecture Diagram

This high-level diagram outlines the flow from ingestion to analysis:

![Architecture Diagram](architecture.jpeg)

## Key Outcomes

- Built an end-to-end pipeline to process and transform YouTube data in the cloud.
- Automated data transformation using serverless Lambda functions and PySpark.
- Queried enriched datasets through Athena without manual loading.
- Delivered insights through QuickSight dashboards for trend and engagement analysis.
- Emulated real-world data engineering practices using scalable and cost-effective AWS services.

## Next Steps

- [ ] Add automated job orchestration using AWS Step Functions
- [ ] Integrate CloudWatch alerts for better observability
- [ ] Create a public QuickSight dashboard for demo access
- [ ] Add data validation and schema enforcement layer using Glue Data Catalog

## Author

**Sai Ranjith Reddy**  
[LinkedIn](https://www.linkedin.com/in/sai-ranjith-reddy-konda-reddy) | [GitHub](https://github.com/SaiRanjithReddyK)

---

**License**: MIT  
This project is open for learning, reuse, and extension. Feel free to fork and customize as needed.
