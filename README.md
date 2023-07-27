# python-api-challenge

## WeatherPy

Imported dependencies
Generated a random list of cities and added the latitudes and longitudes to a list called cities.
Ran through the list of cities and set up the url to do an API query, making sure the temperature was in metric units.
Stored the latitude, longitude, max temperature, humidity, cloudiness, wind speed, country and date from the JSONs returned by the API and appended the values for each variable into an empty list.
Converted the compiled list into a dataframe and then exported the dataframe to a csv.
Created scatterplots that compared a city's latitude to the: 
  1. Maximum temperature ![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/579999d6-7efe-46e5-b680-b61ceb61747d)

  2. Humidity ![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/ad9dbdc9-98c8-4247-890f-3b7d2cd669e7)

  3. Cloudiness ![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/ffe543ea-d445-4f2b-b135-e456f3e4bdc4)

  4. Wind Speed ![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/1616e30b-b6d6-432b-b9d5-06638e6fec7e)

Created scatterplots for the same dataframe, but separated into northern and southern hemisphere with linear regression calculations.

Latitude vs. Maximum Temperature

![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/79fcb4e1-761e-48e4-abb1-c0307b568119)    ![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/709fcaca-523a-42e6-ad19-816d24eb59a9)

Latitude vs Humidity

![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/666e5ecb-69b3-49d5-9103-dcb818a692c6)    ![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/4b6b0a3e-f934-4246-a123-b57b3f7ecc09)


Latitude vs Cloudiness

![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/e485291d-916d-4931-bbe4-279420cecbd7)    ![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/e277f118-d9c2-4f7b-9a77-ab04e423ff1d)


Latitude vs Wind Speed

![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/fade5236-ccdc-4513-bbb3-ef0da559612d)    ![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/ec0552d2-b9e8-406f-9e09-4faa0e9e8bfa)


The average temperature of a given city showed a high corelation with distance from the equator. The closer a city is to the equator, the higher the maximum temperature is. Humidity, cloudiness and wind speed did not show strong correlations with latitude of a city. 
I suspect that other factors such as altitude, nearness to a body of water, and frequency of seismic activity show a higher correlation with these variables.


## VacationPy
Using the previous list of cities, I created a map with each city on it represented by a point with the size of the point proportional to the humidity.


![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/65148cc6-5bdf-49da-b716-1c3cda9e8efa)



I filtered the city data for cities with maximum temperatures between 13 and 32 degrees celsius, humidity lower than 40 g/m^3, and wind speeds slower than 3m/s.
Using GeoAPIfy, I looped through the cities that met my previous conditions and found hotels within 10 km of the city, storing the nearest hotel to the given latitude and longitude for each city. 
I then mapped each hotel and city on a map.

![image](https://github.com/Chemistasaurus/python-api-challenge/assets/132176159/4be8bd3a-fe03-4501-aa4f-b5ffefacdf3c)





