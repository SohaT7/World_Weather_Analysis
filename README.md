# World Weather Analysis
## Table of Contents
- [Overview of the Analysis](#overview-of-the-analysis)
    - [Purpose](#purpose)
    - [About the Dataset](#about-the-dataset)
    - [Tools Used](#tools-used)
    - [Description](#description)
- [Results](#results)
    - [Retrieving Data](#Retrieving-Data)
    - [Creating a Map based on Weather Preferences](#Creating-a-Map-based-on-Weather-Preferences)
    - [Creating a Travel Itinerary Map](#Creating-a-Travel-Itinerary-Map)
- [Summary](#summary)
- [Contact Information](#contact-information)

## Overview of the Analysis
### Purpose:
The purpose of this project is to create a travel itinerary map based on the customer's weather preferences. 

### About the Dataset:
The weather data is collected by making an API 'get' request at the [Open Weather Map website](https://openweathermap.org/api). The data is then retrieved in a JSON (JavaScript Object Notation) format.

### Tools Used:
 - Python (Pandas, Matplotlib, and SciPy libraries)
 - APIs (OpenWeatherMap, Google Directions)

### Description:
This project enables the users to filter the weather data for weather that they prefer, and then view the potential travel destinations and nearby hotels that fall within that preferred weather criteria. Moreover, the user is then able to choose four cities out of those potential destinations and draw up a travel itinerary encompassing those cities. 

## Results
### Retrieving Data:
The [Weather_Database folder](https://github.com/SohaT7/World_Weather_Analysis/tree/main/Weather_Database) contains weather data on multiple cities around the globe, read into a DataFrame.

The weather data is retrieved by generating a set of 2,000 random latitudes and longitudes, retrieving the nearest city, and then performing an API call at OpenWeatherMap. The current weather description for each city is also retrieved and added to the current weather data, in order to create a new DataFrame that contains the updated weather data.

### Creating a Map based on Weather Preferences:
The [Vacation_Search folder](https://github.com/SohaT7/World_Weather_Analysis/tree/main/Vacation_Search) contains the code to create a map that lays out potential travel destinations, as per the customer's weather preferences, and nearby hotels.

A customer travel destinations map is created by first taking the customer weather preferences as input, and then using that input to determine potential travel destiantions and hotels found nearby. The destiantions are then shown on a marker layer map as pop-up markers that contain basic information (hotel name, city, country, and current weather).

![Customer Travel Destinations Map](https://github.com/SohaT7/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

### Creating a Travel Itinerary Map:
The [Vacation_Itinerary folder](https://github.com/SohaT7/World_Weather_Analysis/tree/main/Vacation_Itinerary) contains the code to create a map that shows the travel itinerary between the four cities that the customer choses as possible travel destinations.

A travel itinerary map is created by using Google Directions API, and it shows the travel route between the four cities that the customer chose as their travel destiantions. The map also contains pop-up markers for each of the four cities. 

![Travel Itinerary Map](https://github.com/SohaT7/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

![Travel Itinerary Map with pop-up markers](https://github.com/SohaT7/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)

## Summary
The project asks the customer for their weather preferences, and uses that as input to create a map which shows all possible travel destinations that meet the criteria. It then allows the customer to select four cities out of the many, and lays out a travel route between those four cities on the map.

## Contact Information
Email: st.sohatariq@gmail.com
