# Explore-Weather-Trends-data-analys-
Analysis of local and global temperature data and comparison of the temperature trends of a city to overall global temperature trends.

# Exploring Weather Trends.

**●** Introduction:
SQL Queries were used to download the CSV file that contains the yearly average temperature
of the City ‘Bangalore’ and the global temperature.
Then the data has been analysed using Python Programming Language and IPython Notebook
(Jupyter).

The analysed data has shown that the global temperature has been rising over the past years.

```
● Progress outline:
```
```
➔ SQL Query was used to download two CSV Files that contain :
```
1. Data about global temperature such as (“year”, “Average) and has been imported by
    using the query underneath:
       SELECT * FROM global_data;
2. The closest city to my country that has information about the same data plus the name
    of the country and the City, can be imported by using the query underneath:
       **SELECT * FROM city_data WHERE city=’Bangalore’ AND country=’India’;**

```
➔ Moving Averages:
```
1. Rolling Average has been calculated to smooth out data and to make it easier
    to observe the trends when it is shown in Charts.
2.The Rolling Average has been calculated for every 10 years to each single data
    but the first 10!
3.Python was used for calculating the Moving Average Using built-in functions
    such as rolling() and mean().
4.Python Code for what has been explained:
    **glb_mv_avg = globaltemp['avg_temp'] .rolling( 10 ) .mean()**

**local_mv_avg = citytemp[ 'avg_temp' ] .rolling ( 10 ) .mean ()** (^)
➔ Line Chart for the data:
Comparison of Bangalore temperature to global temperature


➔ .Two other charts for Global Temperature and Bangalore City separately.

Global temperature trend Bangalore temperature trend

```
● Observations:
➢ By noticing the charts, it is clear that the temperature is rising over the years due to
climate change.
➢ There is a delay from when the temperature in Bangalore was recorded as compared to
the global temperature recordings.
➢ Since 1975 the temperature is raising drastically.
➢ Bangalore city is getting hotter over time.
➢ The difference in change in temperature in Bangalore city over time in comparison to the
global average is small.
➢ The difference between 1800 and ~2010 in temperature is below 2 degrees in the
Global and the Bangalore average chart (increasing).
```
```
● Conclusion:
There is evidence suggesting that the global temperature is rising over the years which
support the case of climate change.
```


