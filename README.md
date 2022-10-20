# Surfs_up_analysis
Weather analysis for surfs n shake using SQLite and SQLAlchemy. Click here on the link to see the analysis for June and December : [Surfup analysis for June and December](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/SurfsUp_Challenge.ipynb)

## Overview of Surfs Up Analysis

The purpose of this analysis is to review a dataset for weather conditions that have been stored in a [SQLite database](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/hawaii.sqlite) to provide information that will convince an investor that opening up a **Surf n' Shake** shop in Oahu, Hawaii is a good business idea.
 
* The idea is that the shop will sell surfboards and ice cream throughout the year, but the investor is hesitant because he invested in a similar business that failed due to the weather conditions. 
* To get this investor on board, we need to provide statistical analysis specifically on the weather conditions in Oahu that will convince him that this will be a successful business venture.
* To convince an investor, we used  [Jupiter notebook](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/climate_analysis.ipynb) for weather analysis for different criteria.
* Below is a sample of the dependencies and functions that were used to access the content in the *SQLite* database:

![SQLAlchemy dependencies](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/Resources/dependencies.png)

* We also used *Visual Studio Code* to create Python applications to share the results via a webpage by creating *Flask* routes and using Terminal to run the Flask app.


## Results

* When we fetched the data, we first looked at the precipitation for a one-year timeframe. We reviewed the activity from August 23, 2016 - August 23, 2017. The average was 18% based on 2,021 observations. The summary reports that Oahu was sunny for most of the year and experienced low rainfall. The below image shows a code for last year's precipitation.

![exploretry climate analysis](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/Resources/EDA_for_precipitation_plot.png)

* After running the program we get a graph plot of last year's rainfall. Its image is shown below:

![last_year_precipitation_observation](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/Resources/last_year_precipitation_observation.png)

* We also looked at the number of weather stations that actively collect precipitation data and focused on the station that reported the most observations. In total, (9) stations with `USC00519281` show the highest number of observation counts at 2,772 entries. We used data from these stations to review temperatures for the period. The results show that the average temperature throughout the year was **72°F** with a **54°F** and a high of **85°F**.

![last_year_temp_observation](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/Resources/last_year_temp_observation.png)

* We expanded our results to look at all of the observations which were recorded in the month of **June** and **December** regardless of year. 

The program and dataframe for June are shown below which include dates and temperature:

![june_dataframe_code](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/Resources/june_dataframe_code.png)

![june_dataframe](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/Resources/june_dataframe.png)

The program and dataframe for the month of December are shown below which include dates and temperature:

![dec_dataframe_code](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/Resources/dec_dataframe_code.png)

![dec_dataframe](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/Resources/dec_dataframe.png)

* Here comparison between the month of June and December.

![june_dec_summary](https://github.com/miralchangela/Surf-s_up_analysis/blob/main/Resources/june_dec_summary.png)

The result showed that:

* The average temperature is in the 70's.
* Both June and December showed similar min/max and average temperatures.
* The assumption is that the temperature does not have drastic fluctuations throughout the year.

## Summary

* In summary, the temperature in Oahu is relatively the same throughout the year and the chances of continuous rainfall are low. 

* there are two additional queries to perform to gather more weather data for June and December:

1)  When we rewrite the queries to add precipitation to the results for June and        December, the average precipitation in those months showed:
        * June at 14%
        * December at 22%

2) we can also add average hours of sunshine per day.





