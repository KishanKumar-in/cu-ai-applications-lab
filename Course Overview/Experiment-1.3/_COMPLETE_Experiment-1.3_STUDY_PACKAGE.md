# Experiment-1.3 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-1.3
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

---


## 🖥️ PRESENTATION SLIDES


# Experiment-1.3 - All Lecture Slides Text


## Exp 1.3
### Slide 1
- UNIVERSITY INSTITUTE OF
- ENGINEERING
- DEPARTMENT OF ENGINEERING FOUNDATION-2
- PROGRAM
- NAME
- :
- Bachelor
- of Engineering
- SPECIALIZATION
- :
- COMPUTER SCIENCE & ENGINEERING
- /SEMESTER:IST
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 1                   Experiment No.1.3
- Topic
- :
- Understand supervised learning to train and develop classifier models
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester July-Dec
- 2026

### Slide 2
- Learning
- Objectives
- Understand the core concept of supervised learning
- and differentiate it from other types of learning (unsupervised and reinforcement learning
- ).
- Train
- and develop classification models
- using labeled datasets and evaluate their performance using appropriate metrics (e.g., accuracy, precision, recall
- ).
- Apply
- supervised learning algorithms
- such as Decision Trees, Logistic Regression, and K-Nearest Neighbors to solve
- real-world classification
- problems
- .

### Slide 3
- Recap
- of Previous Experiment
- Exploration:
- Understand the dataset's structure, identify missing values, outliers, and visualize data distributions to detect patterns.
- Transformation:
- Clean and convert the data by handling missing values, encoding categorical variables, and scaling numerical features for model compatibility.
- Summarization:
- Aggregate and visualize key insights from the dataset to support feature selection and improve classification model performance.

### Slide 4
- Topic 1 : Introduction
- to Supervised Learning and Classification
- Topic 2: Training
- Classifier Models Using Labeled Data
- Topic 3 :Evaluating Classification
- Performance
- Figure-1 : Supervised Machine Learning
- Source:
- https
- ://encord.com/blog/mastering-supervised-learning-a-comprehensive-guide/
- Understand supervised learning to train and develop classifier models.

### Slide 5
- Introduction to Supervised Learning
- Definition:
- Supervised learning is a machine learning paradigm where a model learns from labeled data to make predictions.
- Key Characteristics:
- Requires labeled datasets (input-output pairs).
- Goal:
- Minimize the difference between predicted and actual outputs.
- Applications:
- Spam detection, image recognition, and medical diagnosis.
- Additional/Recommended Readings
- https://www.geeksforgeeks.org/supervised-machine-learning/
- Figure-2 : Supervised Machine Learning
- Source:
- https
- ://databasetown.com/supervised-learning-algorithms/

### Slide 6
- Types of Supervised ML
- Classification:
- Predicting categorical labels (e.g., spam or not spam).
- Regression:
- Predicting continuous values (e.g., house prices).
- Examples:
- Classification: Email spam detection.
- Regression: Predicting stock prices.
- Additional/Recommended Readings
- https://www.datacamp.com/blog/supervised-machine-learning
- Figure-3 : Types of Supervised Machine Learning
- Source:
- https://www.geeksforgeeks.org/supervised-machine-learning/

### Slide 7
- What is Classification?
- Classification is
- defined as
- the
- process of recognition, understanding,
- and
- grouping
- of objects
- and ideas
- into present
- Categories
- .
- Figure-4 : Classification in ML
- Source:
- https
- ://www.analytixlabs.co.in/blog/classification-in-machine-learning/

### Slide 8
- Additional / Recommended Readings
- :
- https://www.geeksforgeeks.org/getting-started-with-classification/
- Figure-5: Classification ML Types
- Source:
- https
- ://www.datacamp.com/blog/classification-machine-learning
- Classification ML Types

### Slide 9
- Figure-6:
- Steps in Building a Classifier Model
- Source:
- https
- ://www.techguruspeaks.com/classification-technique/
- Steps in Building a Classifier Model
- Dataset Preparation
- Exploratory Data Analysis (EDA)
- Data Pre-processing
- Model Selection
- Model Training
- Evaluation

### Slide 10
- Figure-7: The most popular classification algorithms
- Source:
- https
- ://serokell.io/blog/classification-algorithms
- Classification Algorithms

### Slide 11
- Confusion
- matrix
- is a simple table used to measure how well a classification model is performing. It compares the predictions made by the model with the actual results and shows where the model was right or wrong. This helps you understand where the model is making mistakes so you can improve it. It breaks down the predictions into four categories:
- True Positive (TP):
- The model correctly predicted a positive outcome
- i.e.
- the actual outcome was positive.
- True Negative (TN):
- The model correctly predicted a negative outcome
- i.e.
- the actual outcome was negative.
- False Positive (FP):
- The model incorrectly predicted a positive outcome
- i.e.
- the actual outcome was negative. It is also known as a Type I error.
- False Negative (FN):
- The model incorrectly predicted a negative outcome
- i.e.
- the actual outcome was positive. It is also known as a Type II error.
- Figure-8: Confusion Matrix
- Source:
- https
- ://www.geeksforgeeks.org/confusion-matrix-machine-learning/
- Confusion
- Matrix in Machine Learning

### Slide 12
- Figure-9:
- Confusion Matrix
- Source:
- https
- ://encord.com/glossary/confusion-matrix/
- Model Evaluation
- Evaluate model performance using metrics: Accuracy, Precision, Recall, F1-Score,
- Specificity.

### Slide 13
- Summary of the
- Experiment
- Learn the concept of supervised learning
- and how it uses labeled data to train classification models
- .
- Apply algorithms like Logistic Regression, Decision Trees, and K-NN
- to build and train classifier models
- .
- Evaluate model performance
- using metrics such as accuracy, precision, recall, and confusion matrix.

### Slide 14
- Next
- Experiment
- T
- opic(s)
- Overview
- of Classification and Machine Learning
- Algorithms
- Building
- and Training Classification
- Models
- Evaluating
- and Comparing Model Performance

### Slide 15
- Quiz/ FAQ’s
- What is the difference between supervised and unsupervised machine learning?
- How will you determine the Machine Learning algorithm that is suitable for your problem?
- What is supervised learning, and how does it differ from unsupervised learning?
- Why is data preprocessing important before training a classifier model?
- What are some common evaluation metrics for classification models, and when would you use them?

### Slide 16
- R
- eferences/ Articles/ Videos
- Reference/Articles
- Scikit
- -Learn Documentation – Supervised Learning
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId3"/></a:rPr><a:t>https://scikit-learn.org/stable/supervised_learning.html
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>– Official documentation for implementing and understanding supervised classifiers.
- Google Developers – Machine Learning Crash Course
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://developers.google.com/machine-learning/crash-course
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>– Offers interactive explanations and labs for classification model building.
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0" smtClean="0"/></a:br><a:r><a:rPr lang="en-US" sz="2800" dirty="0" smtClean="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/></a:rPr><a:t>Videos
- Machine Learning in Python: Building a
- Classification Model
- https
- ://youtu.be/XmSlFPDjKdc?si=_
- quEviyM23MtMZlf
- Machine Learning
- Algorithms
- -
- https
- ://youtu.be/E0Hmnixke2g?si=mqbAqFlFbzXc6AhP

### Slide 17
- Additional
- learning
- R
- esources
- https
- ://
- openclassrooms.com/en/courses/6389626-train-a-supervised-machine-learning-model/6405911-build-and-evaluate-a-classification-model
- https
- ://
- www.datacamp.com/blog/classification-machine-learning
- https
- ://www.geeksforgeeks.org/basic-concept-classification-data-mining/

### Slide 18
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 19
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in


---
