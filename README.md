# World_Weather_Analysis

 ## Basic Project Plan

Here's an outline of your project plan:

  - Task: Collect and analyze weather data across cities worldwide.

  - Purpose: PlanMyTrip will use the data to recommend ideal hotels based on clients' weather preferences.

  - Method: Create a Pandas DataFrame with 500 or more of the world's unique cities and their weather data in real time. This process will entail   collecting, analyzing, and visualizing the data.
  
  
## Your analysis of the data will be split into three main parts, or stages.

### 1. Collect the Data

   - Use the NumPy module to generate more than 1,500 random latitudes and longitudes.
    
   - Use the citipy module to list the nearest city to the latitudes and longitudes.
    
   - Use the OpenWeatherMap API to request the current weather data from each unique   city in your list.
    
   - Parse the JSON data from the API request.
    
   - Collect the following data from the JSON file and add it to a DataFrame:
    
       - City, country, and date
       - Latitude and longitude
       - Maximum temperature
       - Humidity
       - Cloudiness
       - Wind speed
      
### 2. Exploratory Analysis with Visualization

  - Create scatter plots of the weather data for the following comparisons:
       - Latitude versus temperature
       - Latitude versus humidity
       - Latitude versus cloudiness
       - Latitude versus wind speed
  - Determine the correlations for the following weather data:
       - Latitude and temperature
       - Latitude and humidity
       - Latitude and cloudiness
       - Latitude and wind speed
  - Create a series of heatmaps using the Google Maps and Places API that showcases the following:
      - Latitude and temperature
      - Latitude and humidity
      - Latitude and cloudiness
      - Latitude and wind speed
### 3. Visualize Travel Data

 Create a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. Complete these steps:

   1. Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
   2. Create a heatmap for the new DataFrame.
   3. Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
   4. Store the name of the first hotel in the DataFrame.
   5. Add pop-up markers to the heatmap that display information about the city, current maximum temperature, and a hotel in the city.



# Challenge
 ## Deliverable 1: Retrieve Weather Data (25 points)
 Deliverable 1 Instructions: Generate a set of 2,000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with the OpenWeatherMap. In addition to the city weather data you gathered in this module, use your API skills to retrieve the current weather description for each city. Then, create a new DataFrame containing the updated weather data.
 
 ## Deliverable 1 Requirements
 - Retrieve all of the following information from the API call: (15 pt)

   - Latitude and longitude
   - Maximum temperature
   - Percent humidity
   - Percent cloudiness
   - Wind speed
   - Weather description (for example, clouds, fog, light rain, clear sky)
 - Add the weather data to a new DataFrame (5 pt)
- Export the DataFrame as WeatherPy_Database.csv into the Weather_Database folder (5 pt)
- Be sure to double-check that you have the following in the Weather_Database folder:

    - The Weather_Database.ipynb file
    - The WeatherPy_Database.csv file

## Deliverable 2: Create a Customer Travel Destinations Map (35 points)
 Deliverable 2 Instructions: Use input statements to retrieve customer weather preferences, then use those preferences to identify potential travel destinations and nearby hotels. Then, show those destinations on a marker layer map with pop-up markers.

## Deliverable 2 Requirements
Deliverable 2 Requirements:
 - Input statements are written to prompt the customer for their minimum and maximum temperature preferences. (5 pt)
 - A new DataFrame is created based on the minimum and maximum temperature, and empty rows are dropped. (5 pt)
 - The hotel name is retrieved and added to the DataFrame, and the rows that don’t have a hotel name are dropped. (10 pt)
 - The DataFrame is exported as a CSV file into the Vacation_Search folder and is saved as WeatherPy_vacation.csv. (5 pt)
 - A marker layer map with pop-up markers for the cities in the vacation DataFrame is created, and it is uploaded as a PNG. Each marker has the following information: (5 pt)
     - Hotel name
     - City
     - Country
     - Current weather description with the maximum temperature
  - The marker layer map is saved and uploaded to the Vacation_Search folder as WeatherPy_vacation_map.png. (5 pt)
 - Be sure to double-check that you have the following in the Vacation_Search folder:

    - The Vacation_Search.ipynb file
    - The WeatherPy_vacation.csv file
    - The WeatherPy_vacation_map.png image

## Deliverable 3: Create a Travel Itinerary Map (40 points)
Deliverable 3 Instructions: Use the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations. Then, create a marker layer map with a pop-up marker for each city on the itinerary.

## Deliverable 3 Requirements:

 - Four DataFrames are created, one for each city on the itinerary. (10 pt)
 - The latitude and longitude pairs for each of the four cities are retrieved. (5 pt)
 - A directions layer map between the cities and the travel map is created and uploaded as WeatherPy_travel_map.png. (10 pt)
 - A DataFrame that contains the four cities on the itinerary is created. (10 pt)
 - A marker layer map with a pop-up marker for the cities on the itinerary is created, and it is uploaded as WeatherPy_travel_map_markers.png. Each marker has the following information: (5 pt)
   - Hotel name
   - City
   - Country
   - Current weather description with the maximum temperature
- Be sure to double-check that you have the following in the Vacation_Itinerary folder:
  - The Vacation_Itinerary.ipynb file
  - The WeatherPy_travel_map.png image
  - The WeatherPy_travel_map_markers.png image
