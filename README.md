# Cyclistic Bike-Share Analysis - Capstone Project. Google Data Analytics Professional Certificate (using R & Tableau)
This case study forms a key component of the capstone project for the Google Data Analytics Professional Certificate. It involves analyzing data from Cyclistic Bike-Share, a fictional company. My goal is to tackle a business challenge by leveraging the data analysis techniques and methodologies taught throughout the certificate program. This analysis will guide the development of a strategic plan based on the insights gained from the data.

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
Each .csv file includes a table with 13 columns of different data types. Each column represents a field describing the usage of Cyclistic's bike-sharing service, while each row provides details of an individual ride.

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
> Here I also created new metrics/new columns.

I used Rstudio to combine and clean the dataset. Here are the steps that I did during this phase

1. Check for null and duplicates
2. Check consistency between ID and Names for Stations.
3. Additional columns and data transformation (change the data type, remove trailing or leading spaces, etc.)
4. Extract data for analysis

For all the detailed process, you can review it in the code. here it is. <a href="[https://divvy-tripdata.s3.amazonaws.com/index.html](https://github.com/RogelioRFmx/google_data_analytics_project/blob/main/RogelioReyna-CapstoneProject-ProcessPhase.Rmd)" target="_blank">Process code</a>

This part was very interesting and challenging for me since I tried to fix the inconsistencies for the ID Stations and Stations names.

# Phase 4: Analyze
> During this phase, I employ tools capable of formatting, transforming, filtering, and sorting our data. This enables us to recognize patterns, make predictions, draw conclusions, and provide recommendations, facilitating the formulation of data-driven decisions.
> In this phase I also created new columns to have specific metrics that helped me to visualize and analyze better the data.

I used R to look at a huge data I cleaned and prepared.


Findings
* 64.89% of the total Cyclistic users are annual members while 35.11% are casual riders.
* The most preferred  rideable type for both users is classic bikes. But, for casual users the difference between classic and electric is not huge in number. And Only casual riders use docked bikes.
* Generally, casual riders have the longest average ride duration (almost 27 minutes) compared with annual members (13 minutes).
* Docked bikes have the longest average ride duration (56 minutes).
* There is a clear difference in the usage of bikes during the week for casual and members, during working days the members are who use it more, and during weekends the casual users are who use the service more.
* There are more trips during summer and less during winter.

# Phase 5: Share
Share the findings using visualizations.

> Data Visualization
> I used Tableau public in making the visualization.


# Distribution of User Types in the Last 12 Months
64.89% of the total Cyclistic users are annual members while 35.11% are casual riders.
![Distribution of User Types in the Last 12 Months](https://github.com/user-attachments/assets/7de92ba9-6ef3-4d17-b385-6736af3e8ac3)

# Rideable Preference and Average Ride Duration per Type of User
The most preferred  rideable type for both users is classic bikes. But, for casual users the difference between classic and electric is not huge in number. And Only casual riders use docked bikes.
Generally, casual riders have the longest average ride duration (almost 27 minutes) compared with annual members (13 minutes).
Docked bikes have the longest average ride duration (56 minutes).

![Rideable Preference and Average Ride Duration per Type of User](https://github.com/user-attachments/assets/f569a328-841d-4e1b-b211-1492822d6f9e)

# Count of Rideable Type and Ride Length - By Weekdays and User Type
There is a clear difference in the usage of bikes during the week for casual and members, during working days the members are who use it more, and during weekends the casual users are who use the service more.

![Count of Rideable Type and Ride Length - By Weekdays and User Type](https://github.com/user-attachments/assets/4f8710b9-6744-4e77-b1f6-90c8184356c4)


# Seasonal - Monthly Trip Trends
There are more trips during summer and less during winter.

![Seasonal - Monthly Trip Trends](https://github.com/user-attachments/assets/5f16aad5-2a5e-4430-b4da-acda74c3eff0)

# 6 Most Popular Start Stations
The most popular start stations are close to the coast and are dominated by casual members.
![6 Most Popular Start Stations](https://github.com/user-attachments/assets/35422134-edd6-44e6-945d-e5f9a89fc438)

# 6 Most Popular End Stations
The most popular end stations are close to the coast and are dominated by casual members.
![6 Most Popular End Stations](https://github.com/user-attachments/assets/f87bfe7d-30c7-43be-9b67-32d062349f42)


# Phase 6: Act
> In this final phase, the insights gained are utilized to make informed decisions that address the issues identified during the initial analysis phase. This decision-making process may involve a range of actions, including refining or enhancing existing products and services based on the new understanding. Additionally, it could lead to the development and introduction of entirely new products or services designed to better meet the needs and expectations revealed through the analysis. By leveraging these insights, we aim to implement strategic changes that effectively resolve the problems and drive improvements in our offerings.

# Recommendations

* **Highlight Benefits for Long-Duration Riders**: Since casual riders have longer average ride durations (27 minutes compared to 13 minutes for annual members), develop targeted marketing campaigns that emphasize **the value and cost-efficiency of annual memberships for frequent, long-duration rides**.
* **Promote Seasonal Discounts** Offer special promotions or discounts on annual memberships during the summer months to attract casual riders who are more active during this time.
* **Improve Docked Bike Usage**: Since docked bikes have the longest average ride duration (56 minutes), explore ways to make docked bikes more appealing. This could include adding more docked bike stations in high-traffic areas or offering incentives for **using docked bikes**, such as a **discount on an annual membership**.
* Since casual riders use bikes more on weekends, while annual members ride more on weekdays. Create **weekend-centric promotions** or events to **encourage casual riders** to consider the **benefits of an annual membership** for more consistent usage throughout the week.
* **Winter Engagement Programs**: This could include **winter promotions for annual memberships** or special events that encourage bike usage even in colder months.
* **Summer Member Drives**: Capitalize on **higher bike usage in summer** to run a **membership drive with incentives** such as **limited-time summer discounts** or **perks for new annual members**.










