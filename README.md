# Data Science Tools 1 Final Project - Kristoffer Sorensen
* COMP 4447
* Fall Quarter 2021

## Topic
Atlantic Ocean Temperature Fluctuation and the impact on Hurricane Intensity and Frequency

## Datasets
Data regarding Hurricane statistics will be collected from Kaggle, and will span from 1851 to 2015. Much of the data from the dataset is not used, and was removed during the cleaning process. The necessary data contained status symbols of 'HU' and allowed for specific focus on hurricanes only. Kaggle was provided the information from NOAA (National Oceanic and Atmospheric Administration) and was designed for data science projects.
  * https://www.kaggle.com/noaa/hurricane-database?select=atlantic.csv (atlantic.csv)

In regards to the Atlantic Ocean temperature data, that information was collected within the desired timeframe of 1851 to 2015. The main dataset only contained four columns titles as the following: year, annual anomaly, upper, and lower confidence. It's worth noting that the data is considered as deviations from 0 degrees Celsius and is easier to visualize on a graph.
  * https://www.metoffice.gov.uk/hadobs/hadcrut5/data/current/download.html (Summary Series - Northern Hemisphere - CSV - Annual)

## Current work
This is a relatively new field of research and has yet to have a set answer to its question. Much of the data requires several years of accurate information to make a proper answer. Using the data from 2016-2021 would help boost the information but unfortunately, meteorological data can take several years to be deemed 'ready'. Currently the topics answer is passed from how SST rise actually decreases hurricane generation rates to increasing it. Several more years of data collection will be needed to ensure an accurate result.

## Goals
Within this project, we want to identify several trends that can help present the connection between SST's and Hurricane frequency. Although, changing SST's cannot solely explain an increase/decrease in Hurricane frequency or intensity, we can say it is a contributor due to the necessity of it. The end results will show several numerical plots, plotting Hurricane strengths over time along side SST anomalies from that year.

## Methods and Libraries
The purpose of this project is to apply data cleaning techniques on historical environmental data. Several methods were used in this project, including:
* Pandas
* Matplotlib
* Seaborn
* NumPy
* Sklearn
* WordCloud

## Cleaning Issues
When using the Kaggle Hurricane data, I was met with an interesting set up. Each hurricane has several rows that detailed every 6 hours of its life cycle, complete with wind speeds from every direction (N, S, E, W), location in degrees, and several other unnecessary columns. Since the project only required a set amount of columns, I had to use a mix of repeated groupby() and pythonic functions to trim the data from 50,000 lines down to around 850. Objectives such as plotting the total amount of hurricanes per year was made increasingly more tedious than it should've been. What was very surprising was the lack of missing data. The only missing data that appeared was when a new column was created from previous results, of which was very easy to handle.

## Purpose
Climate science has been a personal project I have been looking into since my undergraduate, and working with the impacts it has on severe weather is one of my personal goals in life. Being committed to understanding how variables changing can impact storm generation has been always fascinating and combining that knowledge with the power of data analytics unlocks new pieces of information I have never seen. The purpose of this project was specifically created to look for changes regarding hurricane structure in comparison to one of the more important variables in its generation. Unlike land-based severe weather, tropical systems can have an impact on every part of the planet and I have been curious as to what we could expect to see in the future based off past trends and patterns.
