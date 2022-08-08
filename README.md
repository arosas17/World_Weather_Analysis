### Overview

The overall goal is to create functions that will be useful for traveling; this would include a list of viable vacation locations filtered out by the customer to meet their preferences, such as temperature or particular weather. Besides this, the app should be able to identify nearby hotels and create a route to each city with an itinerary. In order to acheive this, this section was devided into three parts.

The first step was meant to create a list of cities and obtain their weather data, as seen in the Weather Database folder. This was performed by generating random latitudes and longitudes and then proceeding to apply them to real world locations. Obtaining the weather was done through an API provided by openweathermap.org. All this data was then made into a DataFrame, the one displayed below. This DataFrame was then converted to an csv file.


The second step had three main goals: filter out the cities by desired temperature from the list of cities provided from step 1, obtain a hotel name for each city that was still listed afterwards, and then place markers of the hotels on a map, with the marker containing information such as hotel name and max temperature. The filtered DataFrame that obtains the hotel names was made into a csv file to be used in step 3. The map is shown below.

The last step's purpose is to create directions between four cities, creating a circle. This is performed by using the csv file created in the previous step and determining four cities (in the same country) that are still fairly close together. After creating this route, a second map was created to display the marker textbox, displaying information. Images of these maps are displayed below.
