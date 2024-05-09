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
## DATA HEAD
![328637595-bde29583-b6ae-4a22-b5fe-4c4fae4b052a](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/43deae2a-3f21-4dfc-ac0b-963d3a9f639a)
## DATA INFO
![328637691-7ba8517c-1727-4fba-afea-7bed30941e92](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/a338d294-731e-4657-a8d0-3f08f4fd708a)
### isnull() and sum():
![328637867-e09a6979-3cf4-41e6-879d-396e4b84a27b](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/d2734149-280f-43e0-8bb0-979d9d58916e)
### Data Head for salary
![328637983-fb7aef98-95e8-4983-a54c-a6c7d63beca9](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/0caccb4a-507c-4799-a797-933dd8f22ad8)
### MSE:
![328638036-d858df6f-f905-4243-848f-04695662f381](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/7a6f9092-27ff-4689-aade-145ea6206eb3)
r2:
![328638154-40f6226c-8dcf-4374-a342-7d566ccc3ee4](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/71b89bb0-3747-49ae-b264-a3df7a92b737)
### DATA PREDICTION:
![328638214-5fa7684c-e677-42d2-b9c6-dc14ddfeab2d](https://github.com/shivanshyam79/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/5aa60521-224f-4832-aa7f-8657c8a9bd8b)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
