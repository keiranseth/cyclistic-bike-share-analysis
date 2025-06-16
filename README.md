# Cyclistic Bike-Share Analysis

This data analysis project is my attempt at tackling the Google Data Analytics Professional Certificate's first case study, Cyclistic Bike-Share analysis.

## Project Deliverables

### Statement of the business task

With the ultimate goal of increasing annual memberships, our goal as the analytics team is to determine and understand the difference between how annual members and casual riders use Cyclistic's services. Answering this difference may help the company convince casual riders into becoming members.

#### Problem Statement for the Analytics Team

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

See the [final data analysis report](./report/report.pdf).

See the [preliminary analysis report](./preliminary/preliminary_analysis.md).

### Summary of Analysis and Final Recommendation

Here are the insights gathered by the analytics team.

1. There as more members (at least twice as many as) than casual riders.
2. Classic bikes are used by more than half of the rides in 2024. Electric bikes cover one-third. Electric scooters are rarely used.
3. Across membership types, insight 2 still holds. However, note that among riders who used electric scooters, there are more casual riders than members.
4. The average ride duration is 16 minutes and 39 seconds. The total ride duration exceeds 1,000,000 hours.
5. On average, casual riders bike twice as long as members. They also dominate the total ride duration.
6. Across all membership types, insight 2 still holds, and casual riders bike twice as long as members.
7. Quarters 2 and 3 observe peaks in ride count and average ride duration.
    - Across all quarters, there are at least 100% more members than casuals, but casuals still ride twice as long as members.
    - Across all quarters, insight 2 still holds.
8. Ride counts are observed to peak from May to October, while ride durations are observed to peak from May to August.
    - Across all months, there are at least 100% more members than casuals, but casuals still ride longer than members.
    - Across all months, except for August, insight 2 still holds.
9. Average ride counts are observed to peak on Wednesday and Saturday, while average ride durations are observed to peak on the weekends (Saturday and Sunday).
    - Across all days of the week, there are more members on average than casuals, but casuals still ride twice as long as members.
    - Across all days of the week, insight 2 still holds.

From these insights, let us now answer the problem statement.

> **How do annual members and casual riders use Cyclistic bikes differently?**

-   Annual members dominate the ride count across bicycle types, and across all quarters, months, and in any day of the week.
-   Casual riders dominate the average ride duration across bicycle types, and across all quarters, months, and on any day of the week.
-   The average ride duration of annual members is more or less within 12 to 14 minutes across all quarters, months, and on any day of the week.
-   The average ride duration of casual riders is more or less within 14 to 28 minutes across all quarters, months, and on any day of the week.
-   In the use of electric scooters in August and September, there are more casual riders than annual members.

After finding out that casual riders bike twice as long as annual members, the analytics team mainly recommends more research on why this is so. Although we can formulate the following hypotheses:

-   **Casual riders use the bike-share service for leisurely bike rides or for cycling exercise, especially on the weekends.**
-   **Annual members use the bike-share service for utility and transportation/commute, especially on the weekends.**

**_The analytics team cannot assess, or even support the veracity of these hypotheses from the current data we are given, unless we have more comprehensive data in the form of brief surveys and questionnaires to our entire consumer base._** Hopefully, with more comprehensive data for next year, the analytics team can uncover deeper insights.

The main, but tentative, recommendation from the analytics team is:

> **Create annual pricing plans tailored for prospective bikers and scooters who ride either for leisure and scenery rides, or for exercise, such as long-distance cycling.**

Since the analytics team also looked at quarterly and monthly trends of the ride duration and average ride count, another recommendation by the analytics is:

> **Increase or emphasize advertising for the months May to October, or quarters 2 and 3, using tailored pricing plans for leisure, recreation, or exercise to casual riders.**
