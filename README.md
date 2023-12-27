# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import an package of panda and from sklearn import linear_model
<br>

### Step2
Then link the data available csv file as an variable data
<br>

### Step3
then take weight and volume as x and CO2 as y
<br>

### Step4
using linear_model.LinearRegression() fit as x and y Then predict the output
<br>

### Step5
End the program.
<br>

## Program:
```
# Implement of Multivariate linear regression and predict the output
# Developed By: AKASH KUMAR M.
# Reference number:212223230010
import pandas as pd
from sklearn import linear_model
data=pd.read_csv("cars (1).csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predictCO2)





```
## Output:
![output](https://github.com/akash7812/Multivariate-Linear-Regression/assets/146819826/54156dd9-5486-4d8e-a80a-48a5497c4454)



<br>

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
