## Author: Ruben Gallardo

## Description
The U.S. is known for it's car-dependent culture, but unfortunately is has taken a turn for the worst. 
According to recently published [NPR article](https://www.npr.org/2023/06/26/1184034017/us-pedestrian-deaths-high-traffic-car), pedestrian deaths from vehicle are at a 40-year high. This is likely attributed to the increase in vehicle size, which has made collisions with vehicles even more deadly ([source](https://www.economist.com/interactive/united-states/2024/08/31/americans-love-affair-with-big-cars-is-killing-them)). In addition, the disinvestment in public transit services continues accross the country, which doesn't help combat the dependency on cars. For instance, even in big cities like Chicago, public transit services struggle to provide the same level of service before the pandemic. 

The goal of this project is to analyze the impact of the "big car" trend and the disinvestment in public transit in the city of Chicago through a series of data visuals. The project will consist of visuals that will hopefully capture how these trends have materialized throughout Chicago. For example, the data visuals could help us answer the question of whether traffic crashes or congestion has increased due to the reliance issues of the CTA or if the deadliness of car crashes has increased in the past decade, which is the same decade we have seen the size of cars rapidly increase. 

## Data Sources 
- [Traffic Crashes: Crashes](https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if/about_data) - Crash data shows information about each traffic crash on city streets within the City of Chicago limits and under the jurisdiction of Chicago Police Department (CPD).
  - Rows: 879,740 Columns: 48
  - How I will use it: I want to visualize these crashes onto a map of Chicago similar to how this person did in this [tweet](https://x.com/ronythebikeczar/status/1841159287889969387), however, I want to include a time series component to make it more interesting and useful. 
- [Traffic Crashes: People](https://data.cityofchicago.org/Transportation/Traffic-Crashes-People/u6pd-qa9d/about_data) - This data contains information about people involved in a crash and if any injuries were sustained.
  - Rows: 1.93 million Columns: 29
  - How I will use it: I want to visualize the amount of people involved in crashes and the number of injuries sustained. This could be as simple as a bar graph, but it could also be interesting to include a geography component to see if there's any areas in the cities that stand out for being the "deadliest" when it comes to car crashes. 
- [Historical Congestion Estimates by Segment - 2011-2018](https://data.cityofchicago.org/Transportation/Chicago-Traffic-Tracker-Historical-Congestion-Esti/77hq-huss/about_data) - This dataset contains the historical estimated congestion for 1270 traffic segments, in selected time periods from August 2011 to May 2018.
  - Rows: 19.5 million Columns: 5
  - I would like to visualize this data onto a map to identify which areas have seen the largest increases in congestion. I want to use this pre-pandemic dataset for comparision purposes. For example, it could help identify areas that have seen an increase or decrease in congestion after the pandemic. 
- [Historical Congestion Estimates by Segment - 2018-Current](https://data.cityofchicago.org/Transportation/Chicago-Traffic-Tracker-Historical-Congestion-Esti/sxs8-h27x/about_data) - This dataset contains the historical estimated congestion for over 1,000 traffic segments, starting in approximately March 2018.
  - Rows: 292 million Columns: 22
  - I would like to visualize this data onto a map to identify which areas have seen the largest increases in congestion. This dataset is huge, so I will need to figure out a way to decrease the size of the dataset if that becomes an issue. 
- [CTA - Ridership - Daily Boarding Totals](https://data.cityofchicago.org/Transportation/CTA-Ridership-Daily-Boarding-Totals/6iiy-9s97/about_data) - This dataset shows systemwide boardings for both bus and rail services provided by CTA, dating back to 2001.
  - Rows: 8,675 Columns: 5
  - I would like to create some visuals of CTA ridership so it can help complete the story that I'm trying to tell. If there's a geography component to CTA data, I would also be interested to see if I can discover physical areas in the city where there's a correlations between increases in congestion or traffic crashes and a decrease in CTA ridership in nearby stations. 