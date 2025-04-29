# 🚖 NYC Taxi Trip Data Analytics Pipeline

This project demonstrates a complete end-to-end data pipeline for ingesting, transforming, storing, and visualizing NYC Taxi Trip data using Microsoft Azure services and Power BI. It follows best practices in Big Data architecture using tools like Azure Data Factory, Databricks, Delta Lake, and Azure Blob Storage.


## 📌 Table of Contents
- [Project Overview](#project-overview)
- [Architecture](#architecture)
- [Tech Stack](#tech-stack)
- [Data Source](#data-source)
- [Data Pipeline Stages](#data-pipeline-stages)
- [Final Dashboard](#final-dashboard)



## Project Overview

This project showcases how to build a scalable big data analytics solution using Azure services. It ingests trip data from the NYC Taxi open dataset, processes it with Apache Spark on Azure Databricks, stores it efficiently with Parquet and Delta Lake formats, and visualizes insights using Power BI.


## Architecture

![Image](https://github.com/user-attachments/assets/eb6176c6-a50c-42f4-962d-a7736744d7d9)


## Tech Stack

- **Data Ingestion:** Azure Data Factory
- **Data Transformation:** Azure Databricks (Apache Spark)
- **Data Storage:** Azure Blob Storage with Parquet and Delta Lake formats
- **Data Visualization:** Power BI
- **Security:** Access Keys for secure Blob access


## Data Source

We use the publicly available **NYC Taxi Trip Records** provided by the New York City Taxi & Limousine Commission (TLC).

🔗 [NYC Taxi Trip Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)


## Data Pipeline Stages

1. **Ingestion:**  
   Azure Data Factory pulls data from NYC TLC API into Azure Blob Storage (Raw Layer) in Parquet format.

2. **Transformation:**  
   Azure Databricks cleans and transforms raw data and saves it in the Transformed Layer as optimized Parquet files.

3. **Serving:**  
   The curated dataset is stored in Delta Lake format in the Serving Layer, ready for analysis.

4. **Visualization:**  
   Power BI connects directly to Delta Lake to create meaningful, real-time dashboards.


## Final Dashboard
![Image](https://github.com/user-attachments/assets/9bc31d73-5206-4fe4-8eda-6c8d546b7adc)

This NYC Taxi dashboard summarizes 2023 trip data, highlighting key metrics like total rides (787K), revenue ($18.78M), and average trip distance (19.02 miles). It shows that **Vendor 2 dominates** trip volume, **Thursdays see the most rides**, and **revenue peaks in March and September**. A map visualizes pickup hotspots, mostly in North America. The dashboard offers clear insights into vendor performance, daily trends, and monthly revenue patterns.
