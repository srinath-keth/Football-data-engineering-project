# Football-data-engineering-project

This Python-based project is designed to automate the end-to-end data pipeline for extracting, transforming, and loading (ETL) football-related data. Using Apache Airflow, the project crawls historical and real-time football data from Wikipedia, applies cleaning and transformation processes, and stores the results in Azure Data Lake for further analysis and reporting. This project demonstrates a modern data engineering workflow by integrating tools like Docker, PostgreSQL, and Airflow to handle data pipelines efficiently.

The key objective is to create a scalable, reproducible, and maintainable data engineering framework that can be extended for various sports analytics use cases. The cleaned and transformed data can be utilized for downstream applications such as business intelligence dashboards, machine learning models, or interactive visualizations.

# Key Features:

** Automated Data Collection: Uses Python and Apache Airflow to fetch football data from Wikipedia.
** Data Cleaning and Transformation: Standardizes raw data for consistency and accuracy.
** Cloud Integration: Pushes processed data to Azure Data Lake for storage and further analytics.
** Containerized Workflow: Deployable as a Dockerized application for consistency across environments.
** Scalability: Designed to handle growing datasets and adapt to different sources with minimal changes.

## Table of Contents

1. [System Architecture](#system-architecture)
2. [Requirements](#requirements)
3. [Getting Started](#getting-started)
4. [Running the Code With Docker](#running-the-code-with-docker)
5. [How It Works](#how-it-works)


## System Architecture
![system_architecture.png](assets%2Fsystem_architecture.png)

## Requirements
- Python 3.9 (minimum)
- Docker
- PostgreSQL
- Apache Airflow 2.6 (minimum)

## Getting Started

1. Clone the repository.
   ```bash
   git clone https://github.com/airscholar/FootballDataEngineering.git
   ```

2. Install Python dependencies.
   ```bash
   pip install -r requirements.txt
   ```
   
## Running the Code With Docker

1. Start your services on Docker with
   ```bash
   docker compose up -d
   ``` 
2. Trigger the DAG on the Airflow UI.

## How It Works
1. Fetches data from Wikipedia.
2. Cleans the data.
3. Transforms the data.
4. Pushes the data to Azure Data Lake.
