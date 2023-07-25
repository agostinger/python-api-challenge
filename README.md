# python-api-challenge
Cite: Collaboration with Ryan Himes, Juliet Hamilton

Using Python requests, APIs, and JSON traversals to answer a fundamental question: "What is the weather like as we approach the equator?"

Part 1: WeatherPy
In this deliverable, created a Python script to visualize the weather of over 500 cities of varying distances from the equator. Using the citipy Python libraryLinks to an external site., the OpenWeatherMap APILinks to an external site., and analysis to create a representative model of weather across cities.

Used the OpenWeatherMap API to retrieve weather data from a random list of cities generated. Then, created a series of scatter plots to showcase the following relationships:

A. Latitude vs. Temperature
B. Latitude vs. Humidity
C. Latitude vs. Cloudiness
D. Latitude vs. Wind Speed

Then, computed the linear regression for each relationship above. The plots were separated into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). A function was defined in order to create linear regression plots across all the relationships.

This function was used then to create a series of scatter plots for each relationship. A linear regression line, the model's formula, and the r values were included in the visualization.

Part 2: VacationPy

The list of cities and weather data generated in Part 1 was used to plan future vacations. This used Jupyter notebooks, the geoViews Python library, and the Geoapify API. The main focus was to use the Geoapify API and the geoViews Python library to employ Python skills to create map visualizations.

First, a map was created  that displays a point for every city in the city_data_df DataFrame. The size of the point was the humidity in each city.

Second, the DataFrame was narrowed down to my ideal weather conditions, which was less than 50% humidity and a maximum temperature less than 28 degress celsius.

Lastly, this new filtered data was used to create a new Dataframe called hotel_df, which brought in the city, country, coordinates and humidity. For each city, Geoapify API was used to find the first hotel located within 10,000 meters of the city's coordinates and plot on to a new map. The hotel name and the country was added as additional information in the hover message for each city on the map. 
