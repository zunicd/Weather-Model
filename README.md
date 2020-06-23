# Weather-Model

## Part I - WeatherPy

**Summary dashboard**: https://zunicd.github.io/Web-Design-Challenge/

### Objective

The purpose of this project was to analyze weather patterns with respect to latitude. 

To visualize the weather of 500+ randomly chosen cities across the world of varying distance from the equator, first we used a `citypy` Python library and then the [OpenWeatherMap API](https://openweathermap.org/api). 

After assembling the dataset, we used Matplotlib to create a series of scatter plots to showcase the relationships between different weather factors (temperature, humidity, cloudiness, wind speed) and latitude.

In addition to that I ran linear regression on each relationship, only this time separating them into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude).



## Part II - VacationPy

### Objective

First, we created a heat map that displays the humidity for every city from the Part I. 

![](C:\Users\zunic\Butler\DataBootCamp\github\Weather-Model\Images\heatmap.png)

Next, we narrowed down our dataframe to ideal weather conditions:

- A max temperature lower than 80 degrees but higher than 70.

- Wind speed less than 8 mph.

- Zero cloudiness.


The resulted list contained 11 cities. Using Google Places API we found the first hotel for each city located within 5000 meters. At the end, we plotted the hotels on top of the humidity heatmap with each pin containing the **Hotel Name**, **City**, and **Country**.

![](C:\Users\zunic\Butler\DataBootCamp\github\Weather-Model\Images\hotel_map.png)



###  Tools / Techniques Used:

- Python
- Pandas
- Matplotlib
- Numpy
- SciPy
- Jupyter Notebook
- gmaps
- citypy
- OpenWeatherMap API
- Google Places API



### About Data

 The dataset *output_data/cities.csv* was created in the Part I and used as an input in the part II:

-  **Number of records:**      567
-  **Columns**:
   -  City
   -  Cloudiness
   -  Country
   -  Date
   -  Humidity
   -  Lat
   -  Lng
   -  Max Temp
   -  Wind Speed