# Detecting Fraudulent Transactions

This project aims to combat online credit card fraud. The data is from Vesta, a leading corporation in the online payments space, on a transactional basis found on [Kaggle.com](https://www.kaggle.com/c/ieee-fraud-detection/data)

#### -- Project Status: [Completed]

## Project Objective
This project was my first foray into Machine Learning, and utilizes various modeling techniques, including Random Forests, xgboost, and KNN. The goal output will be a model that can be run real-time to predict if a transaction is fraudulent, while also minimizing false positives (i.e. predicting a transaction as fraud, when it is not).


### Methods
* Machine Learning:
    * xgboost, Decision Tree, Random Forest, Naive Bayes
* Adaptive Synthetic Over-sampling
    * generating random samples for our minority class
* GridsearchCV
    * parameter tuning

### Technologies
* Pandas - loading and pre-processing data
* Seaborn - plotting results
* imblearn - over-sampling unbalanced dataset
* sklearn - modeling

## Project Description
* #### EDA:
    To start, I first gathered information about my dataset, including the % of observations that fraud represents, $ amount of fraud transactions, avg fraud spend, distributions of the dataset.
    
* #### Clean Data/ Prepare for Modeling:
    The dataset included large amounts of missing data - in order to not lose out on missing data, I imputed the values using the median for each feature. I also wanted to balance the data, and utilized ADASYN to create new 'fraudulent' observations. The dataset was also train/test split to validate my model's efforts.
    
* #### Modeling:
    I first ran 'vanilla' models to determing my base scores, and improved upon using grid search to tune parameters to optimize my AUC score. In modeling, having a wide dataset with many features greatly increased tuning time, so implementing feature importance to remove non-important features was vital to my scoring efforts.



## Contact
* Feel free to contact me if any questions, or comments on the project - [hello@dancorley.com]