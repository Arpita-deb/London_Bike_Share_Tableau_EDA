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

![Number of bikes used in each month)](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/895fae6d-9d72-4798-89aa-c570bf7c63ac)

![number of bikes by weekday](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/23ddcb12-3a0d-4ecb-bd5e-fb1e52a53a0a)

![Weekend/weekday](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/6d15bb87-32b2-4d44-8fc8-a439c0d0df7d)

![holiday/nonholiday donut](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/f768e3ca-6d07-49d4-b061-b4a1cdc8f945)

![list of holidays](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/11d595df-1dac-4ef8-80e3-9adf847e4cba)

![hour of the day](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/3bac74e3-9a4b-46ed-80d0-8f1ca39a2481)

![hours for weekends/weekdays)](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/b0d073f7-143a-47c7-bd36-6e5a9a7fd29e)

![weekends by seasons](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/b9f29257-9d9f-4a23-8591-d0bd110b08b3)

**Part 2**:

![seasons donut](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/9b51b207-9137-471f-81fa-a370f2151f75)

![Scatterplot](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/0f957dee-dc4f-44e6-9850-fe1cc0eb76fa)

![scattered clouds (2)](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/340a1f12-f658-4043-afd1-606a210e6736)

![cloudy (2)](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/a7d7147b-3c02-43f6-a80d-1cfd76e94ea8)

![thunderstorm (2)](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/1edce8e9-f656-4d1a-a83e-c7625196ce25)

![snowing (2)](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/1900db97-81f6-4aae-857f-fb0d98eabab0)

![humidity histogram](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/26d9e68d-845d-4895-9d79-75193b7d9d48)

![temp graph](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/f2c1c56a-89ba-4297-a38e-cd6a6a897df9)

![temp histogram](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/2e0d633d-49d4-4f68-9e59-ce2d13e3861e)

![cummulative effects of weather](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/f090a31e-ee7d-4e51-a2d1-a01e08343fad)

## Conclusion: 

From the above analysis, the following conclusions can be drawn:

1. Weather and seasons have positive if not strong influence over the number of bike riders in London. Temperate weather conditions as can be seen in summer and fall, draws more riders out than a rainy or snowy day.
   
2. Number of riders seems to increase as temperature increases, annually as well as daily. July and August had the highest number of riders, while these were also the warmest months in 2016.
   
3. Number of riders gradually decreases as humidity of the air increases. It coincides well with people heading out on clearer days than on cloudy or rainy days.
   
4. Most people tend to use bikes during the daytime rush-hours i.e., at 8 AM and 5 PM during weekdays, as they commute to and from workplaces. On weekends most people use bikes in early afternoon (1PM — 5PM).


## Dashboard:


![London Bike Share Dashboard](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/6d40fa25-c5f6-40e6-8802-a8de7fa26681)

check out the dashboard here [London Bike Share - What do you need to know before heading out?](https://public.tableau.com/views/LondonBikeShare_16917538190290/Dashboard4?:language=en-US&:display_count=n&:origin=viz_share_link)

## Citations:

* [Santander Cycles](https://en.wikipedia.org/wiki/Santander_Cycles)
* [Climate of London](https://en.wikipedia.org/wiki/Climate_of_London)
* [State of the UK Climate 2016 - Met Office](https://www.metoffice.gov.uk/about-us/press-office/news/weather-and-climate/2017/state-of-the-uk-climate-report-2016)
* [Holiday Lists of London - 2016](https://www.timeanddate.com/holidays/uk/2016)

