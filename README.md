# SEOUL-BIKE-SHARING-PREDICTION-USING-REGRESSION-MODEL-MACHINE-LEARNING-

## Problem Description
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

## Data Description
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.
Attribute Information:
Date : year-month-day
Rented Bike count - Count of bikes rented at each hour
Hour - Hour of he day
Temperature-Temperature in Celsius
Humidity - %
Windspeed - m/s
Visibility - 10m
Dew point temperature - Celsius
Solar radiation - MJ/m2
Rainfall - mm
Snowfall - cm
Seasons - Winter, Spring, Summer, Autumn
Holiday - Holiday/No holiday
Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)


## What is the business use case of your project?
Users can verify their trip details (distance, duration) and measure of bodily activities (burnt calories). With this kind of smart technology and convenience, the use of Rental bikes is increasing every day. So, there is a need to manage the bike rental demand and manage the continuous and convenient service for the users. This study proposes a machine learning based approach including weather data to predict whole city public bike demand. A ML model is used to predict the number of rental bikes needed at each hour.

## What is the potential impact of your project?
 Findings provide a new option for researchers to predict hourly rental bike sharing demand.


## HOW you approached the problem statement? 
As the first step I’ve performed Exploratory data analysis, In EDA I’ve focused on rental bike counts over seasons, day, month, year, temperature, hour etc. I’ve divided the whole project into four parts EDA, Preprocessing, splitting into training and test set and last model building.

In preprocessing I’ve converted categorical columns into numerical columns as machine learning algorithms only understand numerical format. I’ve converted seasons, functioning day, date and holiday columns into numerical format. There was Multicollinearity present in the Temperature and dew point temperature column so I’ve merged both the columns. 

After preprocessing I’ve started building models. At first I used linear regression but as there was no Linearity between independent and dependent columns that’s the reason our linear regression model didn’t perform well I got the test score of 0.55. After that I’ve used regularised regression which are ridge and lasso regression but still we didn’t get a good score. 

After that I used a tree based model. I've used Decision tree regressor and Random forest, decision tree regressor have performed well with the test score of 0.84. After that I used ensemble technique as it overcomes the previous error of the tree. That's the reason our ensemble model performed really well as compared to other models. I’ve used Gradient boost and XGBoost. I got a test score of 0.92 for both Gradient and XGBoost, which is really good. 
