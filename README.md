# sqlalchemy-challenge

In this challenge we've treated ourselves to a long holiday vacation in Honolulu, Hawaii. To help with the trip planning, we decide to do a climate analysis about the area. In order to accomplish these tasks we had to complete the following outline of items:

Precipitation Analysis
1. Find the most recent date in the dataset.
2. Using that date, get the previous 12 months of precipitation data by querying the previous 12 months of data.
3. Select only the "date" and "prcp" values.
4. Load the query results into a Pandas DataFrame, and set the index to the "date" column.
5. Sort the DataFrame values by "date".
6. Plot the results by using the DataFrame plot method
7. Use Pandas to print the summary statistics for the precipitation data.

Then we had to conduct a Station Analysis which included:

1. Design a query to calculate the total number of stations in the dataset.
2. Design a query to find the most-active stations (that is, the stations that have the most rows). To do so, we had to complete the following steps:
  2a. List the stations and observation counts in descending order.
  2b. Answer the following question: which station id has the greatest number of observations?
  2c. Using the most-active station id, calculate the lowest, highest, and average temperatures.

3.Design a query to get the previous 12 months of temperature observation (TOBS) data. To do so, we completed the following steps:
  3a. Filter by the station that has the greatest number of observations.
  3b. Query the previous 12 months of TOBS data for that station.
  3c.Plot the results as a histogram with bins=12, as the following image shows:

4. Close the session.

Finally we had to  complete Part 2 of tasks which entailed the: "Design Your Climate App"

We did this by designing a Flask API based on the queries that we  developed. Then we had to use Flask to create our routes as follows:

1. /
Start at the homepage.

List all the available routes.

2. /api/v1.0/precipitation
Convert the query results to a dictionary by using date as the key and prcp as the value.

Return the JSON representation of your dictionary.

3. /api/v1.0/stations
Return a JSON list of stations from the dataset.

4. /api/v1.0/tobs
Query the dates and temperature observations of the most-active station for the previous year of data.

Return a JSON list of temperature observations for the previous year.

5. /api/v1.0/<start> and /api/v1.0/<start>/<end>
  
Return a JSON list of the minimum temperature, the average temperature, and the maximum temperature for a specified start or start-end range.

For a specified start, calculate TMIN, TAVG, and TMAX for all the dates greater than or equal to the start date.

For a specified start date and end date, calculate TMIN, TAVG, and TMAX for the dates from the start date to the end date, inclusive.
