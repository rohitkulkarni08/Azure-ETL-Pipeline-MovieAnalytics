# End-to-End ETL Pipeline with Microsoft Azure for IMDb Movie Rating Dataset

## Overview

This project focuses on building a comprehensive Extract, Transform, and Load (ETL) pipeline leveraging the robust functionalities of Microsoft Azure. The pipeline is designed to efficiently fetch data from Azure Blob Storage perform necessary transformations using Azure Databricks and Azure Data Factory, store it in Azure Data Lake and finally store the analyzed data in a SQL layer for further use. This end-to-end solution aims to streamline the data processing workflow and provide actionable insights from the transformed data.

## Dataset

The [Dataset](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset) used in this project contains information for over 45,000 movies with 26 million ratings! Since this is primarily a Data Engineering project, we'll only be focusing on one of the datasets "movies-metadata" which contains information such as budget, revenue, release dates, languages, production countries and companies.

## Prerequisites

1. **Microsoft Azure subscription**
2. **Azure Blob Storage**: Object storage service for storing large amounts of unstructured data
3. **Azure Data Lake Gen2 Storage**: Scalable storage for big data analytics
4. **Azure Databricks**: Analytics platform based on Apache Spark for big data processing and machine learning
5. **Azure SQL Server**: Fully managed relational database service with SQL Server engine
6. **Azure SQL Database**: Managed relational database with SQL Server compatibility
7. **Azure Data Factory**: Data integration service that enables you to create, schedule, and orchestrate ETL and ELT workflows. ADF provides a visually intuitive interface to build data-driven workflows for orchestrating data movement and transforming data at scale

<img src="https://github.com/rohitkulkarni08/Azure-ETL-Pipeline-MovieAnalytics/blob/a0e8db3a6c03ef87bdfc023cd12e7c31da40ff17/images/azure_resource_group.png" width="1100" height="550">

## Data flow:

1. **Extract Data**: Retrieve CSV data from Azure Blob Storage for processing.
2. **Transform Data**: Utilize Python and PySpark on Azure Databricks to analyze and process the data, storing the results in Azure Data Lake Storage Gen2.
3. **Load Data**: Transfer the processed data into an Azure SQL database to establish a reporting layer for dashboard creation.
4. **Automation**: Construct end-to-end pipelines in Azure Data Factory to automate the data flow from extraction to reporting.

<img src="https://github.com/rohitkulkarni08/Azure-ETL-Pipeline-MovieAnalytics/blob/a0e8db3a6c03ef87bdfc023cd12e7c31da40ff17/images/azure_resource_group.png">

