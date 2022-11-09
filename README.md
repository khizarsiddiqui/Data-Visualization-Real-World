# Data-Visualization-Real-World
Python program to work with real-world data sets extracted from CSV and JSON file formats.
This is a simple data set that contains only precipitation and temperature-related data. When you download your own weather data, you can choose to include a number of other measurements relating to wind speed, direction, and more detailed precipitation data.

# strptime()
Python interprets '%Y-' to mean the part of the string before the first dash is a four-digit year; '%m-' means the part of the string before the second dash is a number representing the month; and '%d' means the last part of the string is the day of the month, from 1 to 31. The strptime() method can take a variety of arguments to determine how to interpret the date. Table 16-1 shows some of these arguments.

# Shading an Area in the Chart
An alpha value of 0 is completely transparent, and 1 (the default) is completely opaque. By setting alpha to 0.5, we make the red and blue plot lines appear lighter.

# Downloading Your Own Data
If you want to download your own weather data, follow these steps:
1. Visit the NOAA Climate Data Online site at https://www.ncdc.noaa.gov/cdo-web/. In the Discover Data By section, click Search Tool. In the Select
a Dataset box, choose Daily Summaries.
2. Select a date range, and in the Search For section, choose ZIP Codes. Enter the ZIP Code you’re interested in, and click Search.
3. On the next page, you’ll see a map and some information about the area you’re focusing on. Below the location name, click View Full Details, or
click the map and then click Full Details.
4. Scroll down and click Station List to see the weather stations that are available in this area. Choose one of the stations, and click Add to Cart. This data is free, even though the site uses a shopping cart icon. In the upper-right corner, click the cart.
5. In Select the Output, choose Custom GHCN-Daily CSV. Make sure the date range is correct, and click Continue.
6. On the next page, you can select the kinds of data you want. You can download one kind of data, for example, focusing on air temperature, or you can download all the data available from this station. Make your choices, and then click Continue.
7. On the last page, you’ll see a summary of your order. Enter your email address, and click Submit Order. You’ll receive a confirmation that your order was received, and in a few minutes you should receive another email with a link to download your data.

# Examining JSON Data
We first import the json module to load the data properly from the file, and then store the entire set of data in all_eq_data. The json.load() function converts the data into a format Python can work with: in this case, a giant dictionary. We create a file to write this same data into a
more readable format. The json.dump() function takes a JSON data object and a file object, and writes the data to that file. The indent=4 argument
tells dump() to format the data using indentation that matches the data’s structure.

# Note 
When we talk about locations, we often say the location’s latitude first, followed by the longitude. This convention probably arose because humans discovered latitude long before we developed the concept of longitude. However, many geospatial frameworks list the longitude first and then the latitude, because this corresponds to the (x, y) convention we use in mathematical representations. The geoJSON format follows the (longitude, latitude) convention, and if you use a different framework it’s important to learn what convention that framework follows.

# World map
We set 'reversescale' to True, because we want to use bright yellow for the lowest values and dark blue for the most severe earthquakes. The 'colorbar' setting allows us to control the appearance of the colorscale shown on the side of the map. Here we title the colorscale 'Magnitude' to make it clear what the colors represent.

# Colors Scale
If you print the PLOTLY_SCALES dictionary, you can see how colorscales are defined.Every scale has a beginning color and an end color, and some scales have one or more intermediate colors defined as well. Plotly interpolates shades between each of these defined colors. This is impressive! In approximately 40 lines of code (hover and other things associated with it in eq_world_map.py), we’ve created a visually appealing and meaningful map of global earthquake activity that also illustrates the geological structure of the planet. Plotly offers a wide range of ways you can customize the appearance and behavior of your visualizations. Using Plotly’s many options, you can make charts and maps that show exactly what you want them to.