# Read-from-CSV

## AIM:
To write a python program for reading the csv file content.
## ALGORITHM:
### Step 1:
 Load the CSV into a DataFrame.
### Step 2:
 Import linear model from sklearn.
### Step 3:
 Declare weight and volume in x.
### Step 4:
 Declare CO2 in y.
### Step 5:
Using regression formula print the result.
## PROGRAM:
```
import pandas as pd
from sklearn import linear_model
data=pd.read_csv('car.csv')
x=data[['Weight','Volume']]
y=data['CO2']
regression=linear_model.LinearRegression()
regression.fit(x,y)
print("Coefficient:",regression.coef_)
print("Intercept:",regression.intercept_)
predictCO2=regression.predict([[3300,1300]])
print("CO2 required is",predictCO2)
```
## OUTPUT:
![Screenshot 2024-05-16 202534](https://github.com/Devadhaarini/Read-from-CSV/assets/145796552/3b4f42bb-1efe-4851-aa36-d60e077714e3)

## RESULT:
Thus the program is written to read the csv file.
