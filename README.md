# Bike Sharing Assignment
> Linear Regression model for predicting demand of shared bikes.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- This project is part of course study assignment. The course is Advanced Certification Program in Machine Learning and Deep Learning (ACP in ML & DL) conducted by IIIT Banglore. The project is building a Linear Regression model for predicting demand of shared bikes.
- A US bike-sharing provider BoomBikes aspires to understand the demand for shared bikes among the people and the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market.

- The company wants to know:
1) Which variables are significant in predicting the demand for shared bikes.
2) How well those variables describe the bike demands

- Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
The EDA has following Observations.
- Average demand is highest in 'fall' followed by 'summer' then 'winter'. Demand is lowest in Spring and the drop looks more than 50%.
- Average demand in 2019 has surged by around 50% compared to 2018.
- There is gradual increase in average demand from January to September and then drops may be due to holiday season and/or snow/rain fall.
- There is low average demand on holidays than not-holiday, the drop looks around 30%.
- Average demand across week is stable.
- Average demand is same on working and non-working days though some non-working days there is low demand( lower quartile is lower than `working` in box-plot comparison).
- The average demand is high when the weather is clear and the drop in demand looks more than 50% when there is light rain/snow.
- The average demand on non-workingday is almost same as on workingday if it is not-holiday. As per the dictionary a non-working day which is not a holiday is a weekend so the demand is almost same on weekends as is on workingday.

#### With the r2_score of 0.81 on test data we are confident that the model fit isn't by chance, and has decent predictive power.

The equation of our best fitted line is:

cnt = 0.2036 + (0.2338 × yr) + (0.4923 × temp) + (-0.1498 × windspeed) + (-0.0680 × spring) + (0.0467 × summer) + (0.0831 × winter) + (-0.0486 × July)+ (0.0721 × sep) + (-0.0456 × Tues) + (-0.2856 × Light Rain) + (-0.0816 × Mist)

The above equation tells which features which variables are significant in predicting the demand for shared bikesa and how well those variables describe the bike demands.

Based on the final model the top 3 features which most contribute in predicting the demand are;

- ‘temp’ (Temperature)  which has positive correlation with demand for bikes.
- ‘Light Rain’  (Light rain/snow weather) which has negative correlation with demand for bikes.
- ‘yr’ (Year) which has positive correlation with demand for bikes.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Jupyter Notebook - version 6.5.4
- Python - version 3.11.5
- numpy - version 1.24.3
- pandas - version 2.0.3
- seaborn - version 0.12.2
- matplotlib - version 3.7.2

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project is done with reference to a example case study 'Predicting Price of House' covered in the course.


## Contact
Created by [@prithviraj2105] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->