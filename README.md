# Exploratory data analysis of the London Public Bikes dataset for 2016 with Tableau
## Introduction:
Santander Cycles (or Boris Bikes) is a public bicycle hire scheme in London in the United Kingdom. The scheme commencing on 30 July 2010 with 5,000 bicycles and 315 docking stations distributed across the City of London, now spreads across 40 square miles of London with over 12,000 bikes and 800 stations. I've used Tableau to provide an Exploratory Data Analysis (EDA) with visualizations of bike usage in the year 2016 to find out if weather, season, holidays and other such variables have any effect on number of bike users and created a final dashboard to bring all the insights together in Tableau Public.

## Dataset Used: 
Historical data for bike sharing in London [Powered by TFL Open Data](https://www.kaggle.com/datasets/hmav) from Kaggle. I’ve filtered the data only for year 2016 with 8699 rows and 9 columns for every hour of the year which contains data on 10,129,546 bikes.

## Data Dictionary:

* Timestamp — timestamp field for grouping the data

* Count Of Bikes — the count of a new bike shares

* Temp — real temperature in C

* Humidity — humidity in percentage

* Wind Speed — wind speed in km/h

* Weather Code — category of the weather

    1 = Clear
  
    2 = scattered clouds / few clouds
  
    3 = Broken clouds
  
    4 = Cloudy
  
    7 = Rain/ light Rain shower/ Light rain
  
    10 = rain with thunderstorm
  
    26 = snowfall

* Is holiday — *Boolean field* — 1 =holiday; 0= non holiday

* Is weekend — *Boolean field* — 1=weekend; 0=weekday

* Season — category field meteorological seasons (spring, summer, fall and winter)

## Overview of the Project:

The analysis is broken down into 2 parts:

**Part 1**: General Statistics for the London Bike Share dataset. In this part, I'll be looking for answers to these questions:

1. Which month showed the highest number of bike riders?
2. Which weekdays were most busiest?
3. Is there any difference of bike riders in weekdays and weekends?
4. How many bike riders used these public bikes on holidays and non-holidays?
5. What percentage of riders used the bikes on weekdays/weekends and holidays/non-holidays?
6. Which hour sees the highest number of bike users during weekdays as well as weekends?

**Part 2**: Here I'll investigate the effects of season, weather, temperature, humidity and wind speed over the bike usage.

Riding bike is an outdoor activity and naturally it is affected by weather and seasons equally. As a summer morning will draw more people out than a rainy or snowy day, it is important to take into account the effect of seasons. In this part, I'll be looking for answers to these questions:

1. Which season is the most popular for bike riding?
2. How does temperature, humidity and wind speed effect number of bike users?
3. Which weather conditions were most suitable for bike riding?

## Analysis:

**Part 1**:




Dashboard:

![London Bike Share Dashboard](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/6d40fa25-c5f6-40e6-8802-a8de7fa26681)

check out the dashboard here [London Bike Share - What do you need to know before heading out?](https://public.tableau.com/views/LondonBikeShare_16917538190290/Dashboard4?:language=en-US&:display_count=n&:origin=viz_share_link)

## Citations:

* [Santander Cycles](https://en.wikipedia.org/wiki/Santander_Cycles)
* [Climate of London](https://en.wikipedia.org/wiki/Climate_of_London)
* [State of the UK Climate 2016 - Met Office](https://www.metoffice.gov.uk/about-us/press-office/news/weather-and-climate/2017/state-of-the-uk-climate-report-2016)
* [Holiday Lists of London - 2016](https://www.timeanddate.com/holidays/uk/2016)

