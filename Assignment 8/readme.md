# Question 
Analyze the data and create a processing pipeline. We are interested if we can predict whether a flight gets delayed or not (arr_delay).

Fit a logistic regression, decision tree, and SVM using grid search. Discuss the performance of each model.

Fit an ensemble using the three above models. Does this improvement performance?

Fit a model using AdaBoost. Does this improve performance?

## Flight Delay Prediction

### Data Definition

Flight Data contains 10000 rows and 25 columns

The Differebt columns are :

carrier
flight
tailnum
origin
dest
air_time
distance
hour
minute
temp
dewp
humid
wind_dir
wind_speed
wind_gust
precip
pressure
visib
type
manufacturer
model
engines
seats
engine
arr_delay

### EDA 
We observed that there are no postive co-relation between column wheb compared to arr_delay
