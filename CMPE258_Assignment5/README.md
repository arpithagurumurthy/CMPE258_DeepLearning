# **CMPE 258 Assignment 5**
New York City Taxi Fare Prediction

### Data :
Kaggle dataset link: https://www.kaggle.com/c/new-york-city-taxi-fare-prediction/data

- train.csv - Input features and target fare_amount values for the training set (about 55M rows).
- test.csv - Input features for the test set (about 10K rows). Your goal is to predict fare_amount for each row.

### ID
* key - Unique value identifying each row in both the training and test sets.

### Features
* pickup_datetime - timestamp indicating when the ride started.
* pickup_longitude - longitude coordinate of where the ride started.
* pickup_latitude - latitude coordinate of where the ride started.
* dropoff_longitude - longitude coordinate of where the ride ended.
* dropoff_latitude - latitude coordinate of where the ride ended.
* passenger_count - number of passengers in the ride.
### Target
* fare_amount - cost of the ride in dollars. 

### Description of the 4 files
CMPE258_HW5_PartA.ipynb : end to end tensorflow model pipeline
CMPE258_HW5_PartB.ipynb : end to end TFX interactivecontext pipeline
CMPE258_HW5_PartC.ipynb : end to end PyTorch implementation of the same
CMPE258_HW5_PartD.ipynb : end to end implementation using XGBoost


