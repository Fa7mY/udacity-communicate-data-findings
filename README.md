# Bike Sharing Dataset Exploration
## by *George Samir Fahmy*

> The data investigation is done as part of Udacity's Advanced Data Analysis Nanodegree program.

## Dataset

The dataset contains the daily count of rental bikes between years 2011 and 2012 in Capital
bikeshare system with the corresponding weather and seasonal information.
Bike-sharing rental process is highly correlated to the environmental and seasonal settings.
For instance, weather conditions, precipitation, day of week, season, hour of the day, etc. can affect the rental behaviors.
The original dataset has 731 entries across 16 columns.
The dataset can be found [here](https://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset)
Proper documentation and attributes definitions are to be found
[here](https://code.datasciencedojo.com/datasciencedojo/datasets/tree/master/Bike%20Sharing)

Since the original dataset encoded many categorical attributes in numerical formats,
an updated dataset is generated including the features of interest in their decoded string values.
A single entry is removed as it contained a humidity values of zero, which is physically impossible.
The updated dataset is stored as `day_updated.pkl`


## Summary of Findings

The investigation showed an above average relationship between the feeling temperature and the number
of bike rentals. This relationship is linear.

The two factors that also had a significant effect on the number of rented bikes are the season and
weather condition. With Fall being the peak season for bike renting, and a weather condition index of
1 providing the optimal condition for increased bike rentals.

A correlation between humidity, windspeed and feeling temperature was expected, however none were found.

The bike rentals across the year matched the expected from the seasons. In addition a significant jump
was observed in the number of rented bikes between 2011 and 2012.


## Key Insights for Presentation

In the presentation, the focus is on the different effectors of increased bike rentals. The presentation
starts with the distibution of bike rentals (which is shown to have a normal distribution), followed by
a plot visualizing the linear relationship between feeling temperature and bike rentals.

Afterwords, the qualitative attributes are introduced, starting with how the weekday had no significant
effect on the number of rented bikes. This is proceeded by highlighting the major factors from each
categorical attributes that is related to increased bike rentals (fall in season, and 1 in weather
situation).

Lastly, the trend across both years is shown, highlighting the observable increment in the bike rental
number from 2011 to 2012.
