# World_Weather_Analysis

# Overview
The world weather project is to apply analysis, visualizations, retrieve weather information from Openweather websites by using API, and using g_key retrieve information from google map platform. 

The expected deliverables are:

  1. Retrieve 2000 cities weather data
  2. Create a Customer Travel Destination Map
  3. Create a Travel Itinerary Map

# Resources

Data: Open Weather Website

Platform: Google Map Platform

Software: Python 3.7.6, Jupyter notebook 6.4.8 

# Results

## Retrieve weather data

First using numpy to randomly generate 2000 pairs of latitude and langitude, and then using citipy to find nearest city of those latitude and langitude. It turns out we have 743 cities founded.

Then the weather data was retrieved from open weather website by using those 743 cities latitude and langitude, and convert the weather data into a DataFrame and save it to a csv file.

![weather dataframe](https://github.com/ivorfanning/World_Weather_Analysis/blob/main/weather_data/challenge_weather_dataframe.png)

## Creat a travel destination map

By using a cutomer tempeture preferences and the csv file we generated above, we filtered the data and obtained a new dataframe which meets the customer requirements. Then we generate a google map of travel destinations with all the markers and pop-up weather information

![destinations map](https://github.com/ivorfanning/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

## Customize a trip 

The customer choose to travel in US, and I use google direction API to customize a travel route for the customer. It shows the travel start, end and 3 stops in the middle. All the destinations are markered with a pop-up weather information.

![route map](https://github.com/ivorfanning/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

![pop-up markers map](https://github.com/ivorfanning/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)
