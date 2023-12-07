** This repository contains the portfolio project that I did to for the Google Data Analytics Certificate program ** 
** Below is an overview of the project and my findings ** 
# Cyclistic Bike_share
## Introduction
Cyclistic is a bike-sharing company launched in 2016. The company is based in Chicago and it is working on appealing to more consumers. So far, the approach that has seen the company grow is having flexible payment plans where customers can purchase annual memberships or they can buy single-ride or full-day passes. Past data shows that annual members are more profitable than casual riders. Therefore, the company wants to maximize annual members for more returns. 
## Business problem
Moreno, the director of marketing wants a strategy that will focus on converting the casual members to annual members instead of one that focuses on all customers. The goal for the analysis is therefore to craft strategies for converting casual to annual members. 

As a junior data analyst, Moreno directed me to find how annual members and casual riders use Cyclistic bikes differently. The insights from this analysis will help Cyclistic devise a marketing strategy that will help the company convert more casual riders to annual members. 
## Data sources used
The data used for this project are made available by [Motivate International Inc](https://divvy-tripdata.s3.amazonaws.com/index.html). There are many datasets in the site but I opted for six datasets; three from October to December 2020 and three from January to March 2021. After merging the 6 datasets, the outcome is 13 variables and 1,154,894 rows. 

The variables are:
* rideable_id - This is a unique identifier for the rides 
* rideable_type - This represents the type of bikes that the Cyclistic offers
* started_at - This represents the time that a customer starts riding the bikes
* ended_at - This represents the time the customer ended a ride
* start_station_name - This represents the station that the customer started riding the bikes
* start_station_id - This is the unique identifiers of the stations
* end_station_name - This represents the station where the customer ended the rides
* end station_id
* start_lat - This is the latitude of the station where the customer started riding the bike
* start_lng - This is the longitude of the station where the customer started riding the bike
* end_lat - This is the latitude of the station where the customer ended the bike ride
* end_lng - This is the longitude of the station where the customer ended riding the bike
* member_casual - This represents the customer 

## Data cleaning & manipulations
In this section, I created a pipeline for selecting only 6 columns that are relevant to the analysis. The columns are rideable_type, start_station_name, end_station_name, member_casual, started_at, ended_at. I checked for missing values in this new dataset and found none. Therefore, I proceeded to create new columns from the started_at and ended_at. The columns I created are: 
* cycling_time_minutes for the time that the riders spent cycling
* start_hour for the time that the riders started cycling
* Month_year for the specific month and year that the riders cycled. 
## Summary of the analysis
For the 12 months under analysis:

1. Annual members used Cyclistic bikes more than casuals
2. Docked bikes were the most popular bikes among all riders
3. Annual members spent a little bit more time riding unlike casual members. 
4. For Annual members, their peak time is 1700 hours. This starts to build up at 1500 hours before peaking at 1700 hours and then dropping. This is the same case for casual members but their numbers are lower compared to annual members. 
5. On Monthly trends, higher number of rides annual members was seen in the months of July, August, September and October of 2020. For casual members, their numbers was high in th months of July, August and September 2020. 
6. The top 3 popular start stations for casual members are Streeter Dr & Grand Ave, Lake Shore Dr & Monroe St and Millennium park. For annual members, their top 3 start stations were Clark St & Elm St, Broadway & Barry Ave and Dearborn St & Erie St. 
7. The top 3 popular end stations for casual members were Streeter Dr & Grand Ave, Millennium park and Lake Shore Dr & Monroe St. The top 3 end stations for annual members are Clark St & Elm St, St. Clair & Erie St, and Broadway & Barry Ave. 
## Marketing recommendations

* Run targeted promotions including exclusive discounts for casual riders willing to be annual members and this should be done at the peak hours starting from 1500 hours to 1700 hours
* Share with the casual riders the benefit of being annual members like convenience and cost saving
* Advertise annual membership and its benefits in the popular routes that the casual members frequent: Streeter Dr & Grand Ave, Lake Shore Dr & Monroe St and Millennium park
* Introduce promotional trials where casual members can try annual membership at a reduced rate for a specific period. 

