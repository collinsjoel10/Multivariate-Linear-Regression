# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
import pandas as pd.

Step2
Read the CSV file.

Step3
Get the value of x and y variables.

Step4
Create the linear regression model and fit.

Step5
Predict the CO2 emission of a car where the weight is 2300Kg, and the volume is 1300cm3.

Step6
Print the predicted output.


## Program:
```

##Developed by:joel p
##REGISTER NUMBER: 22008934

import pandas as pd
from sklearn import linear_model

df = pd.read_csv("cars.csv")

X = df[['Weight', 'Volume']]
y = df['CO2']

regr = linear_model.LinearRegression()
regr.fit(X, y)

print('Coefficients:', regr.coef_)
print('Intercept:',regr.intercept_)

predictedCO2 = regr.predict([[3300, 1300]])
print('Predicted CO2 for the corresponding weight and volume',predictedCO2)









```
## Output:

![eb578267-11ad-41ae-b63d-cbb3532948ce](https://user-images.githubusercontent.com/118626456/214855709-e49a17ed-556d-4117-9ea4-335e77ecc2f0.jpg)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
