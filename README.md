# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1 Import the required libraries.
2 Upload the csv file and read the dataset.
3 Check for any null values using the isnull() function.
4 From sklearn.tree inport DecisionTreeRegressor.
5 Import metrics and calculate the Mean squared error.
6 Apply metrics to the dataset, and predict the output.


## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: shyam R
RegisterNumber:  212223040200
import pandas as pd
data = pd.read_csv("Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le = LabelEncoder()
data["Position"] = le.fit_transform(data["Position"])
data.head()
x = data[["Position","Level"]]
y = data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt = DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
mse = metrics.mean_squared_error(y_test,y_pred)
mse
r2 = metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
*/
```

## Output:
![Screenshot 2024-04-06 115129](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/5f99f1de-4e4f-423b-bd6e-736142e95633)
![Screenshot 2024-04-06 115217](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/6d4d13db-ca95-498f-bb37-484402506321)
![Screenshot 2024-04-06 115252](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/180a976c-5ecb-4860-a3bc-1e1eda2826fe)
![Screenshot 2024-04-06 115333](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/3eda1cf7-988d-4535-9b93-83ae87905949)
![Screenshot 2024-04-06 115406](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/54ba39fd-c294-4820-9f44-89cc31c707e3)
![Screenshot 2024-04-06 115438](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/97b2a2da-eefb-427e-9b50-f8cc39f7cac6)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
