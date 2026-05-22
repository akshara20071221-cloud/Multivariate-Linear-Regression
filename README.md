# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Import the required libraries such as pandas and LinearRegression from sklearn.

### Step2
<br>Read the dataset file using pd.read_csv() and store it in a dataframe.
### Step3
<br>Select the independent variables (Volume and Weight) as x and the dependent variable (CO2) as y.

### Step4
<br>Create the linear regression model using LinearRegression() and train the model using the fit() method.

### Step5
<br>Display the coefficient, intercept, and predict the output for the given input values using the predict() method.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))

```
## Output:
<img width="348" height="81" alt="Screenshot 2026-05-22 103638" src="https://github.com/user-attachments/assets/bc18b8c6-a75a-4741-a9c6-6d8590b3eaef" />


### Insert your output

<br><img width="348" height="81" alt="Screenshot 2026-05-22 103638" src="https://github.com/user-attachments/assets/bc18b8c6-a75a-4741-a9c6-6d8590b3eaef" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
