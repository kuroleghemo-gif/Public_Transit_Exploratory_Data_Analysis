# Public_Transit_Operations_Analytics

<img width="2875" height="3834" alt="valentyn-chernetskyi-m0_o8QB-JGg-unsplash" src="https://github.com/user-attachments/assets/8263da70-816c-4e0b-958a-6e1d43cc2590" />




## Table of Content
##### • [Project Overview](#project-overview)
##### • [Project Objectives](#project-objectives)
##### • [Data Sources](#data-sources)
##### • [Data Preprocessing](#data-preprocessing)
##### • [Key Insights](#key-insights)
##### • [Tools and Skills](#tools-and-skills)
##### • [Recommendations](#recommendations)

## Project Overview
This project analyzes trip records from a multi-modal public transit network operating across multiple cities. The dataset contained messy, inconsistent, and incomplete records. The goal was to clean, explore, and extract actionable insights to support operational decision-making around passenger demand, fare structure, and transport mode performance.

## Project Objectives
##### • Clean and preprocess the dataset to ensure data quality
##### • Perform univariate, bivariate, and multivariate EDA
##### • Compute descriptive statistics to summarize key metrics
##### • Create visualizations that effectively communicate findings
##### • Deliver actionable recommendations for operations

## Data Source
The dataset was provided by 10Alytics as part of their Data Analytics training program. It contained 1000 rows of trip records extracted from a public transit company. Features include unique trip identifier, mode of transport, departure station, arrival station, departure time, fare amount, passenger count, trip duration, day of the week, hour and route.

## Data Preprocessing
Right before anaysis, an extensive data cleaning and preprocessing was done . The dataset had inconsistent text formatting, whitespace errors, and two unnamed redundant columns that were dropped. Missing values in passenger count, fare amount, and trip duration were assessed, found to follow a missing at random pattern, and filled using grouped median imputation. Two new features, hour of day and route, were engineered to support the analysis.

## Key Insights
##### • Bus was the most used mode (33.2%) while trams were significantly underutilized (13.8%)
##### • Sunday had the highest trip volume and Thursday had the lowest yet generated the highest revenue
##### • Passenger demand peaked at 8 AM and 9 PM, with a sharp dip at 11 AM
##### • Bus demand peaked 5–9 PM, ferries at 8 AM, trains at 7 AM and 2 PM, trams were underutilized across all hours
##### • Central station handled the highest trips and revenue, South Point had the lowest across all metrics
##### • Trains underperformed on speed on several occasions compared to other modes for the same routes
##### • Trip demand, passenger volume, and revenue all fluctuate day-to-day with no clear upward or downward trend

## Tools and Skills
• Programming Language: Python
• Libraries:
- Pandas for data manipulation and cleaning,
- Matplotlib and Seaborn for data visualization,
- Missingno for missing data visualization.
• Environment: Jupyter Notebook

## Recommendations
**1. Capacity & Scheduling**
- Increase bus capacity during late afternoon and evening (5–9 PM)
- Use historical trip data to anticipate demand shifts and adjust service levels accordingly
- Trim tram scheduling and use targeted incentives to address consistent underutilization

**2. Route Optimization**
- Review train scheduling and stopping patterns on underperforming routes to identify and fix the cause of delays
- Introduce express train services on routes where trains are slower than buses or trams

**3. Pricing & Demand**
- Investigate and align fares with demand; Thursday's highest revenue on the lowest-demand day indicates pricing inconsistencies that need review
- Implement targeted interventions at South Point (discounted fares or loyalty rewards) to stimulate usage
