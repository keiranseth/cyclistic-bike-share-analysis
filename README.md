# Cyclistic Bike-Share Analysis

This data analysis project is my attempt at tackling the Google Data Analytics Professional Certificate's first case study, Cyclistic Bike-Share analysis.

## Project Deliverables

### Statement of the business task

With the ultimate goal of increasing annual memberships, our goal as the analytics team is to determine and understand the difference between how annual members and casual riders use Cyclistic's services. Answering this difference may help the company convince casual riders into becoming members.

#### Central Problem for the Analytics Team

> **How do annual members and casual riders use Cyclistic bikes differently?**

### Description of Data Sources

As of June 2025, the analytics team will use 2024's entire [Cyclistic's bike trip data](https://divvy-tripdata.s3.amazonaws.com/index.html) spanning 12 months, which is made available by Motivate International Inc. under this [license](https://www.divvybikes.com/data-license-agreement).

See the [original dataset](https://drive.google.com/file/d/16wliXSMBTFmEKHfyWIAZ914GubXTE1bR/view?usp=drive_link) used for this project.

The dataset is partitioned by month, and _initially_ contains the following columns:

-   `ride_id` - unique identifier of the bike ride
-   `rideable_type` - type of bike used
-   `started_at` - starting datetime of the ride
-   `ended_at` - ending datetime of the ride
-   `start_station_name` - the name of the origin station
-   `start_station_id` - identifier of the origin station
-   `end_station_name` - the name of the destination station
-   `end_station_id` - identifier of the destination station
-   `start_lat` - latitude of the starting location
-   `start_lng` - longitude of the starting location
-   `end_lat` - latitude of the ending location
-   `end_lng` - longitude of the ending location
-   `member_casual` - membership type (`casual` or `member`)

Privacy regulations made it so that the data provided by Cyclistic do not contain any personally-identifiable information. Thus, there is no incriminating information such as names, government ID numbers, or addresses, just to name a few. Any included data respects the customer's data rights.

The data is credible, since the datasets are:

-   **Reliable** - relevant data is included in each ride,
-   **Original** - the datasets are provided by Cyclistic with a license,
-   **Comprehensive** - relevant data is provided by month, and there is data for each month of last year,
-   **Current** - the dataset includes last year's data, which may reveal trends within a Cyclistic's financial year, and
-   **Cited** - the data source is revealed with a license for permitted use.

### Documentation of Data Preparation

See the [data preparation process](./data_preparation.md).

### Data Analysis Report

See the final data analysis report.

See the [preliminary analysis report](./preliminary/preliminary_analysis.md).

### Summary of Analysis and Final Recommendation
