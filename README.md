# Plan My Trip APIs
## Overview
The purpose of this project is to collect and analyze weather data across cities worldwide, so that PlanMyTrip could use the data to recommend ideal hotels based on clients' weather preferences.
  - Weather Scattor Plots and Heatmap
    - Use the NumPy module to generate a list of random latitude and longitude to setup locations.
    - Use the citipy module to list the nearest city to these locations.
    - Use the OpenWeatherMap API to request the current weather data from each city to retrieve its JSON file.
    - Collect weather information from JSON file and create a city-weather DataFrame. Including city, country, and date, latitude and longitude, maximum temperature, humidity, cloudiness, wind speed, description.
    - Create scatter plots of the weather data vs latitude
    - Determine the correlations for the weather data vs latitude with linear regression.
    - Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. 
 
 - Vacation Plan
   - Filter the city-weather DataFrame based on user inputs for a minimum and maximum temperature. Create a new heatmap for the new DataFrame, and clean the data.
   - Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby Hotel, add to DataFrame.
   - Add pop-up markers to the heatmap that display information about the city, current maximum temperature, and a hotel in the city.

 - Travel Route for Potential Travel Destination
    - From the list of potential travel destinations, four cities were chosen to create a travel itinerary.
    - Using the Google Maps Directions API, create a travel route between the four cities as well as a marker layer map.

## Results
  - City_Weather and Hotel DataFrame
    ![City_Weather DataFrame](https://user-images.githubusercontent.com/105877888/177010199-a3ba1b8b-9136-443a-a72e-332b65f02bab.PNG)
    
    ![City_Weather DataFrame](https://user-images.githubusercontent.com/105877888/177010485-5ec267ce-3c81-463b-adf8-b70b79219228.PNG)
    
    ![City_Weather_Hotel DataFrame](https://user-images.githubusercontent.com/105877888/177010658-3f2eb8b0-bd23-41c3-80c8-98dbfc17b863.PNG)

  -  City_Weather Scatter Plots Example  
    ![City_Weather Scatter Plots](https://user-images.githubusercontent.com/105877888/177010275-aab6005b-8dc3-474e-86e4-c938f0295931.PNG)
    
  - City_Weather Correlations Example
    ![City_Weather Correlations](https://user-images.githubusercontent.com/105877888/177010311-5994ea69-6e12-4305-8ecd-4e0900c67f6c.PNG)
    
  - City_Weather Heatmap for vacation plan
    ![Latitude_Max Temp Heatmap](https://user-images.githubusercontent.com/105877888/177011151-00291777-f542-40a5-a431-fc29de2eb253.PNG)

    ![Latitude_Max Temp PopupMarker Heatmap](https://user-images.githubusercontent.com/105877888/177011134-006cdcfd-2abc-4e37-8561-2eafd7884ccd.PNG)

    ![WeatherPy_vacation_map](https://user-images.githubusercontent.com/105877888/177010589-0ebc22aa-22fd-4c6c-be76-7951d521468b.PNG)
    
  - City Travel Map
    ![WeatherPy_travel_map_enlarged](https://user-images.githubusercontent.com/105877888/177010724-eb0fd861-ed7f-4daa-a54b-277d12784585.png)

    ![WeatherPy_travel_map_markers](https://user-images.githubusercontent.com/105877888/177010690-8975bffe-db92-43ef-858a-2ca1ad37c42a.png)
## Summary
  - Using realtime layered heatmap, users can easily plan their their trip according to the weather across the world. 
  - Taking input of client's weather preferences, PlanMyTrip may also give recommendations of ideal hotels in target city.
  - For designated cities, PlanMyTrip is able to provide appropriate travel route for their clients by.
