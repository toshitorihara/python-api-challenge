# What's the Weather Like: WeatherPy & VacationPy
![Equator](Images/equatorsign.png)

## Part I - WeatherPy
Create a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator using OpenWeatherMap API.

1. Create a series of scatter plots to showcase the following relationships: After each plot, add an explanation of what the code is analyzing. <br>
 - Temperature (F) vs. Latitude
 - Humidity (%) vs. Latitude
 - Cloudiness (%) vs. Latitude
 - Wind Speed (mph) vs. Latitude <br>

2. Run linear regression on each plots into Northern and Southern Hemisphere with descriptive analysis <br>
* Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
* Perform a weather check on each of the cities using a series of successive API calls.
* Include a print log of each city as it's being processed with the city number and city name.
* Save a CSV of all retrieved data and a PNG image for each scatter plot.

## Part II - VacationPy
Create weather data to plan future vacations. 
* Use jupyter-gmaps and the Google Places API for this part of the assignment.
* Create a heat map that displays the humidity for every city from Part I. 

![heatmap](Images/heatmap.png)

* Narrow down the DataFrame to find your ideal weather condition.
  * A max temperature lower than 80 degrees but higher than 70.
  * Wind speed less than 10 mph.
  * Zero cloudiness.
  * Drop any rows that don't contain all three conditions. 

![hotel map](Images/hotel_map.png)

* Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.
* Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.

## Submission
* Create a Jupyter notebook using Matplotlib or Pandas plotting libraries.
* For Part I, include a written description of **three observable trends** based on the data.
* For Part II, include a **screenshot of the heatmap** you create and include it in your submission.
* Use proper labeling of your plots, including aspects like: Plot Titles (with date of analysis) and Axes Labels.
* For max intensity in the heat map, try setting it to the highest humidity found in the data set.
* Ensure your repository has regular commits (i.e. 20+ commits) and a thorough README.md file.
