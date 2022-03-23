
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

# Conclusion

* The holiday or non-working days their is demand in rented bikes.

* In the Seoul City people prefer more rented bikes in the morning at 8 AM and  evening at 6 PM. As people might be going to their work at morning 8AM and returing from their work at the evening 6PM.

* Performing the various models, but the Random Forest is the best model that can be used for the Bike Sharing Demand Prediction since the performance metrics (mse,rmse) shows lower and (r2,adjusted_r2) shows a higher value for the Random Forest model.

* People won't prefer to go in rainfall. Similarly, in snowfall winter season the snowfall is continuous in the Seoul city, rented bike would impact in negative way because of cold whether.

* The Temperature, Hour & Humidity are the most important features that positively drive the total rented bikes count.

* To do more predictions we can use Random Forest model among all other model.


