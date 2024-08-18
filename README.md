# Cyclistic Bike-Share Analysis - Capstone Project. Google Data Analytics Professional Certificate (using R & Tableau)
This is an analysis case study as part of the capstone project of the Google Data Analytics Professional Certificate, where data fromm Cyclistic Bike-Share is presented, a fictional company. 
I am going to address a business task to understand and plan a smart strategy using the data analysis process that was taught in this certificate.

# Introduction
About the Company
Cyclistic is a bike-sharing service in Chicago, operating a fleet of 5,824 geotracked bicycles at 692 stations across the city. Bikes can be unlocked at one station and returned to any other within the network. Casual riders purchase single-ride or full-day passes, while annual memberships are available for frequent users.

Scenario
As a junior data analyst on Cyclistic’s marketing team, I’m tasked with analyzing how casual riders and annual members use Cyclistic bikes differently. The marketing director believes that increasing annual memberships is key to the company’s growth. My team will use these insights to develop a strategy to convert casual riders into annual members. To proceed, we need to present compelling data insights and professional visualizations for executive approval.

# Phase 1: Ask
> Understanding the problem.

#Business Task
Analyze the usage patterns of annual members versus casual riders to uncover insights into their distinct preferences. Use these findings to inform strategic marketing decisions for Cyclistic.

#Stakeholders
Lily Moreno: Director of Marketing and your manager. Responsible for developing promotional campaigns across email, social media, and other channels.

Cyclistic Marketing Analytics Team: A group of data analysts who collect, analyze, and report data to guide marketing strategies. You’ve been with the team for six months, focusing on learning Cyclistic’s mission and contributing as a junior data analyst.

Cyclistic Executive Team: The executive team, known for their attention to detail, will review and decide on the approval of the proposed marketing strategy.

#Phase 2: Prepare
> Identify and gather various data types, formats, and structures to ensure effective analysis. Additionally, uphold ethical standards in data analysis by addressing issues of bias and ensuring data credibility.

The data set is stored in an <a href="https://divvy-tripdata.s3.amazonaws.com/index.html" target="_blank">AWS server</a> 

# Data Structure
Each .csv file contains a table with 13 columns with varying data types as shown below. Each column stands for a field that describes how people use Cyclistic's bike-sharing service. Each row represents an observation with the details of every ride.

- ride_id = col_character(),
- rideable_type = col_character(),
- ride_id = col_character(),
- rideable_type = col_character(),
- started_at = col_datetime(format = ""),
- ended_at = col_datetime(format = ""),
- start_station_name = col_character(),
- start_station_id = col_character(),
- end_station_name = col_character(),
- end_station_id = col_character(),
- start_lat = col_double(),
- start_lng = col_double(),
- end_lat = col_double(),
- end_lng = col_double(),
- member_casual = col_character()

# Phase 3: Process
> Here I cleaned and transformed data while maintaining the data’s integrity. Documenting the data-cleaning process is essential to keep track of the changes made to the dataset.

I used Rstudio to combine and clean the dataset. Here are the steps that I did during this phase

1. Check for null and duplicates
2. Check consistency between ID and Names for Stations.
3. Additional columns and data transformation (change the data type, remove trailing or leading spaces, etc.)
4. Extract data for analysis





![Distribution of User Types in the Last 12 Months](https://github.com/user-attachments/assets/08c2c778-ef2d-4140-8ab4-8fe365e9f9d0)



