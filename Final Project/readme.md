# Supervised Machine learning to predict COVID-19 Lab result
Project By

Sharath Srinivas (AD59693)

## Introduction 
In this project supervised machine learning techniques are used to develop predictive models for the COVID-19 infection, using an epidemiology labeled dataset for positive and negative COVID-19 cases in Mexico, with supervised learning algorithms such as decision tree, logistic regression,Random Forest and naive Bayes, support vector machine, and k-nearest neighbors
## Problem Statement 
The global pandemic 2019-nCoV or COVID-19 is caused by the latest pandemic outbreak of the novel Severe Acute Respiratory Syndrome-Coronavirus two (SARS-CoV-2). The virus was first discovered in bats in late December 2019 in the Chinese province of Wuhan, with evidence suggesting it spread to people via intermediary hosts such as raccoons, dogs etc. Significant COVID-19 symptoms include fever (98%) cough (76%) and diarrhea (3%), which are generally more severe in older persons with chronic conditions , and many patients have reported shortness of breath, which in many cases appears to be a sign of the flu. , 2019 Since its discovery in late 2019, Covid has spread rapidly throughout the world.

## Motivation 
The healthcare and economic sectors are both at risk becasue of COVID-19. It's evident that non-clinical tools like machine learning, data mining, expert systems, and other artificial intelligence techniques will be crucial in diagnosing and containing the COVID-19 epidemic. The motivation of this project to contribute my domain and technical knowledge to fight against the disease

## Objectives 
To predict covid 19 results based on the symptoms of the patient.
In this project we will be using the Lab result of covid antigen test as our target variables.
## Dataset
The data set used was provided by Mexico's Epidemiological Surveillance System for Viral Respiratory Diseases and includes information on all COVID19-related cases, including positive and negative tested individuals. 
This data set is available for download using below link.
https://www.gob.mx/salud/documentos/datos-abiertos-152127
### Data Description
![image](https://user-images.githubusercontent.com/60420184/145940129-d60c65d5-6225-4b32-8852-f06241947f15.png)
## Exploratory Analysis
1. Dataset consists of  35 columns and 91188 rows
2. After importing the data frames dropped the all DATE columns along with nationality and information related to province/state because it will not help for our analysis
3. The columns "ENTITY RES" and " ENTITY UM" refer to the state of residence and treatment place respectively. These are coded by numbers so that they can be replaced by their respective names.
4. Formated the dataset by removing the rows containing 97 = 'NOT APPLICABLE', 98 = 'IGNORED', 99 = 'NOT SPECIFIED'.

## Conclusion
Early COVID-19 prediction can aid in minimizing the undue burden on healthcare systems by assisting in the diagnosis of COVID-19 patients. In this project prior to creating the models, the correlation coefficient analysis between various dependent and independent features was performed to establish the strength of the association between each dependent and independent feature of the dataset. Sixty percent of the training dataset was utilized to train the models, while the remaining fourty percent was used to test the models. The Random forest model has the highest accuracy of 78.80% percent followed by logistic regression, ADA boost and Gradient Boosting which lies around 65%.The performance of all models was evaluated based on accuracy parameters. In the EDA we can observe that patient male and female between age 40 to 60 are more likely to get Covid-19 and top 4 symptoms are Punemonia, Hypertension, Obesity and daibetes this indicates patients who have history of these decease must be carefully.

## Future Work
We only took the data of one day so after our intial analysis and with data preperation we left with 5000 to 6000 records out 91188. Data was imbalenced only the negative result data was more. For our Future work we try to combine 1 year data and check how the models predicts. 

## References
1. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC7694891/
2. https://www.gob.mx/salud/documentos/datos-abiertos-152127
3. https://www.geeksforgeeks.org/plot-a-pie-chart-in-python-using-matplotlib/

