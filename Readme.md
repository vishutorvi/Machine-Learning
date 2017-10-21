# Project 1: Predicting sentiment from product reviews

The goal of this project is to explore logistic regression and feature engineering with existing GraphLab Create functions.
In this project i have Implemented

       a) Logistic Regression from stratch using gradient descent, log likelihood estimation ( Present in /ImplLogisticRegression)
       b) Using existing Logistic Regression for making sure My implementation works as good as existing ( Present in /LogisticRegression)
       c) implement your own logistic regression classifier with L2 regularization ( Present in /LogisticRegressionL2Regularization)

In this i have used product review data from Amazon.com to predict whether the sentiments about a product (from its reviews) are positive or negative. 

# Approach taken:

Using Existing Logistic Regression Model

	1) Use SFrames to do some feature engineering
	2) Train a logistic regression model to predict the sentiment of product reviews.
	3) Inspect the weights (coefficients) of a trained logistic regression model.
	4) Make a prediction (both class and probability) of sentiment for a new product review.
	5) Having the logistic regression weights, predictors and ground truth labels, written a function to compute the accuracy of the model.
	6) Inspect the coefficients of the logistic regression model and interpret their meanings.
	7) Compare multiple logistic regression models.

When implementing Logistic Regression with L2 regularization

	1) The goal of this second notebook is to implement your own logistic regression classifier with L2 regularization. You will do the following:
	2) Extract features from Amazon product reviews.
	3) Convert an SFrame into a NumPy array.
	4) Write a function to compute the derivative of log likelihood function with an L2 penalty with respect to a single coefficient.
	5) Implement gradient ascent with an L2 penalty.
	6) Empirically explore how the L2 penalty can ameliorate overfitting.


When Implementing logistic regression from scratch

	1) The goal of this notebook is to implement your own logistic regression classifier. You will:
	2) Extract features from Amazon product reviews.
	3) Convert an SFrame into a NumPy array.
	4) Implement the link function for logistic regression.
	5) Write a function to compute the derivative of the log likelihood function with respect to a single coefficient.
	6) Implement gradient ascent.
	7) Given a set of coefficients, predict sentiments.
	8) Compute classification accuracy for the logistic regression model


# Results:
Using Existing Logistic Regression classifier the accuracy of predicting sentiment was about: 89%. 
Using Customized Logistic Regression classifier the accuracy of predicting sentiment was about: 97.24%
Using Logistic Regression using L2 Regularization follow was the predictions:
Logistic Regression: 

	L2 penalty = 0
	train accuracy = 0.742900309247, validation_accuracy = 0.741480720754
	--------------------------------------------------------------------------------
	
	L2 penalty = 4
	train accuracy = 0.744222279927, validation_accuracy = 0.743067874148
	--------------------------------------------------------------------------------
	
	L2 penalty = 10
	train accuracy = 0.745379004273, validation_accuracy = 0.744561665577
	--------------------------------------------------------------------------------
	
	L2 penalty = 100
	train accuracy = 0.73909964354, validation_accuracy = 0.734011763608
	--------------------------------------------------------------------------------
	
	L2 penalty = 1000
	train accuracy = 0.501711479899, validation_accuracy = 0.498832975446
	--------------------------------------------------------------------------------
	
	L2 penalty = 100000
	train accuracy = 0.501569840183, validation_accuracy = 0.497805993838
	--------------------------------------------------------------------------------

# Future Work:
I will be trying out Other classifiers
