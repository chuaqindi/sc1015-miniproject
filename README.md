# SC1015 Mini Project: Predicting Telco Customer Churn


## About 
This is a Mini-Project for the SC1015 (Introduction to Data Science and Artificial Intelligence) module in Nanyang Technological University (NTU).<br>
Our group aims to utilise customer data from Telcos to analyse the factors that affect churn and provide recommendations to reduce churn rate.


## Contributors


## Problem Definition 

In the highly competitive telecommunications industry, customer churn is a critical challenge for telecomunication companies (Telco). <br>
Customer churn (or customer attrition) refers to the loss of customers due to dissatisfaction of the services provided and/or due to better offers 
from other companies. <br>
Churn results in a loss of revenue of the company and it has become increasingly difficult to retain customers today. <br>
Telco businesses are thus seeking to develop models to predict which customers are more likely to leave soon and take actions accordingly.



## Models/ Libraries used (Disclaimer: Ipynb will not run properly without these dependencies installed)
- PhiK
- GraphViz
- Imblearn
- Classification Tree
- Random Forest
- Logistic Regression
- XGBoost
- LightGBM


## Exploratory Data Analysis (EDA)
#### [Combined Ipynb](https://github.com/chuaqindi/sc1015-miniproject/blob/main/All%20models.ipynb)

## Data Preparation

Dataset from Kaggle https://www.kaggle.com/datasets/mnassrib/telecom-churn-datasets <br>

In this section, we prepared the dataset to be trained more accurately by our machine learning models.

- The dataset does not contain missing or NaN values
- However, we did notice that there was an inbalance in classes of the churn data. Hence, we use Synthetic Minority Oversampling Technique (SMOTE) to generate more 'False' values in our Churn data 
- OneHotEncoding library was used to convert categorical data (in String format) to Integers


## Machine Learning
#### 1. [Logistic Regression, XGBoost, LightGBM](https://github.com/chuaqindi/sc1015-miniproject/blob/main/ClassificationTree_RandomForest.ipynb) <br> 2. [Classification Tree & Random Forest](https://github.com/chuaqindi/sc1015-miniproject/blob/main/LogReg_XGBoost_LightGBM.ipynb) 


## Conclusion / Recommendations
 
XGBoost was the best machine learning model to classify our variables. The top 5 important features / variables given XGBoost are: "Total day minutes", "Total eve minutes", "Account Length", "Total intl minutes" and "Total night minutes".

In general,as customers use more of the telco services, they are more likely to discontinue the services. 
Telco companies can look into the other factors. ...


## What we have learnt from this project 
- Methods to visualise and interpret data
- Upsampling data to increase prediction accuracy of model.
- New Machine Learning models: Logistic Regression, XGBoost, LightGBM
- Drawing conclusions from data and relating it to real-world issues
- Collaborating on GitHub

## Contributions

## References
https://www.kaggle.com/code/mnassrib/customer-churn-prediction-telecom-churn-dataset
https://www.datacamp.com/tutorial/understanding-logistic-regression-python

