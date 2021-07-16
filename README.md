# PyBer Analysis

## Overview of the analysis: 

Here we are helping PyBer do some exploratory analysis using ride sharing data. We will use python scripts built using the Pandas library and Jupyter Notebook and the Matplotlib library to create descriptive graphs that will aid in telling our story effectively. Our aim is to showcase the relationship between types of cities, number of drivers and riders as well as the % of total fares for drivers and riders by type of city.

## Resources

### Development Environment
* Anaconda – versions 4.10.3 
* Jupyter Notebook – version 6.10.0 
* Python – version 3.8.8

### Dependencies

* Python Pandas library
* Python Matplotlib library 
* Python Numpy library 
* Python Scipy library

### Resources

* city_data.csv
* ride_data.csv

## Intital Analysis

The first thing we do is add the matplotlib inline magic command %Matplotlib inline – this command magically displays the graphs inside of the jupyter notebook . Next we import all our dependencies, the pandas, the numpy, scipy and matplotlib libraries. 

### Load and read the csv files city_data.csv and ride_data.csv

#### City_data.csv has the following information

* City
* Driver_count
* Type

#### Ride_data.csv has the following information

* City
* Date
* Fare
* Ride_ID

We check the data to make sure there are no nulls and that the data types are correct. 

#### Merge the two datasets using the common column “city” to create pyber_data 

We create the following summary dataframe

![image](https://user-images.githubusercontent.com/85518330/125996673-74f67118-c54d-40f5-896a-72ec412d4b7e.png)

## Findings

* Urban cities account for 68.4% of rides,  86.7% of drivers & 62.7% of fares 
* Rural cities account for 5.3 % of rides,  0.8% of drivers & 6.8% of fares
* Suburban cities account for 26.3% of rides,  12.5% drivers & 30% of fares  
* When we look at Average fares and Average fares per driver we find that 
* Urban cities have the lowest average fare per ride at $24.53 and average fare per driver at $16.57
* Suburban cities have the better average fare per ride at $30.97 and average fare per driver at $39.50
* Rural cities have the highest average fare per ride at $34.62 and average fare per driver at $55.49

We plotted the Average weekly fares between Jan & April 2019 by city type in a line graph as below and learnt the following from it

![PyBer_Fare_Summary](https://user-images.githubusercontent.com/85518330/125997951-be510099-aa1f-4d4c-afad-4e258a62c49b.png)

## Findings

* The average fares for Rural and Suburban cities have been more or less consistent over the 16 weeks of the analysis
* There is a sharp drop in the average fares of urban cities in the last two weeks of March 
* Overall across city types February seems to be a good month for average fares 

## Recommendations 

Our recommendations can be divided into 

### Opportunities
The penetration of our services is low in rural cities so there is scope to expand. The best news is that rural cities have higher average fares and higher average fares per driver. This can be used to motivate more drivers in rural markets to join hands. We need to draw up an aggressive marketing plan to promote PyBer in rural cities 

### Threats
Urban cities have adopted PyBer ride sharing services rather well and account for the largest share of the pie for us, however there is a threat from low average fares and a bigger  threat  from low driver fares. The CEO needs to address these two concerns else we may have unhappy, unloyal drivers and lower profitability because of lower avg fares to deal with in the near future

### Growth 
PyBer seems to be doing quite well in the Suburban cities, they account for a fair share of pie and also seem to have decent average fares and average fares per driver. The CEO should focus at acheiving growth in these markets while maintianing the high avg fares and high avg driver fares

### Other Factors
Lastly I feel the CEO needs to look at other factors that may be affecting average fares and avg fares per driver - like avg distance traveled per trip. It could well be that trips in rural cities while fewer may be longer distance trips causing higher fares per trip. 
Maybe we could also look at average profitability per ride and average driver revenue per trip rather than fares to get a better idea of the profitability of the trips 
