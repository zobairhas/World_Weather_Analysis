# world_weather_analysis

## Project Overview
The goal was to create a vacation itinerary across four different cities.
In order to create this I did the following:
- Retrieve Weather Data
- Create a Customer Travel Destinations Map
- Create a Travel Itinerary Map

## Methodology
- Tools/Programs/Languages used:
    - Python 
    - Jupyter Notebook
    - Pandas library
    - Citipy module
    - Numpy library
    - OpenWeatherMap API
    - Google Maps and Places API's
    

### Retrieve Weather Data
- First thing I did was generate 2,000 random latitudes and longitudes using the Numpy library. 
- From there, I constructed a URL so that I could call the OpenWeatherMap API. I also used the citipy module to identify the nearest city based on the coordinates. 
- After a massive list of cities were generated and added to an empty list, I then added all of that data to a Pandas DataFrame.
- Then I saved that data as a CSV file that can be accessed in the future. 


### Create a Customer Travel Destinations Map
- My city data was already saved as a CSV file so I imported the file as a DataFrame.
- Then I filtered by temperature so that the dataset would be manageable. 
- After that I cleaned the data up as there some empty names. From there I constructed my Google Directions API URL to call, request, and retrieve data in JSON format. 
- I saved the vacation data as a CSV. 
- Then I used the Gmaps marker layer to construct a map with markers for all of my cities. I also applied some formating so that the Hotel Name, City, Country, and Current Description with Max Temp would display. 
- This was the output:
```insert image link```

### Create a Travel Itinerary Map
- My vacation data was already saved as a CSV file so I imported the file as a DataFrame.
- Then I used the Gmaps marker layer to construct a map with markers for all of my cities. I also applied some formating so that the Hotel Name, City, Country, and Current Description with Max Temp would display. 
- After that I filtered the data so that only four cities would display. Then I used the Gmaps directions layer to set waypoints between the four cities. 
- This was the output:
```insert image```

-Finally, I added the Gmaps marker layer to the same four cities with the same format/info as the previous marker layers. 
-This was the output:
```insert image```
