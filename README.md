# SQLAlchemy 

## Climate Analysis and Exploration

In this project, I used Python and SQLAlchemy to do basic climate analysis and data exploration of the Honolulu,Hawaii's climate database. All of the following analysis were completed using SQLAlchemy ORM queries, Pandas, and Matplotlib.

### Precipitation Analysis

I designed a query to retrieve the last 12 months of precipitation data and then loaded the query results into a Pandas DataFrame to plot the results using the DataFrame `plot` method.

https://github.com/Samravp/sqlalchemy-challenge/blob/a1595e211037abb55b0758e5aceb1784846124ba/Images/Precipitation_Plot.png

### Station Analysis

For station analysis section, I designed a query to calculate the total number of stations and another query to find the most active stations.

Continueing on, I also designed a query to retrieve the last 12 months of temperature observation data (TOBS) and plotted the results as a histogram.

### Temperature Analysis I

I identified the average temperature in June and also in December at all stations across all available years in the dataset and followed by using a t-test to determine whether the difference in the means, is statistically significant. 

### Temperature Analysis II

My jupyter notebook contains a function called `calc_temps` that will accept a start date and end date in the format `%Y-%m-%d`. The function will return the minimum, average, and maximum temperatures for that range of dates.

I used this function to calculate the min, avg, and max temperatures for my trip using the matching dates from the previous year.

I plotted the min, avg, and max temperature from my previous query as a bar chart.


### Daily Rainfall Average

In this section, I calculated the rainfall per weather station using the previous year's matching dates.

My jupyter notebook contains a function called `daily_normals` that will calculate the daily normals for a specific date. This date string will be in the format `%m-%d`.

I created a list of dates for my imaginary trip :) in the format `%m-%d`, I used the `daily_normals` function to calculate the normals for each date string and append the results to a list.

Then, I loaded the list of daily normals into a Pandas DataFrame and set the index equal to the date.

I used Pandas to plot an area plot (`stacked=False`) for the daily normals.


## Climate App

After completing  the initial analysis, I designed a Flask API based on the queries that I had developed previously.


