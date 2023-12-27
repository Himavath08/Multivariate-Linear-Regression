# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:

1)Get the independent variable X and dependent variable Y.

2)Calculate the mean of the X -values and the mean of the Y -values.

3)Find the slope m of the line of best fit using the formula.

4)Compute the y -intercept of the line by using the formula: eqn2

5)Use the slope m and the y -intercept to form the equation of the line.

6)Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program:
```
#program for Implementation of Multivariate Linear Regression
#developed by: M Himavath
#register number: 23010121
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient: ",regr.coef_)
print("Intercept:",regr.intercept_)
print("Account",regr.predict([[3300,1300]]))





```
## Output:
![WhatsApp Image 2023-12-24 at 22 19 43_ecbd30e7](https://github.com/Himavath08/Multivariate-Linear-Regression/assets/139110631/5fdb7039-5e8c-44f2-bb90-873523e728e8)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
