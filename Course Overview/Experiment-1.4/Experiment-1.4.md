# Experiment-1.4

## Build a classification model by using different machine learning algorithms.

##      CO3

Objective : To build and compare classification models using various machine learning algorithms such as decision tree, random forest, k-nearest neighbors, logistic regression, and support vector machine in order to analyze their performance on a given dataset and identify the most suitable model for accurate prediction.

Tools/Platforms Used: Google Colaboratory

Theory: Classification is a supervised machine learning task where the goal is to predict the category or class of a given data point based on input features. Various machine learning algorithms can be used to build classification models, each with its strengths and weaknesses. Below is a brief overview of key concepts and algorithms used in classification:

Key Concepts in Classification

- Training and Testing Data:

- The dataset is split into training and testing sets to evaluate the model's performance on unseen data.

- Features and Target Variable:

- Features are the input variables (independent variables), and the target variable (dependent variable) is the class to be predicted.

- Evaluation Metrics:

- Accuracy, precision, recall, F1-score, confusion matrix, ROC-AUC, etc., are used to assess model performance.

- Pre-processing:

- Data must be cleaned, normalized, and encoded (for categorical features) before training.

Popular Machine Learning Algorithms for Classification

1. Logistic Regression: Suitable for binary classification tasks; uses a logistic function to model the probability of a class.

2.  Decision Tree: Splits data based on feature values; provides interpretable results but can overfit on small datasets.

3. Random Forest: An ensemble of decision trees; reduces overfitting and improves generalization.

4. Support Vector Machine (SVM): Finds the optimal hyperplane to separate classes; works well with small datasets and high-dimensional spaces.

5. K-Nearest Neighbors (KNN): Classifies based on the majority vote of nearest neighbors; simple but computationally expensive for large datasets.

6. Naive Bayes: Based on Bayes' Theorem; works well with categorical data and text classification.

## Codes

## Code 1: Installation of Required Libraries

This code installs the Python libraries required for data handling, machine learning, visualization, and model evaluation.

!pip install -q pandas numpy scikit-learn matplotlib seaborn

## Code 2: Importing Classification Algorithms

This code imports all supervised classification algorithms that will be compared in the experiment.

import pandas as pd

import numpy as np

import time

from sklearn.model_selection import StratifiedKFold

from sklearn.model_selection import cross_validate

from sklearn.preprocessing import StandardScaler

from sklearn.metrics import make_scorer

from sklearn.metrics import cohen_kappa_score

from sklearn.metrics import matthews_corrcoef

# Classification Algorithms

from sklearn.naive_bayes import GaussianNB

from sklearn.linear_model import LogisticRegression

from sklearn.linear_model import RidgeClassifier

from sklearn.tree import DecisionTreeClassifier

from sklearn.neighbors import KNeighborsClassifier

from sklearn.svm import SVC

from sklearn.ensemble import RandomForestClassifier

from sklearn.ensemble import ExtraTreesClassifier

from sklearn.ensemble import GradientBoostingClassifier

from sklearn.ensemble import AdaBoostClassifier

from sklearn.discriminant_analysis import LinearDiscriminantAnalysis

from sklearn.discriminant_analysis import QuadraticDiscriminantAnalysis

from sklearn.dummy import DummyClassifier

## Code 3: Loading the Dataset

This code loads the heart disease dataset from the heart.csv file into a Pandas DataFrame.

df = pd.read_csv("heart.csv")

print("First Five Records")

display(df.head())

print("\nDataset Shape")

print(df.shape)

print("\nDataset Information")

print(df.info())

print("\nMissing Values")

print(df.isnull().sum())

## Code 4: Separating Features and Target Variable

This code separates the independent input features into X and the output target variable into y.

X = df.drop("target",axis=1)

y = df["target"]

## Code 5: Feature Scaling

This code standardizes all input features so that they have approximately a mean of 0 and a standard deviation of 1.

scaler = StandardScaler()

X = scaler.fit_transform(X)

## Code 6: Creating Stratified Cross-Validation

This code creates a 10-fold stratified cross-validation procedure. Stratification maintains approximately the same class proportion in every fold.

cv = StratifiedKFold(

n_splits=10,

shuffle=True,

random_state=42

)

## Code 7: Creating the Machine Learning Models

This code stores all classification algorithms inside a Python dictionary. Each model has a name and its corresponding classifier object.

models = {

"Naive Bayes":GaussianNB(),

"Logistic Regression":LogisticRegression(max_iter=1000),

"Ridge Classifier":RidgeClassifier(),

"Decision Tree":DecisionTreeClassifier(random_state=42),

"K Nearest Neighbor":KNeighborsClassifier(),

"SVM":SVC(probability=True),

"Random Forest":RandomForestClassifier(random_state=42),

"Extra Trees":ExtraTreesClassifier(random_state=42),

"Gradient Boosting":GradientBoostingClassifier(random_state=42),

"AdaBoost":AdaBoostClassifier(random_state=42),

"Linear Discriminant Analysis":LinearDiscriminantAnalysis(),

"Quadratic Discriminant Analysis":QuadraticDiscriminantAnalysis(),

"Dummy Classifier":DummyClassifier(strategy="most_frequent")

}

## Code 8: Defining Evaluation Metrics

This code defines the metrics used to compare the classification models. It includes Accuracy, AUC, Recall, Precision, F1 Score, Kappa, and MCC.

scoring = {

"Accuracy": "accuracy",

"AUC": "roc_auc",

"Recall": "recall",

"Precision": "precision",

"F1": "f1",

"Kappa": make_scorer(cohen_kappa_score),

"MCC": make_scorer(matthews_corrcoef)

}

## Code 9: Comparing All Models

This code trains and evaluates every model using 10-fold cross-validation. It calculates the average value of each performance metric and records the total execution time.

results=[]

for name,model in models.items():

start=time.time()

scores=cross_validate(

model,

X,

y,

cv=cv,

scoring=scoring,

error_score="raise"

)

end=time.time()

results.append({

"Model":name,

"Accuracy":scores["test_Accuracy"].mean(),

"AUC":scores["test_AUC"].mean(),

"Recall":scores["test_Recall"].mean(),

"Precision":scores["test_Precision"].mean(),

"F1 Score":scores["test_F1"].mean(),

"Kappa":scores["test_Kappa"].mean(),

"MCC":scores["test_MCC"].mean(),

"TT (Sec)":end-start

})

## Code 10: Displaying the Model Comparison

This code displays the final comparison table containing the performance of all classification algorithms.

comparison=pd.DataFrame(results)

comparison=comparison.sort_values(

by="Accuracy",

ascending=False

)

comparison.reset_index(drop=True,inplace=True)

comparison=comparison.round(4)

print("\nModel Comparison")

display(comparison)

## Video Links

Classification In Machine Learning

Top 6 Machine Learning Algorithms for Beginners | Classification

How to build a classification model by using different machine learning algorithms

PyCaret Tutorial: Creating Model for the Classification Task

## Practice Task Questions

- Write a Python program to load a classification dataset using Pandas.

- Write a Python program to preprocess the dataset before applying machine learning algorithms.

- Write a Python program to divide the dataset into input features and target output.

- Write a Python program to split the dataset into training and testing data.

- Write a Python program to build a classification model using Logistic Regression.

- Write a Python program to build a classification model using Decision Tree algorithm.

- Write a Python program to build a classification model using Random Forest algorithm.

- Write a Python program to build a classification model using K-Nearest Neighbors algorithm.

- Write a Python program to evaluate different classification models using accuracy score, confusion matrix, precision, recall, and F1-score.

- Write a Python program to compare the performance of different machine learning classification algorithms and identify the best model.

## Additional Resources

- Openclass Room Tutorials: https://openclassrooms.com/en/courses/6389626-train-a-supervised-machine-learning-model/6405911-build-and-evaluate-a-classification-model

- Datacamp Tutorial: https://www.datacamp.com/blog/classification-machine-learning

- GeeksforGeeks - https://www.geeksforgeeks.org/basic-concept-classification-data-mining/

## TEXT BOOKS/REFERENCE BOOKS

## TEXT BOOKS

T1: Data Science from Scratch, Joel Grus, Shroff Publisher Publisher /O’Reilly Publisher Media, 2019.

https://drive.google.com/file/d/1qv89LVaEshX9hcmSS9KDMsvBP-UYC78h/view?usp=sharing

T2: Artificial Intelligence: A Modern Approach, 3rd Edition, by Stuart Russell and Peter Norvig, Pearson Publisher, 2010.

https://drive.google.com/file/d/1G-s5fsBh5rLMdWmIYvyeI2zclcDCAA_D/view?usp=sharing

T3: Machine Learning, Tom Mitchell, McGraw Hill, 2017.

https://drive.google.com/file/d/1IBgLq2GvyEXURAPfSDm-Eep94X0vYXDb/view?usp=sharing

## REFERENCE BOOKS

RB1: Philipp Janert, Data Analysis with Open-Source Tools, Shroff Publisher Publisher /O’Reilly Publisher Media.

https://drive.google.com/file/d/1SVtjE5XEih7_aU433_cAJKiDF41-KuzU/view?usp=sharing

RB2: Andreas C. Müller & Sarah Guido ,Introduction to Machine Learning with Python,published by O'Reilly Media

https://www.nrigroupindia.com/e-book/Introduction%20to%20Machine%20Learning%20with%20Python%20(%20PDFDrive.com%20)-min.pdf

RB3: Ms.Anitha Patibandla, Dr.B.Jyothi, Ms.K.Bhavana,ARTIFICIAL INTELLIGENCE & MACHINE LEARNING,Lecture notes

https://mrcet.com/downloads/digital_notes/ECE/III%20Year/AI%20&%20ML%20DIGITAL%20NOTES.pdf