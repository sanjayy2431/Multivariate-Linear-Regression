# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd    
### Step2   
Read the csv file    
### Step3
Get the value of X and y variables      
### Step4
Create the linear regression model and fit    
### Step5
Predict the CO2 emission of a car where the weight is 2300kg, and the volume is 1300cm cube     
### Step 6
Print the predicted output  
<br>
<br>
<br>
<br>
<br>
## Program:
```
#implemetation of multivariate linear regression
#Developed by: Sanjay v
#Register number: 212223230188
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("C:/Users/admin/Downloads/car.csv")
x=df[['Weight','Volume']]
y=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('coefficients:',regr.coef_)
print('Intercept:',regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
```

## Output:
![image](https://github.com/sanjayy2431/Multivariate-Linear-Regression/assets/149365143/c5b0434f-8a85-4217-9ba2-2a2734656ef3)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
