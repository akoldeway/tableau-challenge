# 2018 NY Citi Bike Analysis


## Project Overview
The goal of this project was to review and analyze Citi Bike trip data published by New York city.  In addition to retrieving and scrubbing the data, visualizations were created in Tableau to illustrate the findings and made into dashboards and a story.  

The Tableau story (and corresponding dashboards and individual visualizations) can be found here: https://public.tableau.com/views/CitibikeTripAnalysis_15761786485620/Story-CitibikeNYAnalysis


## Data Retrieval and Cleaning Performed
All of the 2018 Citi Bike trip data published by New York city was downloaded and each monthly file was combined into a single file.  That single file was then loaded into pandas to perform the following cleaning activities:
* remove all trips that started and ended at the same station and were less than 2 minutes in duration
    * these trips may indicate issues with the bike when removed from dock
* remove all trips more than 2 hours in duration
    * these trips may indicate a stolen bike, issues docking a bike, or a data anomaly

## Data Analysis Performed

### Station Usage
#### Station Usage Map
I plotted all unique starting stations for each trip in the data analysis on a map.  Size and color of marker are relative to the total number of trips taken (blue largest number to red as the smallest number).  The map shows most trips began within the city center with stations further way from the city center showing less trips beginning.  Given the business and entertainment offered to residents and tourists, those areas most populated would show the most trips taken.  

#### Top 10 Start and End Stations
I sorted total trips to find the top 10 most popular start and end stations.  Again, we find the most popular stations are in the city center.  We also find common stations across both lists.  New York offers a variety of transportation options and it make sense that Citi Bikes would be used most often for short trips. 


### Top Trips
An evaluation of all trips was performed to find the top 20 trips for 2018.  A sum of trips between each station combination was performed to find the most popular trips.  We find a lot of trips near Central Park with the most popular trip beginning and ending at the same station near Central Park.  This information can be used to help ensure bikes are readily available in these locations.

### Top Trip Times
#### Trips by Month
Plotting the total number of trips by month we find the most rides are taken in late spring to early fall.  This aligns with optimal summer-like weather conditions providing the most comfortable times to use Citi Bikes.

#### Trips by Hour
Reviewing all trips taken by hour show a surge in bikes used during the morning and evening commute times.

#### Popular Trip Times
A heatmap was created showing the relationship between month and hour of trips taken.  This heatmap provides a clearer view of peak usage by month and hour.

## Tableau
In addition to the visualizations outlined above, I created dashboards in Tableau to combine the viz's in meaniingful way.  A tableau story was used to pull all the information together.

