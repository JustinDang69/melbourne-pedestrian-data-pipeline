# Melbourne Pedestrian Data Pipeline

An end-to-end data engineering and analytics project using Melbourne pedestrian-count data, built with AWS S3, Snowflake, SQL and Tableau.

## Project Overview

This project builds a data pipeline for processing and analysing pedestrian-count data from the City of Melbourne.

The dataset contains approximately **1.6 million pedestrian-count records**. The project covers the workflow from raw data ingestion through data cleaning, transformation, analytical querying and dashboard visualisation.

The main objective was to turn a large raw dataset into structured and useful information that could be explored through SQL and an interactive Tableau dashboard.

## Architecture

```text
City of Melbourne Dataset
          |
          v
       AWS S3
          |
          v
      Snowflake
   ┌─────────────┐
   │ RAW Layer   │
   └──────┬──────┘
          |
          v
   Data Cleaning &
   Transformation
          |
          v
 ┌─────────────────┐
 │ Analytics Layer │
 └────────┬────────┘
          |
          v
       Tableau
          |
          v
 Interactive Dashboard
