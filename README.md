# Bayes_logistic_regression_DS_6014
Bayes DS 6014 Final Project

# GitHub Files 
Bayes Final Presentation – This is a copy of our presentation 
Bayes_Final_Project – This is our notebook with all the code 
default of credit card clients – This is the dataset used for the project it is also available at archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients
DS 6014 Bayes Final Report – This is a copy of our final report


## Project Description
Our dataset contains information on default payments, demographic information, credit history, payment history, and bill statements of credit card clients in Taiwan. The goal of our project is to not just predict whether or not a customer defaults on their credit card payment but also to measure the uncertainty around such predictions by analyzing the posterior probability of default. The data set contains 30,000 distinct credit card clients. The response is a binary classification of whether or not the customer defaulted. The predictors include the amount of given credit, gender, education, marital status, age, six months of history of past payment, six months of past bill statements, and six months of monthly payment.

By using a Bayesian framework for logistic regression rather than a frequentist approach, we are able to evaluate the uncertainty of not only our predictions but also of each predictor’s role in the model. This allows us to identify the impact that changes in the predictor values have on the probability that a customer will default. A key benefit of such an approach is that we can use soft classification for load decision making by evaluating the probabilities and uncertainties instead of making strict predictions based on a predetermined threshold.
Since our response, default, is a binary outcome, logistic regression is an obvious choice. However, by using Bayesian logistic regression, we treat the coefficients of the predictors in the model as random variables that come from some prior distribution rather than fixed values that must be estimated. This Bayesian approach allows us to obtain a mean and variance for each of the distributions of the coefficients, which enables us to measure their uncertainty. We can then use sampling or variational inference to approximate the posterior probabilities.

## Instructions to Reproduce Findings
-Download .csv file and .ipynb

-Install required packages

-run cells in sequence

This project is based heavily on pymc3. To learn more about pymc3, see https://docs.pymc.io/notebooks/getting_started.html. 

## Required Packages
python==3.8.5
pymc3==3.9.3
seaborn==0.11.0
graphviz
numpy
pandas
theano
arviz


