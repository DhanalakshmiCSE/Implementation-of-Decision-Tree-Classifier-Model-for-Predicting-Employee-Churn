# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. import pandas module and import the required data set.

2.Find the null values and count them.

3.Count number of left values.

4.From sklearn import LabelEncoder to convert string values to numerical values.

5.From sklearn.model_selection import train_test_split.

6.Assign the train dataset and test dataset.

7.From sklearn.tree import DecisionTreeClassifier.

8.Use criteria as entropy.

9.From sklearn import metrics.

10.Find the accuracy of our model and predict the require values.
 

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Dhanalakshmi S
RegisterNumber:212222040033

import pandas as pd
data = pd.read_csv("Employee.csv")
data.head()
data.info()
data.isnull().sum()
data["left"].value_counts
from sklearn.preprocessing import LabelEncoder
le= LabelEncoder()
data["salary"]=le.fit_transform(data["salary"])
data.head()
x= data[["satisfaction_level","last_evaluation","number_project","average_montly_hours","time_spend_company","Work_accident","promotion_last_5years","salary"]]
x.head()
y=data["left"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size=0.2,random_state = 100)
from sklearn.tree import DecisionTreeClassifier
dt = DecisionTreeClassifier(criterion="entropy")
dt.fit(x_train,y_train)
y_pred = dt.predict(x_test)
from sklearn import metrics
accuracy = metrics.accuracy_score(y_test,y_pred)
accuracy
dt.predict([[0.5,0.8,9,260,6,0,1,2]])


*/
```

## Output:

## 1.DATASET:

 ![1](https://github.com/DhanalakshmiCSE/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119477832/74fc8e45-0a8e-42b2-ae5c-d2c9de64b36e)

## 2.df.head()

![2](https://github.com/DhanalakshmiCSE/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119477832/a56d0683-2078-4e5f-a72a-cc5ef4141829)

## 3.X.head()

![3](https://github.com/DhanalakshmiCSE/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119477832/c1c90423-e72a-4c30-b9ab-9e881e057a6e)

## 4.df.info()

![4](https://github.com/DhanalakshmiCSE/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119477832/a735caea-1c47-4027-a4ce-a8f26d2e4412)

## 5.ISNULL:

![5](https://github.com/DhanalakshmiCSE/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119477832/2e9e76f3-1737-48a0-b3e7-e82b1c3570f7)

## 6.VALUE COUNTS:

![6](https://github.com/DhanalakshmiCSE/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119477832/40f72006-6eff-4514-b779-859be11e00e6)

## 7.Data transformed head:

![7](https://github.com/DhanalakshmiCSE/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119477832/ba0944f7-fcb7-4cc0-a620-16eed70cffe6)

## 8.DECISION TREE:

![8](https://github.com/DhanalakshmiCSE/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119477832/13970265-2342-4f5a-9ceb-1a1ce3e8352e)

## 9.ACCURACY:
![9](https://github.com/DhanalakshmiCSE/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/119477832/5ed5fac3-a6da-40d8-b7b2-ff112cf0ad17)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
