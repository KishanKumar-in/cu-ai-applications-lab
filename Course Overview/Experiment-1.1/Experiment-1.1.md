# Experiment-1.1

##

## Introduction to Data Pre-processing, Pandas, NumPy & Matplotlib for Data Analysis.

##      CO1, CO2

## Objective:

To understand and apply data pre-processing techniques using Python libraries such as NumPy , Pandas and Matplotlib, which are essential for preparing datasets for machine learning models.

## Tool/Platform Used:

Google Colaboratory

## Theory:

Data Pre-Processing

Data pre-processing is a critical step in preparing raw data for analysis and model building. The goal is to clean, transform, and organize data into a format suitable for AI/ML algorithms. Proper preprocessing ensures that the data is consistent, relevant, and free from biases or inaccuracies that might negatively impact the model's performance. The process of data preprocessing is shown in Figure 1 below.

Figure 1. Data Pre-processing process

Data Pre-processing Packages

Data pre-processing is a crucial step in any AI/ML pipeline. It involves cleaning, transforming, and preparing data for analysis and modeling. The two important data preprocessing packages are shown in Figure 2 below.

a. NumPy

- Purpose: Numerical computations and array operations.

- Features:

- Provides high-performance multidimensional arrays (numpy.ndarray).

- Supports operations like slicing, masking, reshaping, and statistical functions.

- Use Case: Efficient for handling large numerical datasets.

b. Pandas

- Purpose: Data manipulation and analysis.

- Features:

- Data structures: DataFrame and Series.

- Tools for handling missing data, filtering rows/columns, and grouping datasets.

- Supports reading/writing data from multiple formats like CSV, Excel, SQL, etc.

- Use Case: Cleaning messy datasets, managing missing values, and reshaping.

Figure 2: Python Libraries for Data Manipulation and Analysis

Relevance to AIML Algorithms

Clean and well-structured data is essential for training accurate machine learning models. Pre-processing ensures:

- Data quality and consistency

- Reduced training time

- Improved model performance

Introduction to Data Analysis and Visualization

Data analysis and visualization are fundamental steps in the workflow of Artificial Intelligence (AI) and Machine Learning (ML) algorithms. These steps ensure that data is properly understood, preprocessed, and visualized before applying AIML models. Matplotlib, a Python library, plays a significant role in visualizing patterns, relationships, and trends in the data, enabling decision-making and model optimization, as shown in Figure 3 below.

Figure 3: Matplotlib: Visualization with Python

Importance of Data Analysis and Visualization

- Data Understanding: Before applying AIML algorithms, understanding the dataset's structure (size, type, and values) is crucial.

- Feature Engineering: Identifying trends, relationships, and outliers helps prepare the data and design better features for training models.

- Model Explanation: Visualizing the results of models (e.g., regression lines, decision boundaries) helps explain model predictions.

- Performance Metrics: Visualization assists in evaluating the performance of models (e.g., accuracy curves, confusion matrices).

Role of AIML Algorithms in Data Analysis

- AI and ML Algorithms analyze large volumes of data, uncover hidden patterns, and predict outcomes.

- Supervised Learning: Algorithms like Linear Regression, Decision Trees, and Support Vector Machines rely on analyzing historical data to predict outcomes.

- Unsupervised Learning: Clustering algorithms (e.g., K-means) analyze and group similar data points.

- Deep Learning: Neural networks analyze high-dimensional and complex data for pattern recognition.

- Data visualization serves as a pre-processing and post-analysis tool to validate the assumptions of AIML models and visualize results.

Matplotlib for Data Visualization

Matplotlib is a Python library that provides tools for creating static, animated, and interactive visualizations. It is widely used for representing data analysis results in graphical form.

Key Features of Matplotlib:

- Simple to Use: Create visualizations with minimal coding.

- Wide Range of Plots: Supports line plots, scatter plots, bar charts, histograms, pie charts, etc.

- Customization: Offers control over colors, labels, legends, and other elements.

- Integration: Works seamlessly with Pandas, NumPy, and other data analysis libraries.

## Codes

## Basic Python Fundamentals

## Code 1 ( Printing )

print ("Hello World !!")

Output:-

Hello World !!

## Code 2 ( Arithmatic Operations)

# Define variables

a = 220

b = 16

# Perform arithmetic operations

addition = a + b

subtraction = a - b

multiplication = a * b

division = a / b  # Floating-point division

floor_division = a // b  # Integer division

modulus = a % b

exponentiation = a ** b

# Display results

print("Addition:", addition)

print("Subtraction:", subtraction)

print("Multiplication:", multiplication)

print("Division (float):", division)

print("Floor Division (integer):", floor_division)

print("Modulus (remainder):", modulus)

print("Exponentiation:", exponentiation)

Output:-

Addition: 236

Subtraction: 204

Multiplication: 3520

Division (float): 13.75

Floor Division (integer): 13

Modulus (remainder): 12

Exponentiation: 115792089237316195423570985008687907853269984665640564039457584007913129639936

## Code 3 :-Variables and Data Types

name = "Alice"

age = 20

height = 5.4

print("Name:", name)

print("Age:", age)

print("Height:", height)

Output:-

Name: Alice

Age: 20

Height: 5.4

## Pandas Codes for Data Analysis

## Code 1:-Simple Pandas DataFrame

import pandas as pd

data = {

'Name': ['Alice', 'Bob', 'Charlie', 'David', 'Eva'],

'Age': [25, 30, 35, 40, 28],

'Score': [88, 92, 95, 70, 85],

'City': ['Delhi', 'Mumbai', 'Delhi', 'Bangalore', 'Mumbai']

}

df = pd.DataFrame(data)

print(df)

Output:-

## Code 2: Display DataFrame Info

print(df.info())

Output:-

## Code 3:-Summary Statistics

print(df.describe())

Output:-

## NumPy Codes for Data Analysis

## Code 1:- Creating Arrays

import numpy as np

array = np.array([1, 2, 3, 4, 5])

print("Array:", array)

Output:-

Array: [1 2 3 4 5]

## Code 2:- Basic Statistical Analysis

import numpy as np

data = np.array([1, 2, 3, 4, 5])

print("Mean:", np.mean(data))

print("Median:", np.median(data))

print("Standard Deviation:", np.std(data))

Output:-

Mean: 3.0

Median: 3.0

Standard Deviation: 1.4142135623730951

## Code 3:- Correlation Coefficient

import numpy as np

x = np.array([1, 2, 3])

y = np.array([10, 20, 30])

correlation = np.corrcoef(x, y)

print("Correlation Coefficient:\n", correlation)

Output:-

Correlation Coefficient:

[[1. 1.]

[1. 1.]]

## Matplotlib Codes for Data Visualization

## Code 1:- Matplotlib Adding Grid Lines

import numpy as np

import matplotlib.pyplot as plt

x = np.array([80, 85, 90, 95, 100, 105, 110, 115, 120, 125])

y = np.array([240, 250, 260, 270, 280, 290, 300, 310, 320, 330])

plt.title("Sports Watch Data")

plt.xlabel("Average Pulse")

plt.ylabel("Calorie Burnage")

plt.plot(x, y)

plt.grid()

plt.show()

Output:-

## Code 2:- Matplotlib Bars

import matplotlib.pyplot as plt

import numpy as np

categories = ['A', 'B', 'C', 'D']

values1 = [4, 7, 1, 8]  # Data for Group 1

values2 = [5, 3, 6, 9]  # Data for Group 2

values3 = [6, 8, 5, 7]  # Data for Group 3

# Define the position of bars on the X-axis

x = np.arange(len(categories))

# Bar width

bar_width = 0.25

# Create bars for each group

plt.bar(x - bar_width, values1, width=bar_width, label='Group 1', color='blue')

plt.bar(x, values2, width=bar_width, label='Group 2', color='orange')

plt.bar(x + bar_width, values3, width=bar_width, label='Group 3', color='green')

# Add labels and title

plt.xlabel('Categories')

plt.ylabel('Values')

plt.title('Multiple Bar Chart Example')

plt.xticks(x, categories)  # Set the labels for the X-axis

plt.legend()  # Add legend

# Display the plot

plt.tight_layout()

plt.show()

Output:-

## Code 3:- Matplotlib Pie Chart

import matplotlib.pyplot as plt

import numpy as np

y = np.array([35, 25, 25, 15])

mylabels = ["Apples", "Bananas", "Cherries", "Dates"]

plt.pie(y, labels = mylabels)

plt.legend()

plt.show()

Output:-

Video links

Introduction to Google Colab

Python Basics for Beginners

Data Preprocessing in Machine learning

Python Tutorial: What is data preprocessing?

NumPy vs Pandas

Data Analysis with Python Numpy & Pandas

Matplotlib Tutorial

Data Visualization with Python Matplotlib

Exploring Types of Plot with Matplotlib

## Practice Task Questions

- Write a Python program to create and display a Pandas DataFrame.

- Write a Python program to load a CSV file using Pandas and display the first five records.

- Write a Python program to identify and handle missing values in a dataset.

- Write a Python program to perform basic statistical analysis using NumPy.

- Write a Python program to clean a dataset by removing duplicate records.

- Write a Python program to filter records from a dataset based on a given condition.

- Write a Python program to sort a dataset based on a selected column.

- Write a Python program to add a new calculated column in a Pandas DataFrame.

- Write a Python program to visualize student marks using Matplotlib.

- Write a Python program to create different plots such as bar chart, line chart, pie chart, and histogram using Matplotlib.

## Additional Resources for Learning Basics of python

- Kaggle Tutorials: https://www.kaggle.com/learn/python

- W3Schools Tutorial: https://www.w3schools.com/python/default.asp

- GeeksforGeeks - https://www.geeksforgeeks.org/python-programming-language-tutorial/

Additional Resources for Learning Pandas and NumPy

Kaggle Tutorials: Hands-on tutorials on Pandas and NumPy designed for data science beginners. Check them out.https://www.kaggle.com/code/chats351/introduction-to-numpy-pandas-and-matplotlibW3Schools Pandas Tutorial: A beginner-friendly guide to Pandas and Numpy covering essential concepts. Learn here.https://www.w3schools.com/python/default.aspGeeksforGeeks - NumPy and Pandas Guide: Easy-to-follow tutorials and exercises for NumPy and Pandas. Start here.https://www.geeksforgeeks.org/pandas-tutorial/

##

## Additional Resources for Learning Basics of Matplotlib

##

- Kaggle Tutorials: https://www.kaggle.com/code/prashant111/matplotlib-tutorial-for-beginners

- W3Schools Tutorial: https://www.w3schools.com/python/matplotlib_intro.asp

- GeeksforGeeks: https://www.geeksforgeeks.org/matplotlib-tutorial/

## TEXT BOOKS/REFERENCE BOOKS

## Text Books

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