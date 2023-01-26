# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>
Import Pandas library
### Step2
<br>
Import Linear_model from sklearn
### Step3
<br>
Read the csv file using pandas library
### Step4
<br>
Enter the parameters of the linear function
### Step5
<br>
Print the parameters of the linear function
## Program:
student name:sivaram R
reference no:22008680
```
developed by:sivaram R
reference no:22008680
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 to for the corresponding weight and volume",predictedCO2)
```
## Output:
![image](https://user-images.githubusercontent.com/121165794/214757165-3929f747-c951-4f50-a6ab-a4e27ce97e46.png)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
