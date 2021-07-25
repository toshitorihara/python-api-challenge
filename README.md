# What's the Weather Like As We Approach the Equator?
![Equator](Images/equatorsign.png)

## Part I - WeatherPy
Create a Python script to visualize the weather of 500+ cities across the world of varying distance from the equator. To accomplish this, you'll be utilizing a simple Python library, the OpenWeatherMap API, and a little common sense to create a representative model of weather across world cities. <br>

1. Create a series of scatter plots to showcase the following relationships:
 - Temperature (F) vs. Latitude
 - Humidity (%) vs. Latitude
 - Cloudiness (%) vs. Latitude
 - Wind Speed (mph) vs. Latitude <br>
After each plot, add a sentence or two explaining what the code is analyzing. <br>

2. Run linear regression on each relationship. Separate the plots into Northern Hemisphere and Southern Hemisphere:
* Northern Hemisphere - Temperature (F) vs. Latitude
![NoTemp](Images/.png)
* Southern Hemisphere - Temperature (F) vs. Latitude
![SoTemp](Images/.png)
* Northern Hemisphere - Humidity (%) vs. Latitude
![NoHumid](Images/.png)
* Southern Hemisphere - Humidity (%) vs. Latitude
![SoHumid](Images/.png)
* Northern Hemisphere - Cloudiness (%) vs. Latitude
![NoCloud](Images/.png)
* Southern Hemisphere - Cloudiness (%) vs. Latitude
![SoCloud](Images/.png)
* Northern Hemisphere - Wind Speed (mph) vs. Latitude
![NoWind](Images/.png)
* Southern Hemisphere - Wind Speed (mph) vs. Latitude 
![SoWind](Images/.png)
<br>
 
After each pair of plots, take the time to explain what the linear regression is modeling. For example, describe any relationships you notice and any other analysis you may have. Your final notebook must:<br>
* Randomly select at least 500 unique (non-repeat) cities based on latitude and longitude.
* Perform a weather check on each of the cities using a series of successive API calls.
* Include a print log of each city as it's being processed with the city number and city name.
* Save a CSV of all retrieved data and a PNG image for each scatter plot.

## Part II - VacationPy
Now let's use your skills in working with weather data to plan future vacations. 
* Use jupyter-gmaps and the Google Places API for this part of the assignment.
* Create a heat map that displays the humidity for every city from Part I. 

![heatmap](Images/heatmap.png)

* Narrow down the DataFrame to find your ideal weather condition. For example:
  * A max temperature lower than 80 degrees but higher than 70.
  * Wind speed less than 10 mph.
  * Zero cloudiness.
  * Drop any rows that don't contain all three conditions. You want to be sure the weather is ideal.
  * Note: Feel free to adjust to your specifications but be sure to limit the number of rows returned by your API requests to a reasonable number.<br>

* Using Google Places API to find the first hotel for each city located within 5000 meters of your coordinates.
* Plot the hotels on top of the humidity heatmap with each pin containing the Hotel Name, City, and Country.

![hotel map](Images/hotel_map.png)

## Submission
* Create a [**Jupyter notebook**](.ipynb) using Matplotlib or Pandas plotting libraries.
* For Part I, include a written description of **three observable trends** based on the data.
* For Part II, include a **screenshot of the heatmap** you create and include it in your submission.
* Use proper labeling of your plots, including aspects like: Plot Titles (with date of analysis) and Axes Labels.
* For max intensity in the heat map, try setting it to the highest humidity found in the data set.
* Ensure your repository has regular commits (i.e. 20+ commits) and a thorough README.md file.
