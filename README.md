# Introduction
The project involves predicting whether a person makes more than 50k dollars per year.

# About the data
The data was obtained from the following site http://archive.ics.uci.edu/ml/datasets/Census+Income (just click on this link and you will get the data). The detailed description of the data is also given in this link. Just to summarize, the data contains information on various features that can potentially impact an individual's earning capability such as age, type of employemnt (government, private, self-employed), race, sex, and many other.

# Project Description
The first step was to identitfy gaps in the data and remove them. After that, the data was manipulated to extract important statistical information from the data, the details of which can be found by going through the python notebook. After this, the model building was done seqentially to both shed light on the interrelations of the features and to finally build a predictor for predicting (or classifying as you wish to call it) whether a person earns more or less than 50k dollars per year. The details of the models are given below - 
## Logistic Regression
First, a logistic regression model was built taking yearly income as the dependent variable and occupation as the independent variable to see if a reasonably good prediction of the yearly income can be obtained just from the type of the occupation. In the second step a multivariate logistic regression model was built for predicting yearly income from the 'age', type of employment - 'workclass', and 'education' using an **80-20** split into training and testing set. The model gave more than **74 percent** of correct predictions out of the total number of predictions. 
## Decision Tree
A decision tree classifier was built using a **70-30** split of the data into training and testing sets. The model used all the features available in the dataset to classify a person's annual income into two categories - annual income more than 50k and less than 50k. The model gave more than **80 percent** of correct accurate predictions of the total number of predictions over the test set.
## Random Forest 
A random forest classifier was built using a **80-20** split of the data into training and testing sets. The model used all the features available in the dataset to classify a person's annual income into two categories - annual income more than 50k and less than 50k. The model gave more than **85 percent** of correct accurate predictions of the total number of predictions over the test set.
