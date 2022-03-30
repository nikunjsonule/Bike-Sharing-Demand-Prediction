
# Project Title

Seoul-Bike-Sharing-Demand-Prediction

# Problem Description

Currently Rental bikes are introduced in many urban cities 
for the enhancement of mobility comfort. It is important
 to make the rental bike available and accessible to the 
 public at the right time as it lessens the waiting time.
  Eventually, providing the city with a stable supply of 
  rental bikes becomes a major concern. The crucial part 
  is the prediction of bike count required at each hour for
   the stable supply of rental bikes.

# Data Description

The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall),
 the number of bikes rented per hour and date information.

# Attribute information

*  Date : year-month-day
*  Rented Bike count - Count of bikes rented at each hour
* Hour - Hour of he day
*  Temperature-Temperature in Celsius
*  Humidity - %
*  Windspeed - m/s
*  Visibility - 10m
*  Dew point temperature - Celsius
*  Solar radiation - MJ/m2
*  Rainfall - mm
*  Snowfall - cm
*  Seasons - Winter, Spring, Summer, Autumn
* Holiday - Holiday/No holiday
* Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)


# Summary of Project

Rental Bikes are introduced in many urban cities for the enhancement of mobility comfort. We were provided with ‘Seoul Bike Demand Prediction’ dataset to perform machine learning task, were to get insights from the independent and dependent variable of a dataset. By analyzing the problems with count of bikes rented at each hour the demand is getting increases with some specific times, seasons and whether. We’ve a data from 1st December 2017 till 30th November 2018. In this particular time duration we’ve all record and data with different seasons, whether, temperature, rented bike count, hour, humidity, visibility, solar radiation, rainfall, snowfall, holiday and functioning day.

As the first step, I performed data preprocessing and EDA part. I extracted features from ‘Date’ column, to get month, dayofweek and weekday_weekends. In EDA plotting heatmap for correlation, univariate and bivariate analysis, graphs and other plots to get some insights from the data. 

After data preprocessing, our data was ready to fit into the models. Different model used to get best accuracy score, models are – Linear Regression, implementing Lasso, Ridge and ElasticNet Regression, Decision Trees and Random Forest model.

The third step is to do some hyperparamter tuning. Doing GridSearchCV on Regularization(i.e Lasso, Ridge and ElasticNet)  part to get best accuracy and to shrink the coefficient. But it didn’t get a useful accuracy. 

As to get more insights from data, that which independent variable is more important when we fit data on model. Looking towards feature importance I noticed ‘temperature’ and ‘Hour’ are the most important variable for Decision tree and Random Forest model. There is slightly competition between ‘Solar Radiation’ and ‘Functioning Day_Yes’  with more necessary feature for model. The ‘temperature’ is the most feature importance among all features.

The final section is to observe model evaluation metrics. Linear regression, Lasso, Ridge and ElasticNet regression shows accuracy score with 56%. As for Decision Tree and Random Forest we get 77% and 84% adjusted R2 score respectively.

So accuracy of the best model is 84% for this dataset. This performance could be due to various reasons: no proper pattern of data, it may be some negligible noise in the data, different model give different accuracy score. 

# Machine Learning (Regression) Data Pipeline

1.	Data Preprocessing

2.	Exploratory Data Analysis

•	Univariate Analysis on numeric features

•	Bivariate Analysis

•	Analysis from categorical variables
                                
3. Fitting different models
                
•	Linear Regression

•	Building Lasso, Ridge and ElasticNet Regression

•	Decision Trees

•	Random Forest

4. Finding best parameters by GridSearchCV in Lasso, Ridge and ElasticNet
   Regression

5. Getting Feature Importance on Decision Tree and Random Forest model

6.    Model Evaluation Metrics

•	Mean square error

•	Root mean square error

•	R2

•	Adjusted R2


# Conclusion

* The holiday or non-working days their is demand in rented bikes.

* In the Seoul City people prefer more rented bikes in the morning at 8 AM and  evening at 6 PM. As people might be going to their work at morning 8AM and returing from their work at the evening 6PM.

* Performing the various models, but the Random Forest is the best model that can be used for the Bike Sharing Demand Prediction since the performance metrics (mse,rmse) shows lower and (r2,adjusted_r2) shows a higher value for the Random Forest model.

* People won't prefer to go in rainfall. Similarly, in snowfall winter season the snowfall is continuous in the Seoul city, rented bike would impact in negative way because of cold whether.

* The Temperature, Hour & Humidity are the most important features that positively drive the total rented bikes count.

* To do more predictions we can use Random Forest model among all other model.


