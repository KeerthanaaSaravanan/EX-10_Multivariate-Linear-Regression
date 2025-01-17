# EX-10: Implementation of Multivariate Linear Regression
# Aim
To write a python program to implement multivariate linear regression and predict the output.

# Equipment’s required:
Hardware – PCs
Anaconda – Python 3.7 Installation / Moodle-Code Runner
# Algorithm:
Step1:
Import panda
Step2:
Import linear model from sklearn
Step3:
Read the file cars.csv
Step4:
Assign the values for x and y as required
Step5: 
Create the linearRegression model and predict the output
# Program:
```
'''
# Developed by: KEERTHANA S
# Register no: 23013398
'''

import pandas as pd
from sklearn import linear_model

df = pd.read_csv('employee.csv')

x = df[['Experience', 'Education']]
y = df['Salary']

regr = linear_model.LinearRegression()
regr.fit(x, y)

print("Coefficient:", regr.coef_)
print("Intercept:", regr.intercept_)

new_employee = [[5, 2]]  
predicted_salary = regr.predict(new_employee)

print("Predicted Salary for the corresponding experience and education:", predicted_salary)
```
# Output:
![Screenshot 2023-12-25 153402](https://github.com/KeerthanaaSaravanan/EX-10_Multivariate-Linear-Regression/assets/145742596/9b43054a-c7ab-46b3-bd4c-bbc125c235c4)
![Screenshot 2023-12-25 153241](https://github.com/KeerthanaaSaravanan/EX-10_Multivariate-Linear-Regression/assets/145742596/e4fb5217-c4a2-4419-98e2-0a988f14dd18)
![Screenshot 2023-12-25 153256](https://github.com/KeerthanaaSaravanan/EX-10_Multivariate-Linear-Regression/assets/145742596/e8274234-77ef-4187-ba76-89af5712de7e)


# Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
