# Python-API-Challenge

In this section, we'll create a Python script to visualize the weather of 500+ cities of varying distance from the equator.

Use a [simple Python library](https://pypi.python.org/pypi/citipy), the [OpenWeatherMap API](https://openweathermap.org/api), to create a representative model of weather across cities.

Create a series of scatter plots to showcase the following relationships

* Temperature (F) vs. Latitude

![Lattitude   Max Temp](https://user-images.githubusercontent.com/100891182/181995741-1a759d98-327a-41c1-bbdd-959ddc2acd8d.jpg)

* Humidity (%) vs. Latitude

![Latitue   Humidity](https://user-images.githubusercontent.com/100891182/181995747-58ee8464-703f-4079-b464-36aa1cfcc447.jpg)

* Cloudiness (%) vs. Latitude

![Latitude   Cloudiness](https://user-images.githubusercontent.com/100891182/181995756-0d16b778-a7da-4dd1-9892-a0c33a7dfc25.jpg)

* Wind Speed (mph) vs. Latitude

![Latitude   Wind speed](https://user-images.githubusercontent.com/100891182/181995763-21458a18-24c4-40a7-9d7a-16abd46ba71a.jpg)


Compute the linear regression for each relationship. 

* Northern Hemisphere - Temperature (F) vs. Latitude

![Northern Hemisphere - Max Temp vs  Latitude Linear Regression](https://user-images.githubusercontent.com/100891182/181995794-5325f864-e31c-40a7-9dd6-d3b5bf4b73e1.jpg)

* Southern Hemisphere - Temperature (F) vs. Latitude

![Southern Hemisphere - Max Temp vs  Latitude Linear Regression](https://user-images.githubusercontent.com/100891182/181995799-150a7f22-ab86-4ba5-801a-d8585935f41c.jpg)


* Northern Hemisphere - Humidity (%) vs. Latitude

![Northern Hemisphere - Humidity (%) vs  Latitude Linear Regression](https://user-images.githubusercontent.com/100891182/181995809-204c02ee-eebf-4f9c-a0d5-b557ddca9449.jpg)

* Southern Hemisphere - Humidity (%) vs. Latitude

![Southern Hemisphere - Humidity (%) vs  Latitude Linear Regression](https://user-images.githubusercontent.com/100891182/181995814-5d41afaa-62a1-46ca-81d5-5b968258ec01.jpg)

* Northern Hemisphere - Cloudiness (%) vs. Latitude

![Northern Hemisphere - Cloudiness (%) vs  Latitude Linear Regression](https://user-images.githubusercontent.com/100891182/181995818-6108bc37-35d8-432b-8198-01d4d46653b1.jpg)

* Southern Hemisphere - Cloudiness (%) vs. Latitude


* Northern Hemisphere - Wind Speed (mph) vs. Latitude

* Southern Hemisphere - Wind Speed (mph) vs. Latitude

![Southern Hemisphere - Wind Speed (mph) vs  Latitude Linear Regression](https://user-images.githubusercontent.com/100891182/181995831-f00195e6-a36e-445c-ac58-4185125605a6.jpg)

After each pair of plots, explain what the linear regression is modeling. For example, describe any relationships that you notice and any other findings you may have.
Final notebook must:

* Randomly select **at least** 500 unique (non-repeated) cities based on latitude and longitude.
* Perform a weather check on each of the cities using a series of successive API calls.
* Include a print log of each city as it's being processed, with the city number and city name.
* Save a CSV of all retrieved data and a PNG image for each scatter plot.

### Part 2: VacationPy

Now, let's use skills working with weather data to plan future vacations. Use Jupyter-gmaps and the Google Places API for this part of the assignment.

* **Note:** Remember that any API usage beyond the $200 credit will be charged to your personal account. You can set quotas and limits to your daily requests to be sure you can't be charged. Check out [Google Maps Platform Billing](https://developers.google.com/maps/billing/gmp-billing#monitor-and-restrict-consumption) and [Manage your cost of use](https://developers.google.com/maps/documentation/javascript/usage-and-billing#set-caps) for more information.

To complete this part of the assignment, we will need to do the following:

* Create a heat map that displays the humidity for every city from Part 1, as in the following image:

![Humidity Heatmap](https://user-images.githubusercontent.com/100891182/181995607-834375ed-a6f9-4a9a-9846-61b5360fbf50.png)


* Narrow down the DataFrame to find your ideal weather condition. 

  * Use Google Places API to find the first hotel for each city located within 5,000 meters of your coordinates.

* Plot the hotels on top of the humidity heatmap, with each pin containing the **Hotel Name**, **City**, and **Country**
![The Best Hotels](https://user-images.githubusercontent.com/100891182/181995613-457c5769-abf2-4dad-a34a-8eda69681823.png)


