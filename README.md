# python-api-challenge
----------------------

[Weather](https://github.com/caitlin-hartley/python-api-challenge/blob/main/README.md#analyzing-weather-relative-to-the-equator-through-a-series-of-plots-and-regressions)

[Regression Plots](https://github.com/caitlin-hartley/python-api-challenge/blob/main/README.md#created-regression-plots)

----------------------

[Vacation!]

[Humidity Map!]

[Hotels Map!]

----------------------

# Analyzing Weather Relative to the Equator through a Series of Plots and Regressions

## Pull City Data and Create Scatter Plots

Used OpenWeatherMap API to retrieve weather data from the cities list generated in the code. Created a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature

![lattemp](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig1.png)

Latitude vs. Humidity

![lathumidity](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig2.png)

Latitude vs. Cloudiness

![latcloud](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig3.png)

Latitude vs. Wind Speed

![latwind](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig4.png)


## Created Regression Plots

Computed the linear regression for each relationship. Separated the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). Defined function to create linear regression plots.

### Temperature

Northern Hemisphere: Temperature vs. Latitude

![reg1](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig5.png)

Southern Hemisphere: Temperature vs. Latitude

![reg2](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig6.png)

Analysis: Both the Northern Hemisphere plot and Southern Hemisphere plot show some correlation between Latitude and Humidity. In the Northern Hemisphere plot, there is a negative relationship between Latitude and Max Temp, where as Latitude increases, Max Temp decreases. This is the reverse for the Southern Hemisphere, where there is a positive relationship between Latitude and Max Temp. This indicates that temperature decreases the further away you are from the equator, which logically makes sense. Furthermore, Southern Hemisphere has a stronger correlation, indicated by the higher slope (x) value. Additionally, the data fits the linear regression model better for the Southern Hemisphere, indicated by the higher r^2 value.


### Humidity

Northern Hemisphere: Humidity vs. Latitude

![reg3](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig7.png)

Southern Hemisphere: Humidity vs. Latitude

![reg4](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig8.png)

Analysis: Neither the Southern or Northern Hemispheres show significant correlation between Latitude and Humidity. This is represented by the low correlation values for both plots, as well as the low r^2 values, showing the model does not fit the data well. Both show a slightly negative relationship, but because the r^2 value is so low, it is difficult to draw any conclusions about the correlation between these variables. 


### Cloudiness

Northern Hemisphere: Cloudiness vs. Latitude

![reg5](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig9.png)

Southern Hemisphere: Cloudiness vs. Latitude

![reg6](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig10.png)

Analysis: Similarly to the Humidity regression plots, neither the Southern or Northern Hemispheres show significant correlation between Latitude and Cloudiness. The Northern Hemisphere shows a slightly more significant relationship, although the r^2 value is still very low. Again, both relationships are negative, but because the r^2 value is so low, it is difficult to draw any conclusions about the correlation between these variables. 



### Wind Speed

Northern Hemisphere: Wind Speed vs. Latitude

![reg7](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig11.png)

Southern Hemisphere: Wind Speed vs. Latitude

![reg8](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig12.png)

Analysis: There is virtually no correlation between Wind Speed and Latitude in both the Southern Hemisphere and Northern Hemisphere. The r^2 value is slightly higher for the Southern Hemisphere compared to the Northern Hemisphere, showing the data fits the model a little better. However, the only conclusion that can be drawn from these plots without further analysis is that there is no correlation between these variables.

Overall, temperature seems to be the only thing with a correlation relationship with latitude. Latitude seems to have little correlation with humidity, cloudiness, and wind speed, indicating that these weather conditions vary no matter the distance to the equator. 

----------------------

# Filtering Cities, Finding Hotels, Making maps

## Used the Geoapify API and the geoViews Python library to create map visualizations

Created a map that displays a point for every city in the city_data_df DataFrame with the size of the point the humidity in each city:

![humidity](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/humidity_map.png)

Filtered the data based on chosen weather conditions for prefered weather and loaded into new dataframe:

![chosen](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/filtering_cities.png)

Used Geoapify to find hotels within 10,000 meters of each city in the hotel dataframe. Created map with names of these cities and the hotels that were found within 10,000 meters. 

![hotels](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/hotels.png)

