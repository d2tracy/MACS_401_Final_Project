### MACS 401 Final Project
# Gutenberg-Richer Law Regression
By: Declan Tracy


## Goals: 
To create a sequence of code that can take a list of earthquake imputs as a csv file and display them in a Gutenberg-Richer regression graph.  


## Motivation:
I am interested in better understanding the frequency that magnitude 9.0 or greater earthquakes occur at, especially in Subduction zones. Additionally, I am interested in how the frequency of megathrust earthquakes compared to the frequency of smaller magnitude earthquakes. The Gutenberg-Richer regression equation shows this relationship, so making it very easy to examine large amounts of earthquake data using this equation will be very helpful.


## Data:
The datasets that I am using are the earthquake data gathered from the USGS Earthquake catelog. I am using the data from the Chilean subduction zone, the San Andreas subduction zone, and the Alaskan Subduction zone. I am using data spanning the time period of 2020 through 2021, and I am using all earthquakes with a magnitude 2 or higher. The datasets that I used are included as csv files in this github page. The program I wrote is intended to run given any csv dataframe compiled in the same way that USGS sets up their data downloads.


## Data Analysis:
I am analyzing this data by graphing frequency of earthquakes against the magnitude that they occur at, and displaying the results on a logarithmic scale. This is known as the Gutenberg-Richer Law/Equation. In order to do this, I first pull all the magnitudes of each earthquakes from the csv dataframe, and add these to an array. After this, I sort the data by magnitude, making a variable for each magnitude value at 0.1 intervals. I then plot the occurances of earthquakes at each magnitude interval against that magnitude. 

As stated before, this program is able to run regardless of what csv data file is imputed, as long as it is in an identical formal to those downloaded off of the USGS earthquake catelog. I have tested this by downloading a variety of datasets from the USGS catelog and imputing them into the program, and have had no issues. In addition, the graphs are set up to automaticlly format to fit the dataset, so no additional cleanup is required.


## References: 
Gutenberg and Richer, 1944
