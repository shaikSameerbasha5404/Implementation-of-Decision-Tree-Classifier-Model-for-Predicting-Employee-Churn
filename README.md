# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas
2. Import Decision tree classifier
3. Fit the data in the model
4. Find the accuracy score

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Shaik Sameer Basha
RegisterNumber:  212222240093

import pandas as pd
data=pd.read_csv("/content/Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x=data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()    #no departments and no left
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])

*/
```

## Output:
#### data.head()
![6 1](https://github.com/shaikSameerbasha5404/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707756/6ae597c8-28ab-441a-9ae5-7b5560f0d6e2)

#### data.info()
![6 2](https://github.com/shaikSameerbasha5404/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707756/4c025146-e857-4b62-bae6-068e4b3a8f46)

#### isnull() and sum()
![6 3](https://github.com/shaikSameerbasha5404/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707756/fb53bfde-2589-47a8-bc26-d830a0b1fca1)

#### data value counts()
![6 4](https://github.com/shaikSameerbasha5404/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707756/325b6739-1236-4ab3-bcc2-8880a666104b)

#### data.head() for salary
![6 5](https://github.com/shaikSameerbasha5404/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707756/a36a0d90-dcd9-4d0b-a081-54309063bc3a)

#### x.head()
![6 6](https://github.com/shaikSameerbasha5404/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707756/09a2a464-0f8f-41e4-826f-eb9bda9ac676)

#### accuracy value
![6 7](https://github.com/shaikSameerbasha5404/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707756/f76952c9-ec6d-4524-a50b-2d86279c7233)

#### data prediction
![6 8](https://github.com/shaikSameerbasha5404/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/118707756/d8f13865-bd75-4183-a457-a0fc6d30ef4b)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
