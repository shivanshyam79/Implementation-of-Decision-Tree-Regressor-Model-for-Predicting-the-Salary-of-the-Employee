# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. 
2. 
3. 
4. 

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: shyam R
RegisterNumber: 212223040200
import pandas as pd
data=pd.read_csv("C:/Users/admin/Downloads/Salary.csv")
data.head()
data.info()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data['Position']=le.fit_transform(data['Position'])
data.head()
x=data[['Position','Level']]
y=data['Salary']
from sklearn .model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_predicted)
mse
r2=metrics.r2_score(y_test,y_predicted)
r2
dt.predict([[5,6]])
*/
```

## Output:
![Screenshot 2024-04-06 113335](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/821cf500-3d57-4fb9-9d41-a80f59d53ccd)
![Screenshot 2024-04-06 113900](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/80ab2fd0-d7aa-490e-9c63-6140602f3d48)
![Screenshot 2024-04-06 113956](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/d6110cd7-ab86-4447-96c7-101b72470996)
![Screenshot 2024-04-06 114057](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/11356d20-5c84-401b-990c-df0ad5903861)
![image](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/8e3c93a8-0978-4e7a-ac18-e511f871218d)
![image](https://github.com/AkilaMohan/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/151513860/04a6a159-cdef-4adc-b281-9fbaca72d3f7)
![Uploading Screenshot 2024-04-06 114258.png…]()



## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
