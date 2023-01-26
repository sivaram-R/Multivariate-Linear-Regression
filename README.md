# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
STEP 1:
Import Pandas library
<br>
STEP 2:
Import Linear_model from sklearn.
<br>
STEP 3:
Read the csv file using pandas library
<br>
STEP 4:
Enter the parameters of the linear function
<br>
STEP 5:
Print the parameters of the linear function.
## Program:
#student name:sivaram R
#reference no:22008680
```
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
![image](https://user-images.githubusercontent.com/121165794/214757512-d3ca0b17-ba26-44aa-958a-f7d64ce37d55.png)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
