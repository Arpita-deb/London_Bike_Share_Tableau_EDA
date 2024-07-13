# London Public Bikes - What do you need to know before heading out?
## Exploratory data analysis of the London Public Bikes dataset for 2016 with Tableau

## Introduction:
Santander Cycles (or Boris Bikes) is a public bicycle hire scheme in London in the United Kingdom. I've used Tableau to provide an Exploratory Data Analysis (EDA) with visualizations of the bike usage in 2016 to find out if weather, season, holidays and other such variables have any effect on number of bike users. I've created a dashboard in Tableau Public to bring all the insights together.

## Dataset Used: 
[Historical data for bike sharing in London 'Powered by TFL Open Data'](https://www.kaggle.com/datasets/hmav) from Kaggle. I’ve filtered the data only for the year 2016, with 8699 rows and 9 columns for every hour of the year which contains data on 10,129,546 bikes.

## Data Dictionary:

| Column Name | Column Description|
| :---        | :---              |
| **Timestamp** | timestamp field for grouping the data |
| **Count Of Bikes** | the count of a new bike shares |
| **Temp** | real temperature in degree celsius |
| **Humidity** | humidity in percentage |
| **Wind Speed** | wind speed in km/h|
| **Weather Code** | category of the weather 1 = Clear; 2 = scattered clouds / few clouds; 3 = Broken clouds; 4 = Cloudy; 7 = Rain/ light Rain shower/ Light rain; 10 = rain with thunderstorm; 26 = snowfall |
| **Is holiday** | *Boolean field* 1 =holiday; 0= non holiday |
| **Is weekend** | *Boolean field* 1=weekend; 0=weekday |
| **Season** | category field meteorological seasons (spring, summer, fall and winter) |

## Potential Stakeholders:

* Bike-sharing companies: These are the entities that own, operate, and maintain the bike-sharing system, such as providing the bikes, stations, docks, apps, etc.

* The public: These are the potential and actual users of the bike-sharing system, who benefit from the convenience, affordability, and health benefits of bike-sharing.

* The media: These are the platforms that communicate and promote the bike-sharing system to the public, such as social media, news outlets, blogs, etc.

* The government: These are the authorities that regulate and support the bike-sharing system, such as providing policies, subsidies, infrastructure, etc.

## Overview of the Project:

The analysis is broken down into 2 parts:

**Part 1**: General Statistics for the London Bike Share dataset. In this part, I'll be looking for answers to these questions:

1. Which month showed the highest number of bike riders?
2. Which weekdays were busiest?
3. Is there any difference of bike riders in weekdays and weekends?
4. How many bike riders used these public bikes on holidays and non-holidays?
5. Which hour sees the highest number of bike users during weekdays as well as weekends?

**Part 2**: Here I'll investigate the effects of season, weather, temperature, humidity and wind speed over the bike usage.

Riding bike is an outdoor activity and naturally it is affected by weather and seasons equally. As a summer morning will draw more people out than a rainy or snowy day, it is important to take into account the effect of different weather conditions. In this part, I'll be looking for answers to these questions:

1. Which season is the most popular for bike riding?
2. How do temperature, humidity and wind speed effect number of bike users?
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

From the above visualizations, the following insights can be inferred:

* **July** showed the highest number of bike users in 2016.
* Most of the bikes were used on **Tuesday, Wednesday and Thursday**.
* There is a significant difference of bike riders in weekdays and weekends. People used these public bikes mostly to commute to workplaces which coincides with our observation of having the number of riders on weekdays being **3 times** of the number of riders on weekends.
* People tend to use these public bikes not only for going to and from workplaces, but for leisure as well on weekends, a significant number being on **Summer** when the weather is temperate and mild.
* **99% of the total users** i.e more than 9 million people used bikes on **non-holidays**, as the number of holidays being very small as compared to the number of non-holidays.
* Among the holidays, people mostly used the bikes on **summer bank holiday** in August.
* The busiest hour in weekdays for all the months is **8 AM** and **5 PM**, and for weekends between **1 PM - 5 PM**.

**Part 2**:

![seasons donut](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/9b51b207-9137-471f-81fa-a370f2151f75)

![Scatterplot](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/0f957dee-dc4f-44e6-9850-fe1cc0eb76fa)
The scatterplot shows the number of riders on clear days.

![scattered clouds (2)](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/340a1f12-f658-4043-afd1-606a210e6736)
This scatterplot shows the number of riders during days with scattered clouds. 

![cloudy (2)](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/a7d7147b-3c02-43f6-a80d-1cfd76e94ea8)
This scatterplot shows the number of riders during cloudy days.

![thunderstorm (2)](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/1edce8e9-f656-4d1a-a83e-c7625196ce25)
This scatterplot shows the number of riders during thunderstorms.

![snowing (2)](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/1900db97-81f6-4aae-857f-fb0d98eabab0)
This scatterplot shows the number of riders when it was snowing in and around London. 

![humidity histogram](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/26d9e68d-845d-4895-9d79-75193b7d9d48)

![temp graph](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/f2c1c56a-89ba-4297-a38e-cd6a6a897df9)

![temp histogram](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/2e0d633d-49d4-4f68-9e59-ce2d13e3861e)

![cummulative effects of weather](https://github.com/Arpita-deb/London_Bike_Share_Tableau_EDA/assets/139372731/f090a31e-ee7d-4e51-a2d1-a01e08343fad)

From the analysis of various weather conditions, the following insights can be drawn-
* **Summer** has the highest number of bike users.
* The effect of seasons and weather on number of bike users is that mild and temperate climate draws more people out, while extreme heat or cold or rain decreases the number of users.
* Humidity has a **negative correlation** with number of users, as can be seen from the scatterplots. Number of riders decreases as humidity of the air increases. Autumn (September - November) is usually London’s rainiest season and Winters (December - February) are characterised by cold and often rainy weather. During these months humidity was 80-90%, which indicates higher chances of precipitation.
* The temperature range was between **10-12 degree celsius** when most of the people rode out. Upto a certain point, number of bike users has a **positive correlation** with temperature, but high temperature (during Summer season) is also unfavourable for riding out.
* The wind speed has **no visible correlation** with number of bike riders, though heavy rainfall and snowstorms are often accompanied by high wind speed.

## Conclusion: 

From the above analysis, the following conclusions can be drawn:

1. Weather and seasons have positive if not strong influence over the number of bike riders in London. Temperate weather conditions as can be seen in summer and fall, draws more riders out than a rainy or snowy day.
   
2. Number of riders seems to increase as temperature increases, annually as well as daily. July and August had the highest number of riders, while these were also the warmest months in 2016.
   
3. Number of riders gradually decreases as humidity of the air increases. It coincides well with people heading out on clearer days than on cloudy or rainy days.
   
4. Most people tend to use bikes during the daytime rush-hours i.e., at 8 AM and 5 PM during weekdays, as they commute to and from workplaces. On weekends most people use bikes in early afternoon (1PM — 5PM).

## Some Recommendations:

* Bike-sharing companies: They should improve their user-interface design, to make it more user-friendly, intuitive, and informative. They should also monitor the feedback and ratings of their products, and adjust their pricing and quality accordingly, to maintain customer satisfaction and loyalty.

* The public: They should use the bike-sharing system responsibly and civilly, by following the relevant rules and norms, such as parking in designated areas, returning the bikes on time, reporting any damages, etc. They should also spread the word and encourage others to use the bike-sharing system, by sharing their positive experiences and benefits on social media, blogs, etc.

* The media: They should raise the awareness and interest of the public towards the bike-sharing system, by highlighting its advantages and impacts on sustainability, health, and mobility. They should also report on the challenges and issues of the bike-sharing system, and provide constructive suggestions and solutions.

* The government: They should provide financial and policy support to the bike-sharing system, such as offering grants, subsidies, tax incentives, etc. They should also provide adequate and safe infrastructure for the bike-sharing system, such as bike lanes, parking zones, signage, etc.

## Dashboard:
![Santander cycles ](https://github.com/user-attachments/assets/29025e2d-ca02-4156-a685-591a2e348f33)
For this project I've created an exploratory dashboard providing an overview of the analysis, highlighting important insights. 

In order to build the tableau visualizations and the dashboards, I've taken the following steps:

1. Used floating containers to contain the individual data visualizations.

2. Used titles for each of the visualizations and the dashboard.

3. Used filter and annotations to highlight important data points.

4. Used consistent color scheme that enhances the data.

5. Cleared the chart junks such as titles of individual data viz, axis and axis labels, color legends etc that doesn't contribute to the data design.

6. Visually grouped the data by using layout containers and colored background

7. Added filter and highlight actions in the dashboard to provide user interactivities.

8. Added an info button that provides additional informations on the dataset and how to read the dashboard.

9. Created 3 device specific layouts.

Check out the dashboard here [London Bike Share - What do you need to know before heading out?](https://public.tableau.com/views/LondonBikeShare_16917538190290/Dashboard4?:language=en-US&:display_count=n&:origin=viz_share_link)

## References:

* [Santander Cycles](https://en.wikipedia.org/wiki/Santander_Cycles)
* [Climate of London](https://en.wikipedia.org/wiki/Climate_of_London)
* [State of the UK Climate 2016 - Met Office](https://www.metoffice.gov.uk/about-us/press-office/news/weather-and-climate/2017/state-of-the-uk-climate-report-2016)
* [Holiday Lists of London - 2016](https://www.timeanddate.com/holidays/uk/2016)

