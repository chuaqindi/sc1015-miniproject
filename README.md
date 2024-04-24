# SC1015 Mini Project: Predicting Telco Customer Churn


## About 
This is a Mini-Project for the SC1015 (Introduction to Data Science and Artificial Intelligence) module in Nanyang Technological University (NTU).

Our group aims to utilise customer data from Telcos to analyse the factors that affect churn and provide recommendations to reduce churn rate.

Dataset from Kaggle https://www.kaggle.com/datasets/mnassrib/telecom-churn-datasets by Baligh Mnassri.

### [-View compiled ipynb](https://github.com/chuaqindi/sc1015-miniproject/blob/main/All_models.ipynb) or follow the Walk-through in README file.

## Members

Lab FDDA Group 6: 

- Anshika Uppal
- Chua Qin Di
- Ting Zhi Hai, James


## Problem Definition 

Customer churn refers to customers that stopped using a company'services during a certain time frame. Churn analysis allows businesses to identify potential issues and take proactive measures to retain customers.

In the highly competitive telecommunications industry, customer churn is a critical challenge for telco businesses. It is roughly 6-7 times more expensive to acquire a new customer than it is to keep a current customer. Thus, even if the company gains a customer for every customer lost, they are still losing money. 

Thus, Telco businesses are seeking to develop models to predict and reduce churn, allowing the business optimize customer retention strategies and cultivate a stronger customer base.


## Models/ Libraries used
- Scipy
- PhiK
- GraphViz
- Imblearn
- Classification Tree
- Random Forest
- Logistic Regression
- XGBoost
- LightGBM


## Exploratory Data Analysis (EDA)

### [-View EDA ipynb](https://github.com/chuaqindi/sc1015-miniproject/blob/main/EDA.ipynb)



Our target variable, `Churn` is a boolean type variable. Hence, we used the following methods to carry out our EDA:

Feature importances:
- Boxplots of Numerical data against Churn
- Countplot of Categorical data against Churn

Correlation:
- Point biserial correlation (for Numerical Data)
- Phi k (𝜙k) correlation coefficent (for Categorical Data)


## Data Preparation

In this section, we prepared the dataset to be trained more accurately by our machine learning models.

- The dataset does not contain missing or NaN values
- However, we did notice that there was an inbalance in classes of the churn data.<br> Hence, we use Synthetic Minority Oversampling Technique (SMOTE) to generate more 'False' values in our Churn data 
- OneHotEncoding library was used to convert categorical data (in String format) to Integers


## Machine Learning
### 1. [View Logistic Regression, XGBoost, LightGBM ipynb](https://github.com/chuaqindi/sc1015-miniproject/blob/main/ClassificationTree_RandomForest.ipynb) <br> 2. [View Classification Tree & Random Forest ipynb](https://github.com/chuaqindi/sc1015-miniproject/blob/main/LogReg_XGBoost_LightGBM.ipynb) 


|      Performance Measure                    | Accuracy | ROC AUC | Precision | Recall | F1-Score |
| ------                             | ------ | ------ | ------ | ------ | ------ |
| XGBoost                            | 0.990248	 | 0.980960 | 0.990222 | 0.990248 | 0.990162 |
| LightGBM                           | 0.988747 | 0.983973 | 0.988708 | 0.988747 | 0.988636 |
| Random Forest with Hyperparameters | 0.984996	 | 0.989352 | 0.984947 | 0.984996 | 0.984779 |
| Random Forest                      | 0.983496 | 0.988223 | 0.983402 | 0.983496 | 0.983257 |
| Classification Tree                | 0.980495	 | 0.961857 | 0.980539 | 0.980495 | 0.980516 |
| Logistic Regression                | 0.791823 | 0.836494 | 0.867328 | 0.791823 | 0.815843 |

## Conclusion / Recommendations
 
XGBoost is the best machine learning model to classify our variables. 

The most important features were `Total day minutes`, `Total eve minutes`, `Total intl minutes` & `Account Length`.


In general,as customers use more of the telco services, they are more likely to discontinue the services. This suggests that telco businesses will have to look into long-term customer satisfaction and loyalty. 

The feature importances provides some insights into how telco businesses can improve their services. Firstly, telcos can look into improving the stability of the communication channels during day and evening timings, where it is expected to have higher traffic of customers. Next, they can look into retaining customers who make frequent international calls by improving the communication channels or by coming up with more enticing international plans.


## What we have learnt from this project 
- Methods to visualise and interpret data
- Upsampling data to increase prediction accuracy of model.
- New Machine Learning models: Logistic Regression, XGBoost, LightGBM
- Drawing conclusions from data and relating it to real-world issues
- Collaborating on GitHub


## References
https://www.pecan.ai/blog/how-why-churn-analysis-prediction/#why-analyze-customer-churn
https://www.kaggle.com/code/mnassrib/customer-churn-prediction-telecom-churn-dataset
https://www.kaggle.com/code/visionary20/orange-telecom-prevention-and-predicting-churn
https://www.datacamp.com/tutorial/understanding-logistic-regression-python
https://www.datacamp.com/tutorial/xgboost-in-python
https://phik.readthedocs.io/en/latest/

