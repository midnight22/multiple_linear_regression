# Umuzi assignment 3: Predicting salary differences
# Multiple Linear Regression

## Submission:
Create a notebook and commit your notebook changes to Github.
Once you are done, create an html report from the notebook.

## To complete this assignment, you should go through the following materials:
- [Robust One-Hot Encoding in Python](https://blog.cambridgespark.com/robust-one-hot-encoding-in-python-3e29bfcec77e)
- [Emulating R Regression Plots in Python](https://medium.com/@emredjan/emulating-r-regression-plots-in-python-43741952c034)
- [Statsmodels Regression Plot](https://www.statsmodels.org/dev/examples/notebooks/generated/regression_plots.html)
- [Test/Train Splits and Crossvalidation](https://towardsdatascience.com/train-test-split-and-cross-validation-in-python-80b61beca4b6)

## Instructions:
In the next series of challenges, we will predict employee salaries from different employee characteristics (or features).
Import the data salary.csv to a Jupyter Notebook. A description of the variables is given in the metadata. You will need the packages `matplotlib` / `seaborn`, `pandas` and `statsmodels`.

## Answer the following questions:
Split your data into a training and test set. Train your model using the training set and use multiple linear regression to predict salary from all the variables in the training dataset.

1. Create scatterplots, histograms, and a descriptive statistics table of the variables of interest.
2.	One-hot encode the variable Field into three dummy variables, using HR as the reference category. You can use `pandas`' get_dummies() function for this.
3.	Produce a correlation matrix comparing the relationship of salary to the predictor variables. Is there any multicollinearity or other problems that may be a problem in the multiple regression?
4.	Run the multiple linear regression and interpret the standardised coefficients given in the statsmodels output. What are the most important features when predicting employee salary?
5.	Calculate the standardised residuals (resid()) and standardised predicted values (fittedvalues()).
6. Plot the residuals versus the predicted values using `seaborn`'s `residplot` with fitted values as the x parameter, and the dependent variable as y. lowess=True.
  * Are there any problems with the regression?

Now run your model on the test set.

7. How does your model compare when running it on the test set - what is the difference in the Root Mean Square Error (RMSE) between the training and test sets?
