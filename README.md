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


## Technologies Used

- SQL
- Snowflake
- Amazon S3
- Tableau
- Data cleaning and transformation
- Data quality validation
- Analytical querying
- Data visualisation

## Key Features

### Data Ingestion

The raw pedestrian-count dataset was staged for loading into Snowflake.

The workflow included:

- External data staging
- File format configuration
- Schema inspection and inference
- Loading data using Snowflake `COPY INTO`

### Data Processing

The project separated raw and analytical data into different layers.

Data processing included:

- Data type validation
- Missing-value and data-quality checks
- Cleaning raw records
- Creating structured analytical datasets
- Preparing data for reporting and visualisation

### SQL Analytics

SQL queries were developed to explore pedestrian activity and identify patterns in the dataset.

Techniques used included:

- Common Table Expressions (CTEs)
- JOIN
- Aggregation
- Filtering
- Ranking
- `DENSE_RANK()`
- Data-quality queries

One analysis focused on identifying the busiest pedestrian locations based on recorded pedestrian activity.

## Tableau Dashboard

A Tableau dashboard was developed to make the processed pedestrian data easier to explore visually.

The dashboard provides an interactive way to investigate pedestrian activity and compare patterns across locations and time periods.

## Repository Contents

### `pedestrian_data_pipeline.sql`

Contains the Snowflake SQL used for:

- Environment setup
- Data loading
- Data cleaning
- Data-quality validation
- Analytical queries
- Ranking pedestrian locations

### `pedestrian_dashboard.twb`

Tableau workbook containing the dashboard developed for the project.

### `project_presentation.pptx`

Presentation material used to demonstrate the project workflow and results.

## Skills Demonstrated

- End-to-end data pipeline development
- Working with large datasets
- Cloud-based data storage
- Snowflake data warehousing
- SQL transformation and analytics
- Data quality validation
- Tableau dashboard development
- Communicating analytical results

## Dataset

The project uses pedestrian-counting data published by the City of Melbourne.

The original dataset is not included in this repository due to its size.

## Project Context

This project was completed as part of NIT2202 at Victoria University.

It involved implementation and live demonstration of the data pipeline, SQL analysis and Tableau visualisation.

## Future Improvements

- Automate data ingestion
- Add scheduled data refreshes
- Expand time-based and location-based analysis
- Add predictive modelling for pedestrian traffic
- Develop a more automated ELT workflow

## Author

Justin Dang

Bachelor of Data Science  
Victoria University
