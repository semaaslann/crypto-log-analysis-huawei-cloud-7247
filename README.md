# Real-Time Crypto Log Analysis on Huawei Cloud

## Description

This project sets up a real-time log analysis pipeline on Huawei Cloud for crypto trading data. It uses Huawei Cloud's LTS for log ingestion, OBS for storage, MRS (Spark) for data processing and anomaly detection, and a basic dashboard for visualization.

## Architecture

The architecture consists of the following components:

*   **Data Source:** Crypto exchanges that generate trading logs.
*   **Log Service (LTS):** Huawei Cloud's log collection service ingests logs from the data source.
*   **Object Storage Service (OBS):** Stores the ingested logs.
*   **MRS (Spark):** Processes the logs from OBS, performs anomaly detection, and prepares data for visualization.
*   **Visualization Dashboard:** A simple dashboard displays the processed data and detected anomalies.

## Setup

1.  Install Docker and Docker Compose.
2.  Clone this repository.
3.  Run `docker-compose up -d` to start the services.

Note:  This MVP uses a local Spark setup for demonstration purposes. In a production environment, you would replace the Dockerized Spark with a proper MRS cluster on Huawei Cloud.  Also, the data sources (exchanges, APIs), LTS configurations, OBS buckets, and MRS configurations need to be set up on Huawei Cloud.
