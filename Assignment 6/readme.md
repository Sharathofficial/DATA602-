### Assignment 3

## Medical Insurance Cost Datasets

Maching learning Assignment to perform EDA on the Medical Insurance Data of different patients The Data set has four numeric attributes and three categorical attributes

# Data Definition

The datasets consists of several medical predictor variables and one target variable, Outcome. Predictor variables includes the number of pregnancies the patient has had, their BMI, insulin level, age, and so on.

** Pregnancies **: Number of times pregnant
** Glucose **: Plasma glucose concentration a 2 hours in an oral glucose tolerance test
** BloodPressure **: Diastolic blood pressure (mm Hg)
** SkinThickness **: Triceps skin fold thickness (mm)
** Insulin **: 2-Hour serum insulin (mu U/ml)
** BMI **: Body mass index (weight in kg/(height in m)^2)
** DiabetesPedigreeFunction **: Diabetes pedigree function
** Age **: Age (years)
** Outcome **: Class variable (0 or 1)
** Number of Observation Units ** : 768 rows and 9 columns

# Business Question/Problem Statement
Implementation of  regression algorithm and predicting the Isurance amount based on other variables.

# EDA Observations
BMI has a outlier of above 45 and charges range from 1000 to 60000 As we observed above Sex and Region are categorical variable for the further regression we need to encode these values into numerical and then apply the Regression Algorithm

# Regression Results
## StatModel Linear 
#### Intial Result
R2 is 87% means the model is capturing 87% variance in the data.

There is no strong coorelation in any of the variable.

Age and smoking are the main factor for insurance charges because of high t- statstics.

We can't see any linear trend with Actual and predicted strengths.

When we compare the charges with all the variables we could not see any proper trend.

Removed Outlier in BMI and applied log Transformation on the charges to re-tun the statmodel
#### Final Result 
When we ran the regression model again on full dataset we observed R2 is increased to 91% and we can see some corellation now between variables
T-statstics for bmi, age increased and for somking it decreased.

Appears to be a normal distribution. There are no concerns about the residuals and we can see linear trend with Actual and predicted strengths.

## Linear Regression 

Pipeline Consists of OneHotEncoder to encode all the categorical variables and Standared scalar operation and OLS linear regression model
R2 values for both test is 79% and train data 74% is nearer so we can conculde no evidence of overfitting but we observed that no linearity between predicted and actual values 

## Ridge Regression

Used Ridge Regularization model for the above pipeline and observed there is no changes between OLS and Ridge model.

We observed that there is no clear linearity between predicted and actual values

## Lasso Regression

Used Lasso Regularization model for the above pipeline and observed there is no changes between OLS and Ridge model.

We observed that there is no clear linearity between predicted and actual values

#### Removed outlier for BMI and applied linear regression and regularization 
###### Linear Regression 
After removing the BMI Outlier we did not find much variation in R2 and Predicted and actual variable are not linear when we used linear regression 

###### Ridge Regression and Lasso Regression 
We observed that there is significant change in the R2 and value and model is predicting at 84% to 85%


# Conclusion
From the above Regression model we observed that all of our linear regression models scored similarly in the scoring metrics but after removing the outliers of the BMI we observed that Ridge and Lasso R2 increased significantly and there is no overfitting.

# Future Work

Applying featuring enginerring on the data set and may be classification and differnt methods would be used


