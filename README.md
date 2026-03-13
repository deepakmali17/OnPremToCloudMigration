# OnPremToCloudMigration

Azure Data Engineering Project – Airline Booking Analytics (Medallion Architecture)
Project Overview

This project demonstrates an end-to-end Azure Data Engineering pipeline built using Azure Data Factory (ADF) and Azure Data Lake Storage Gen2 following the Medallion Architecture (Bronze, Silver, Gold) pattern.

The pipeline ingests data from multiple on-premises and API sources, stores raw data in the Bronze layer, performs data cleansing and transformation in the Silver layer, and generates business-level analytics in the Gold layer.

The final datasets enable analytical insights such as top earning airlines and total flights per airline for reporting and business intelligence.


--- Data Sources ---

The pipeline integrates data from multiple heterogeneous sources:

On-Prem File System
DimAirlines.csv
DimFlight.csv
DimPassenger.csv

API Source
DimAirport.json

On-Prem SQL Database
FactBooking table from Microsoft SQL Server

A Self-Hosted Integration Runtime (SHIR) is used to securely connect on-premises systems with Azure Data Factory.


--- Business Insights Generated ---

The Gold layer provides datasets for analytical reporting such as:

Top 3 revenue-generating airlines
Total flights operated by each airline
Airline revenue summary
Booking analytics

These datasets can be easily connected to visualization tools like Power BI for dashboard creation.

--- Learning Outcomes ---

This project demonstrates practical implementation of:

Azure data ingestion pipelines
Medallion architecture
Data lake design principles
Data transformation using ADF Data Flows
Building scalable cloud data engineering solutions