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

- Analysis: Both the Northern Hemisphere plot and Southern Hemisphere plot show some correlation between Latitude and Humidity. In the Northern Hemisphere plot, there is a negative relationship between Latitude and Max Temp, where as Latitude increases, Max Temp decreases. This is the reverse for the Southern Hemisphere, where there is a positive relationship between Latitude and Max Temp. This indicates that temperature decreases the further away you are from the equator, which logically makes sense. Furthermore, Southern Hemisphere has a stronger correlation, indicated by the higher slope (x) value. Additionally, the data fits the linear regression model better for the Southern Hemisphere, indicated by the higher r^2 value.


### Humidity

Northern Hemisphere: Humidity vs. Latitude

![reg3](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig7.png)

Southern Hemisphere: Humidity vs. Latitude

![reg4](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig8.png)



### Cloudiness

Northern Hemisphere: Cloudiness vs. Latitude

![reg5](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig9.png)

Southern Hemisphere: Cloudiness vs. Latitude

![reg6](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig10.png)



### Wind Speed

Northern Hemisphere: Wind Speed vs. Latitude

![reg7](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig11.png)

Southern Hemisphere: Wind Speed vs. Latitude

![reg8](https://github.com/caitlin-hartley/python-api-challenge/blob/main/output_data/Fig12.png)
