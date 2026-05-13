# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import the required libraries and create the dataset containing employee levels and salaries.

2.Separate the input feature (Level) and output value (Salary) from the dataset.

3.Create and train the Decision Tree Regressor model using the training data.

4.Predict the salary values using the trained regression model for existing and new employee levels.

5.Display the predicted results and plot the graph showing actual salaries and decision tree regression predictions

## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: mohammed salman.j
RegisterNumber:212225040250
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.model_selection import train_test_split
from sklearn.tree import DecisionTreeRegressor, plot_tree
data = pd.read_csv("Salary (1).csv")
X = data.drop("Salary", axis=1)
y = data["Salary"]
X = pd.get_dummies(X, drop_first=True)
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.2, random_state=42)
model = DecisionTreeRegressor(random_state=42)
model.fit(X_train, y_train)
plt.figure(figsize=(25,12))
plot_tree(
    model,
    feature_names=X.columns,
    filled=True
)

plt.title("Decision Tree Regressor")
plt.show()  
*/
```

## Output:
<img width="1183" height="518" alt="WhatsApp Image 2026-05-13 at 9 21 20 AM" src="https://github.com/user-attachments/assets/0d0c3e8f-70cc-4868-bed4-5b51b541e237" />


## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
