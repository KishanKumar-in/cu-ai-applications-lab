# Experiment-1.3

## Understand supervised learning to train and develop classifier models.

##      CO3

##

## Objective: To understand the principles of supervised learning and apply various classification algorithms to train models on labeled datasets, enabling the prediction of categorical outcomes with evaluation of model performance using appropriate metrics.

Tools/Platforms Used: Google Colaboratory

Theory:

Supervised Learning: Supervised learning is a type of machine learning where the model learns from labeled data. In this approach, the dataset provided to the model contains input features (independent variables) and corresponding target labels (dependent variables). The model learns the relationship between the inputs and the outputs to make predictions on new, unseen data. The workflow of supervised learning-based classification model development is shown in the figure 1 below.

Figure 1: Workflow of Supervised Learning-Based Classification Model Development

Key Concepts in Supervised Learning:

- Features and Labels:

- Features (X): Independent variables that act as input to the model.

- Labels (Y): Dependent variables or the output the model needs to predict.

- Training and Testing:

- Training Data: The subset of the dataset used to train the model.

- Testing Data: The subset used to evaluate the model's performance.

- The dataset is typically split into 70–80% training data and 20–30% testing data.

- Objective:

The goal is to minimize the error between the predicted and actual outputs and to generalize well to unseen data.

Classification in Supervised Learning:

Classification is a supervised learning task where the output variable is categorical. Examples include:

- Binary Classification: Predicting one of two categories (e.g., spam or not spam).

- Multi-class Classification: Predicting one of multiple categories (e.g., types of fruits).

Steps to Train and Develop Classifier Models:

- Data Preprocessing:

- Clean the data (handle missing values, outliers).

- Encode categorical variables.

- Normalize or standardize numerical features.

- Feature Selection and Engineering:

- Select relevant features to improve model performance.

- Create new features from existing ones if necessary.

- Model Selection:

- Choose an appropriate classification algorithm, such as:

- Logistic Regression

- Decision Trees

- Random Forest

- Support Vector Machines (SVM)

- Neural Networks

- Training:

- Fit the selected algorithm to the training dataset using fit().

- Evaluation:

- Use metrics like accuracy, precision, recall, F1-score, and ROC-AUC to assess the model’s performance.

- Hyperparameter Tuning:

- Optimize the model's performance by adjusting hyperparameters using techniques like grid search or random search.

Common Use Cases of Classification Models:

- Email spam detection.

- Fraud detection in financial systems.

- Disease diagnosis in healthcare.

- Sentiment analysis of customer reviews.

## The coding examples to implement these concepts practically:

## Codes

## Code 1: Installation of Required Libraries

## !pip install -q pandas numpy matplotlib seaborn scikit-learn

## # This code installs the essential Python libraries required for data analysis, visualization, and machine learning.

## Code 2: Importing Required Libraries

import pandas as pd

import numpy as np

import matplotlib.pyplot as plt

import seaborn as sns

from sklearn.model_selection import train_test_split

from sklearn.model_selection import StratifiedKFold

from sklearn.model_selection import cross_val_score

from sklearn.preprocessing import StandardScaler

from sklearn.naive_bayes import GaussianNB

from sklearn.metrics import accuracy_score

from sklearn.metrics import confusion_matrix

from sklearn.metrics import matthews_corrcoef

from sklearn.metrics import precision_score

from sklearn.metrics import recall_score

from sklearn.metrics import f1_score

from sklearn.metrics import roc_auc_score

from sklearn.metrics import cohen_kappa_score

from sklearn.metrics import roc_curve

# This code imports the necessary libraries and functions for data processing, visualization, model training, cross-validation, and performance evaluation.

## Code 3: Loading the Heart Disease Dataset

df = pd.read_csv("heart.csv")

df.head()

# This code loads the heart disease dataset from a CSV file into a Pandas DataFrame named df.

## Code 4: Checking Dataset Information

df.info()

# This code displays basic information about the dataset, including the number of rows and columns, column names, data types, and missing values.

## Code 5: Displaying Statistical Summary of Dataset

df.describe()

# This code provides descriptive statistics such as count, mean, standard deviation, minimum, maximum, and quartile values for numerical columns.

## Code 6: Separating Features and Target Variable

X = df.drop("target", axis=1)

y = df["target"]

# This code separates the independent variables into X and the target variable into y. The target column represents the output that the machine learning model will predict.

## Code 7: Splitting Dataset into Training and Testing Data

X_train, X_test, y_train, y_test = train_test_split(

X,

y,

test_size=0.20,

random_state=42,

stratify=y

)

print("Original Dataset Shape:", X.shape)

print("Training Feature Shape:", X_train.shape)

print("Testing Feature Shape:", X_test.shape)

print()

print("Original Target Shape:", y.shape)

print("Training Target Shape:", y_train.shape)

print("Testing Target Shape: ", y_test.shape)

# This code divides the dataset into 80% training data and 20% testing data. Stratification maintains approximately the same class distribution in both sets.

##

## Code 8: Feature Scaling Using StandardScaler

This code standardizes the numerical features so that they have approximately a mean of 0 and a standard deviation of 1.

scaler = StandardScaler()

X_train = scaler.fit_transform(X_train)

X_test = scaler.transform(X_test)

## Code 9: Creating Gaussian Naive Bayes Model

This code creates an instance of the Gaussian Naive Bayes classifier, which will be used for classification.

model = GaussianNB()

## Code 10: Applying Stratified K-Fold Cross-Validation

This code applies 10-fold stratified cross-validation to evaluate the model more reliably. The training data is divided into 10 folds while maintaining class proportions.

cv = StratifiedKFold(

n_splits=10,

shuffle=True,

random_state=42

)

cv_scores = cross_val_score(

model,

X_train,

y_train,

cv=cv,

scoring='accuracy'

)

print("Cross Validation Accuracy")

print(cv_scores)

print("Mean Accuracy :", cv_scores.mean())

print("Standard Deviation :", cv_scores.std())

## Code 11: Training the Gaussian Naive Bayes Model

This code trains the Gaussian Naive Bayes model using the complete training dataset.

model.fit(X_train, y_train)

## Code 12: Predicting Test Data Output

This code predicts the class labels and probabilities for the unseen test data.

y_pred = model.predict(X_test)

y_prob = model.predict_proba(X_test)[:, 1]

## Code 13: Comparing Actual and Predicted Values

This code creates a DataFrame to compare the actual test values with the values predicted by the model.

comparison = pd.DataFrame({

"Actual": y_test,

"Predicted": y_pred

})

print(comparison)

## Code 14: Displaying Prediction Probability and Correct Status

This code displays the actual class, predicted class, prediction probability, and whether each prediction is correct or incorrect.

comparison = pd.DataFrame({

"Actual": y_test,

"Predicted": y_pred,

"Probability": y_prob

})

comparison["Correct"] = comparison["Actual"] == comparison["Predicted"]

print(comparison.head(20))

## Code 15: Generating Confusion Matrix

This code generates a confusion matrix to summarize correct and incorrect predictions made by the classification model.

cm = confusion_matrix(y_test, y_pred)

plt.figure(figsize=(6,5))

sns.heatmap(

cm,

annot=True,

cmap="Blues"

)

plt.xlabel("Predicted")

plt.ylabel("Actual")

plt.title("Confusion Matrix")

plt.show()

##

## Code 16: Calculating Model Performance Metrics

This code calculates various classification performance metrics, including Accuracy, Kappa, Precision, Recall, F1 Score, ROC-AUC, and MCC.

accuracy = accuracy_score(y_test, y_pred)

kappa = cohen_kappa_score(y_test, y_pred)

precision = precision_score(y_test, y_pred)

recall = recall_score(y_test, y_pred)

f1 = f1_score(y_test, y_pred)

auc = roc_auc_score(y_test, y_prob)

mcc = matthews_corrcoef(y_test, y_pred)

results = pd.DataFrame({

"Metric": [

"Accuracy",

"Kappa",

"Precision",

"Recall",

"F1 Score",

"ROC-AUC",

"MCC"

],

"Value": [

accuracy,

kappa,

precision,

recall,

f1,

auc,

mcc

]

})

print(results)

## Code 17: Calculating ROC Curve Values

This code calculates the False Positive Rate (FPR) and True Positive Rate (TPR) at different classification thresholds for plotting the ROC curve.

fpr, tpr, threshold = roc_curve(y_test, y_prob)

plt.figure(figsize=(6,5))

plt.plot(fpr, tpr, label="ROC Curve")

plt.plot([0,1], [0,1], "--")

plt.xlabel("False Positive Rate")

plt.ylabel("True Positive Rate")

plt.title("ROC Curve")

plt.legend()

plt.show()

##

## Video Links

Machine Learning in Python: Building a ClassificationModel

Random Forest Algorithm Explained with Python

Machine Learning Algorithms

PyCaret Tutorial: Splitting Data into Training and TestingSets

## Practical Task Questions

- Write a Python program to load a classification dataset using Pandas.

- Write a Python program to separate input features and target class from a dataset.

- Write a Python program to split a dataset into training and testing sets.

- Write a Python program to train a classifier model using supervised learning.

- Write a Python program to develop a Decision Tree classifier model.

- Write a Python program to develop a Logistic Regression classifier model.

- Write a Python program to develop a K-Nearest Neighbors classifier model.

- Write a Python program to predict the class labels for test data using a trained classifier.

- Write a Python program to evaluate a classifier model using accuracy score and confusion matrix.

- Write a Python program to compare the performance of different supervised learning classifier models.

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