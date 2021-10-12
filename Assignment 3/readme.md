### Assignment 3

## Medical Insurance Cost Datasets

Maching learning Assignment to perform EDA on the Medical Insurance Data of different patients The Data set has four numeric attributes and three categorical attributes

# Data Source
Data has been extracted from Kaggle : https://www.kaggle.com/jagjeet555/medical-charges-prediction

# Data Definition
**age**: age of primary beneficiary

**sex**: insurance contractor gender, female, male

**bmi**: Body mass index, providing an understanding of body, weights that are relatively high or low relative to height, objective index of body weight (kg / m ^ 2) using the ratio of height to weight, ideally 18.5 to 24.9

**children**: Number of children covered by health insurance / Number of dependents

**smoker**: Smoking

**region**: the beneficiary's residential area in the US, northeast, southeast, southwest, northwest.

**charges**: Individual medical costs billed by health insurance


# Business Question/Problem Statement
Implementation of  regression algorithm and predicting the Isurance amount based on other variables.

# EDA Observations
BMI has a outlier of above 45 and charges range from 1000 to 60000 As we observed above Sex and Region are categorical variable for the further regression we need to encode these values into numerical and then apply the Regression Algorithm

# Regression Results
## StatModel Linear 
#### Intial Result
R2 is 87% means the model is capturing 87% variance in the data
There is no strong coorelation in any of the variable
Age and smoking are the main factor for insurance charges because of high t- statstics
We can't see any linear trend with Actual and predicted strengths
When we compare the charges with all the variables we could not see any proper trend
