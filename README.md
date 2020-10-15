# HeartFailureClinicalData

 > ## Introduction :

Kaggle dataset containing information of different clinical tests of 299 patients which can help in predicting chances of Heart Failure. Dataset is heavily imbalanced meaning, cases where Heart Failure occurs are less compared to that of healthy patients.
Dataset can be downloaded from url : *https://www.kaggle.com/andrewmvd/heart-failure-clinical-data*



 > ## Exploratory Data Analysis : 

First we need to understand the nature of each of the features in the data by performing Exploratory Data Analysis. This analysis can be found in IPython named **Heart Failure Predictions - EDA.ipynb .** 

As our main task is to predict the chances of Heart Failure, this proble is a Supervised Classification problem. Class labels distribution can be understood from feature *DEATH_EVENT* where out of given 299 patients, 32% cases Heart Failure was observed.

Out of the remaining 11 features, continuous and discrete features are understood by graphical representation. With the histograms of continuous variable, it was helpful to bin the same for better prediction in Modleing phase.



 > ## Modeling

Complete modeling can be understood from IPython named **Heart Failure Predictions - ML Modeling.ipynb.**
To check the underlying nature of complete data, plot of 2 dimensional representation of data using TSNE was plotted. This graph shows, the 2 dimensional representation data was linear in nature and can be separated with hyper-planes in higher dimension.

Different Linear as well Tree based classifiers are used to check the performance of model on given data. Hyper-parameter tuning of data can be done with the help of Cross Validation dataset. From final result table we can understood Logistic Regression without class balancing was performing better on given data.



> ## Final Run

As we understood the model which can run better on given data, we train Logistic Regression model on complete data and made a function which can return the prediction of the label for new class label and also the important features understood by model in predicting the class label.
