# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import required packages and read the data file.

2.Use LabelEncoder to convert categorical data into numerical data.

3.Split data into testing data and training data.

4.Apply Decision Tree Regressor.

5.Calculate mean squared error and R2.

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: BALASUDHAN P
RegisterNumber: 212222240017
 

import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.head()
data.isnull()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred)
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])

*/
```

## Output:
![240554254-fde479e5-8007-4f24-8ab6-26e9676576ce](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118807740/d4d8dfa2-cd59-4cef-b885-730f4127c196)

![240554349-5e88e334-6dd1-47dd-9dc9-f44ecae2208f](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118807740/39bb1312-dfb2-4545-893a-ecb2dd08f408)

![240554450-362bd089-1a64-4d61-abd0-2bad8edfc4a3](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118807740/3182e273-59bc-4bc4-840e-7722f0df70af)

![240554557-6a4e7642-fe74-475a-9abc-e2f08ce9fe92](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118807740/ba3c70ae-25dc-4e51-b90c-c2d47669cebc)

![240554655-0ad7a9b6-4506-4428-8590-6c91f21c7a35](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118807740/11abf069-c81c-429a-a086-87b840a59a52)

![240554818-106cd5f5-50fd-41d4-93bd-5a22674019fc](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118807740/9f7f6102-c518-46c3-9214-47fed961f73f)

![240554979-2df39b4a-d4bc-4b67-b36f-4597cc8bda26](https://github.com/BALASUDHAN18/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/118807740/3406a826-ddf1-4abd-beb3-d581308885a7)


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
