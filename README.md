### MACS 401 Final Project
# Gutenberg-Richer Law Regression
By: Declan Tracy


## Goals: 
To create a sequence of code that can take a list of earthquake imputs as a csv file and display them in a Gutenberg-Richer regression graph.  


## Motivation:
I am interested in better understanding the how the frequencies of high magnitude earthquakes compare to the frequency of smaller earthquakes. Additionally, I am interested in how the these frequencies in certain areas relate to frequencies in other areas. The Gutenberg-Richer regression equation shows this relationship, so making it very easy to quickly examine large amounts of earthquake data using this equation will be very helpful. By automating this proccess, it will be quite simple to download earthquake data and study it in this way.


## Data:
The datasets that I am using are the earthquake data gathered from the USGS Earthquake catelog. I am using the data from the Alaskan Subduction Zone, the San Andreas subduction zone, and the San Francisco Bay Area. I am using data spanning the time period of 2020 through 2021 for the Alaska and San Andreas datasets, and I am using data from 1965 through 2022 for the San Francisco Bay Area dataset. I am using data from all earthquakes with a magnitude 2 or higher recorded by the USGS in these areas. I intentionally selected datasets with differing size, temporal windows, and geographical size parameters to demonstrate the versitility of the program. The datasets that I used are included as csv files in this github page. The program I wrote is intended to run given any csv dataframe compiled in the same way that USGS sets up their data downloads, so feel free to try plugging in other datasets off of the USGS website!


## Data Analysis:
I am analyzing this data by graphing frequency of earthquakes against the magnitude that they occur at, and displaying the results on a logarithmic scale. This is known as the Gutenberg-Richer Law/Equation. In order to do this, I first pull all the magnitudes of each earthquakes from the csv dataframe, and add these to an array. After this, I sort the data by magnitude, making a variable for each magnitude value at 0.1 intervals. I then plot the occurances of earthquakes at each magnitude interval against that magnitude. The program I wrote has three dataslots, A, B, and C, to plug data into so that it is easy to quickly look at multiple datasets simultaneously. This means that the code performs each of the processes detailed above processes three times, one for each dataslot.

As stated before, this program is able to run regardless of what csv data file is imputed, as long as it is in an identical formal to those downloaded off of the USGS earthquake catelog. I have tested this by downloading a variety of datasets from the USGS catelog and imputing them into the program, and have had no issues. In addition, the graphs are set up to automaticlly format to fit the dataset, so no additional cleanup is required. The only limit is that it currently has a minnimum processing magnitude of 2.0. 


## References: 
Gutenberg and Richer, 1944
