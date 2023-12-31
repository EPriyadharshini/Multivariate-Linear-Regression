# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Read the csv file.

### Step3
Get the value of X and y variables.

### Step4
Create the linear regression model and fit.

### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm3

## Step6:
Print the predicted output.

## Program:
```

##Developed by:E.PRIYADHARSHINI
##Register number: 23012593

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("sricar.csv")
a=df[['Weight','Volume']]
b=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3400,1350]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)

```
## Output:


<img width="443" alt="image" src="https://github.com/EPriyadharshini/Multivariate-Linear-Regression/assets/144870831/035bdfd5-a77c-48fe-97ef-5b42f1e1c3cd">



### Insert your output
```
Coefficient: [0.00755095 0.00780526]
Intercept: 79.69471929115939
Predicted CO@ for the corresponding weight and volume [115.90503767]
```

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
