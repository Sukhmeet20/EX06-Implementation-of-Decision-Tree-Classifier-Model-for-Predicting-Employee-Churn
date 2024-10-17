# EX 6 Implementation of Decision Tree Classifier Model for Predicting Employee Churn
## DATE:
## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm

1. Load the Dataset: Use pandas to load the dataset (CSV, Excel, etc.) into a DataFrame.
2. Handle Missing Values: Identify and fill or drop missing values.
3. Encode Categorical Variables: Use label encoding or one-hot encoding for categorical data
(e.g., department, gender).
4. Split the Dataset: Divide the dataset into features (X) and target (y), then split into training and
testing sets.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by: Sukhmeet Kaur G
RegisterNumber: 2305001032
*/
import pandas as pd
from sklearn.tree import DecisionTreeClassifier, plot_tree
from sklearn.preprocessing import LabelEncoder
import matplotlib.pyplot as plt
df=pd.read_csv("/content/Employee_EX6.csv")
data=df.copy()
data
le=LabelEncoder()
data['salary']=le.fit_transform(data['salary'])
data
x=data.drop(['Departments','left'],axis=1)
y=data['left']
clf=DecisionTreeClassifier()
clf.fit(x,y)
plt.figure(figsize=(80,80))
decision tree classifier model
Thus the program to implement the Decision Tree Classifier Model for Predicting Employee Churn is
written and verified using python programming.
plot_tree(clf,feature_names=x.columns,class_names=['LEFT','NOT LEFT'],filled=True)
plt.show()
```

## Output:
![decision tree classifier model](sam.png)
![Screenshot 2024-10-17 113654](https://github.com/user-attachments/assets/c515c1d2-0378-4e41-b657-030006ff394e)
![Screenshot 2024-10-17 113712](https://github.com/user-attachments/assets/876f0ab6-1001-4fbd-9d1d-3105cd864ed4)
![Screenshot 2024-10-17 113729](https://github.com/user-attachments/assets/9d46233f-8a30-4196-add3-d3f15fac6440)
![WhatsApp Image 2024-10-17 at 11 38 38_839e35d9](https://github.com/user-attachments/assets/12f920b2-25c7-4bfc-b82c-d4c94d36f385)

## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
