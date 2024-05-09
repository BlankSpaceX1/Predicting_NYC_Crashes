# Predicting_NYC_Crashes

## Introduction 

My chosen data set for my final project concerns motor vehicle accidents in NYC,
taking into consideration the severity of the collision, in addition to its 
location and other relating factors. Only a sample of this data was collected
ranging from the dates of December 31, 2017 at 11:59:59 PM to January 1, 2024
at 12:00:00 AM. 

## Specific aims 

* What time do most crashes occur?

* Which borough sees the most injuries in collisions for each category?

* Which borough sees the most fatilities in collisions for each category?

* Is it possible to map out all accidents by borough?

* Which areas are the most dangerous for pedestrians?

## Data description

The chosen data set is NYC Arrest Data (December 31, 2017 at 11:59:59 PM to January 1, 2024
at 12:00:00 AM). The source of the data is on [NYC Open Data](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95/about_data)


We can see that the feather file contains over 544,085 points of data spread out 
over 29 different features. While most of this data is clean from the initial 
query, there are still many fields that contain null values, namely the columns
of `CONTRIBUTING FACTOR VEHICLE` 3-5, in addition to `VEHICLE TYPE CODE` columns
3-5. I attribute this to my suspicion that most motor vehicle accidents involve 
only two parties. However, I believe this question will be answered after 
thoroughly investigating the data during the cleaning process. There also exist
null values in the `BOROUGH` and `ZIP CODE` columns, but those values can be 
reverse geocoded with the proper coordinate data.

## Research design/methods/schedule

One of the main features of my project is to create a heatmap of all the 
accident data in the present dataset. However, to start this process, the data 
will first have to be reverse geocoded and cleaned. Additionally, information 
about different areas will be included at the zipcode level to create a better 
picture of which factors may contribute to higher collisions in an area and how
deadly they are. From this data, I expect to create a machine learning model 
that will help users understand which factors may be contributing to more 
crashes by analyzing the differences between predicted crashes and fatalities 
in an area versus the actual observed values of these factors. I then hope to 
summarize these results in a dashboard that will help non-data scientists 
understand the conclusions of this project.

## Discussion and Conclusion 

In this project, I hope to analyze New York City motor collision data to 
investigate which areas of New York City experience the most amount of 
collisions, in addition to their injury and fatality rates. 