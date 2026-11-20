# CONT_26ECP-102 __ AI APPLICATIONS LAB - COMPLETE SEMESTER MASTER NOTES

This document contains all lecture notes and slides across all units.

---

# Experiment-1.1 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-1.1
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

---


## 🖥️ PRESENTATION SLIDES


# Experiment-1.1 - All Lecture Slides Text


## Exp 1.1 (a)
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
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (
- SUBJECT
- CODE-26ECP-102
- )
- Unit No. 1                   Experiment No.1.1
- Topic
- : Understanding the Data analysis/Visualization for AIML algorithms using
- Matplotlib
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning Objectives
- To develop the ability to visualize and interpret patterns, relationships, and distributions in data using
- Matplotlib
- .
- To
- apply appropriate types of plots (line, bar, histogram, scatter, etc.) for effective analysis of AIML datasets
- .
- To
- understand how data visualization supports decision-making in selecting and evaluating AIML algorithms.

### Slide 3
- Recap of Previous
- Experiment
- Data Pre-processing:
- Essential for converting messy data into model-ready form
- Pandas and
- NumPy
- :
- Core Python tools for structured and numerical data operations
- AIML Algorithms:
- Enable systems to learn patterns, classify data, and make predictions
- </a:r><a:br><a:rPr lang="en-US" sz="2800" i="0" u="none" strike="noStrike" cap="none" dirty="0" smtClean="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:rPr></a:br><a:endParaRPr lang="en-US" sz="2800" i="0" u="none" strike="noStrike" cap="none" dirty="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:endParaRPr></a:p></p:txBody></p:sp><p:sp><p:nvSpPr><p:cNvPr id="7" name="TextBox 6"/><p:cNvSpPr txBox="1"/><p:nvPr/></p:nvSpPr><p:spPr><a:xfrm><a:off x="8609524" y="85987"/><a:ext cx="284052" cy="307777"/></a:xfrm><a:prstGeom prst="rect"><a:avLst/></a:prstGeom><a:noFill/></p:spPr><p:txBody><a:bodyPr wrap="none" rtlCol="0"><a:spAutoFit/></a:bodyPr><a:lstStyle><a:defPPr marR="0" lvl="0" algn="l" rtl="0"><a:lnSpc><a:spcPct val="100000"/></a:lnSpc><a:spcBef><a:spcPts val="0"/></a:spcBef><a:spcAft><a:spcPts val="0"/></a:spcAft></a:defPPr><a:lvl1pPr marR="0" lvl="0" algn="l" rtl="0"><a:lnSpc><a:spcPct val="100000"/></a:lnSpc><a:spcBef><a:spcPts val="0"/></a:spcBef><a:spcAft><a:spcPts val="0"/></a:spcAft><a:buClr><a:srgbClr val="000000"/></a:buClr><a:buFont typeface="Arial"/><a:defRPr sz="1400" b="0" i="0" u="none" strike="noStrike" cap="none"><a:solidFill><a:srgbClr val="000000"/></a:solidFill><a:latin typeface="Arial"/><a:ea typeface="Arial"/><a:cs typeface="Arial"/><a:sym typeface="Arial"/></a:defRPr></a:lvl1pPr><a:lvl2pPr marR="0" lvl="1" algn="l" rtl="0"><a:lnSpc><a:spcPct val="100000"/></a:lnSpc><a:spcBef><a:spcPts val="0"/></a:spcBef><a:spcAft><a:spcPts val="0"/></a:spcAft><a:buClr><a:srgbClr val="000000"/></a:buClr><a:buFont typeface="Arial"/><a:defRPr sz="1400" b="0" i="0" u="none" strike="noStrike" cap="none"><a:solidFill><a:srgbClr val="000000"/></a:solidFill><a:latin typeface="Arial"/><a:ea typeface="Arial"/><a:cs typeface="Arial"/><a:sym typeface="Arial"/></a:defRPr></a:lvl2pPr><a:lvl3pPr marR="0" lvl="2" algn="l" rtl="0"><a:lnSpc><a:spcPct val="100000"/></a:lnSpc><a:spcBef><a:spcPts val="0"/></a:spcBef><a:spcAft><a:spcPts val="0"/></a:spcAft><a:buClr><a:srgbClr val="000000"/></a:buClr><a:buFont typeface="Arial"/><a:defRPr sz="1400" b="0" i="0" u="none" strike="noStrike" cap="none"><a:solidFill><a:srgbClr val="000000"/></a:solidFill><a:latin typeface="Arial"/><a:ea typeface="Arial"/><a:cs typeface="Arial"/><a:sym typeface="Arial"/></a:defRPr></a:lvl3pPr><a:lvl4pPr marR="0" lvl="3" algn="l" rtl="0"><a:lnSpc><a:spcPct val="100000"/></a:lnSpc><a:spcBef><a:spcPts val="0"/></a:spcBef><a:spcAft><a:spcPts val="0"/></a:spcAft><a:buClr><a:srgbClr val="000000"/></a:buClr><a:buFont typeface="Arial"/><a:defRPr sz="1400" b="0" i="0" u="none" strike="noStrike" cap="none"><a:solidFill><a:srgbClr val="000000"/></a:solidFill><a:latin typeface="Arial"/><a:ea typeface="Arial"/><a:cs typeface="Arial"/><a:sym typeface="Arial"/></a:defRPr></a:lvl4pPr><a:lvl5pPr marR="0" lvl="4" algn="l" rtl="0"><a:lnSpc><a:spcPct val="100000"/></a:lnSpc><a:spcBef><a:spcPts val="0"/></a:spcBef><a:spcAft><a:spcPts val="0"/></a:spcAft><a:buClr><a:srgbClr val="000000"/></a:buClr><a:buFont typeface="Arial"/><a:defRPr sz="1400" b="0" i="0" u="none" strike="noStrike" cap="none"><a:solidFill><a:srgbClr val="000000"/></a:solidFill><a:latin typeface="Arial"/><a:ea typeface="Arial"/><a:cs typeface="Arial"/><a:sym typeface="Arial"/></a:defRPr></a:lvl5pPr><a:lvl6pPr marR="0" lvl="5" algn="l" rtl="0"><a:lnSpc><a:spcPct val="100000"/></a:lnSpc><a:spcBef><a:spcPts val="0"/></a:spcBef><a:spcAft><a:spcPts val="0"/></a:spcAft><a:buClr><a:srgbClr val="000000"/></a:buClr><a:buFont typeface="Arial"/><a:defRPr sz="1400" b="0" i="0" u="none" strike="noStrike" cap="none"><a:solidFill><a:srgbClr val="000000"/></a:solidFill><a:latin typeface="Arial"/><a:ea typeface="Arial"/><a:cs typeface="Arial"/><a:sym typeface="Arial"/></a:defRPr></a:lvl6pPr><a:lvl7pPr marR="0" lvl="6" algn="l" rtl="0"><a:lnSpc><a:spcPct val="100000"/></a:lnSpc><a:spcBef><a:spcPts val="0"/></a:spcBef><a:spcAft><a:spcPts val="0"/></a:spcAft><a:buClr><a:srgbClr val="000000"/></a:buClr><a:buFont typeface="Arial"/><a:defRPr sz="1400" b="0" i="0" u="none" strike="noStrike" cap="none"><a:solidFill><a:srgbClr val="000000"/></a:solidFill><a:latin typeface="Arial"/><a:ea typeface="Arial"/><a:cs typeface="Arial"/><a:sym typeface="Arial"/></a:defRPr></a:lvl7pPr><a:lvl8pPr marR="0" lvl="7" algn="l" rtl="0"><a:lnSpc><a:spcPct val="100000"/></a:lnSpc><a:spcBef><a:spcPts val="0"/></a:spcBef><a:spcAft><a:spcPts val="0"/></a:spcAft><a:buClr><a:srgbClr val="000000"/></a:buClr><a:buFont typeface="Arial"/><a:defRPr sz="1400" b="0" i="0" u="none" strike="noStrike" cap="none"><a:solidFill><a:srgbClr val="000000"/></a:solidFill><a:latin typeface="Arial"/><a:ea typeface="Arial"/><a:cs typeface="Arial"/><a:sym typeface="Arial"/></a:defRPr></a:lvl8pPr><a:lvl9pPr marR="0" lvl="8" algn="l" rtl="0"><a:lnSpc><a:spcPct val="100000"/></a:lnSpc><a:spcBef><a:spcPts val="0"/></a:spcBef><a:spcAft><a:spcPts val="0"/></a:spcAft><a:buClr><a:srgbClr val="000000"/></a:buClr><a:buFont typeface="Arial"/><a:defRPr sz="1400" b="0" i="0" u="none" strike="noStrike" cap="none"><a:solidFill><a:srgbClr val="000000"/></a:solidFill><a:latin typeface="Arial"/><a:ea typeface="Arial"/><a:cs typeface="Arial"/><a:sym typeface="Arial"/></a:defRPr></a:lvl9pPr></a:lstStyle><a:p><a:r><a:rPr lang="en-IN" dirty="0" smtClean="0"/><a:t>2

### Slide 4
- Understanding the Data analysis/Visualization for AIML algorithms using
- Matplotlib
- Topic 1
- . Introduction to Data Visualization
- Topic 2
- . Importance of Data Visualization
- in AIML
- Topic 3
- .
- Basic
- Plot Types Using
- Matplotlib
- Figure-1 : Data Visualization with python
- Source:
- https://www.geeksforgeeks.org/data-visualization-with-python/

### Slide 5
- Introduction to Data Visualization
- Data Visualization refers to the graphical representation of information and data.
- By
- using visual elements like charts, graphs, and maps, data visualization tools make it easier to see trends, outliers, and patterns in data.
- Additional / Recommended Readings:
- https://www.geeksforgeeks.org/data-visualization-with-python/
- Figure-2 : Data Visualization with
- Matplotlib
- Source:
- https
- ://medium.com/@aakash_7/data-visualization-with-matplotlib-d7967ee42fce

### Slide 6
- Why is it important?
- Humans understand visuals faster than text or raw numbers
- .
- It
- simplifies complex datasets, enabling better decision-making
- .
- Helps
- in identifying trends, correlations, and anomalies quickly
- .

### Slide 7
- Importance of Data Visualization in AIML
- Role in AI/ML Workflow
- :
- Pre-processing
- : Detect missing or inconsistent values.
- Feature Analysis
- : Understand feature distributions and relationships.
- Model Selection
- : Visualize performance metrics to choose the best model.
- Post-
- modeling
- : Interpret the results of ML models using plots like confusion matrix, ROC curve, etc.
- Additional / Recommended Readings:
- https://www.tutorialspoint.com/machine_learning/machine_learning_data_visualization.htm
- Figure-3
- : Importance of Data Visualization
- Source:
- https://www.geeksforgeeks.org/data-visualization-and-its-importance/

### Slide 8
- Basic Plot Types Using
- Matplotlib
- Line Plot:
- Used to display trends over
- intervals
- (
- e.g., time-series data).
- plt.plot
- (x, y
- )
- Bar Chart:
- Represents categorical data using rectangular bars.
- plt.bar
- (categories, values)
- Histogram:
- Shows the frequency distribution of a single
- variable
- .
- plt.hist
- (data, bins=10)
- Additional / Recommended Readings
- :
- https://builtin.com/data-science/data-visualization-tutorial
- Figure-4
- : Basic Plot
- Types Using
- Matplotlib
- Source:
- https://www.geeksforgeeks.org/data-visualization-using-matplotlib/

### Slide 9
- Applications of
- Data Visualization
- Business
- dashboards
- Scientific data
- analysis
- Financial market
- analysis
- Health monitoring systems
- Figure-5 : Applications of
- Data Visualization
- Source:
- https
- ://www.analyticssteps.com/blogs/10-applications-data-visualization

### Slide 10
- Summary of the
- Experiment
- Objective:
- To explore the role of data visualization in AIML and learn how to create basic plots using the
- Matplotlib
- library in Python
- .
- Activities
- Performed:
- Implemented line plots, bar charts, histograms, scatter plots, and pie charts to visualize sample data and understand trends, distributions, and relationships
- .
- Outcome
- :
- Gained hands-on experience in visualizing data, improving data interpretation, and enhancing decision-making in machine learning workflows.

### Slide 11
- Next
- Experiment
- T
- opic(s)
- Descriptive Statistics for
- EDA
- Handling Missing and Duplicate
- Data
- Data Visualization Techniques in EDA

### Slide 12
- Quiz/ FAQ’s
- What
- is the difference between plot(), scatter(), and bar() functions in
- Matplotlib
- ?
- How
- do you add a title, labels, and grid lines to a
- Matplotlib
- plot
- ?
- What
- is the purpose of subplot() in
- Matplotlib
- , and how is it used to create multiple plots in one figure?
- How
- does a histogram differ from a bar chart in terms of data representation?
- In
- a pie chart, how can you add custom labels and display a legend using
- Matplotlib
- ?

### Slide 13
- R
- eferences/ Articles/ Videos
- Reference/Articles
- Hunter, J. D. (2007).
- Matplotlib
- : A 2D graphics
- environment. Computing
- in Science & Engineering, 9(3),
- 90–95. This
- foundational paper introduces
- Matplotlib
- and discusses its use in scientific data visualization
- .
- Zhang, Z. et al. (2017).Data visualization in machine learning: A review
- . IEEE
- Access, 6, 41256–41268
- .
- Provides a comprehensive overview of data visualization techniques applied to machine learning tasks.
- Videos
- Data Visualization with Python
- Matplotlib
- https
- ://
- www.youtube.com/watch?v=gvn8RIG38CM
- Exploring Types of Plot with
- Matplotlib
- https
- ://www.youtube.com/watch?v=x0Ga1UG9szU

### Slide 14
- Additional
- learning
- R
- esources
- https://
- www.kaggle.com/code/prashant111/matplotlib-tutorial-for-beginners
- https://
- www.w3schools.com/python/matplotlib_intro.asp
- https://www.geeksforgeeks.org/matplotlib-tutorial/

### Slide 15
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 16
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in


## Exp 1.1
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
- /Semester:
- Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 1                   Experiment No.1.1
- Topic
- :
- Explore
- Data Pre-processing Packages, Pandas, and
- Numpy
- for Data Analysis and AIML A
- lgorithms
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning Objectives
- 1.To Understand
- the role of data pre-processing in preparing raw data for machine learning applications
- .
- 2
- .To Gain
- proficiency in using Pandas for data manipulation tasks such as filtering, grouping, and handling missing values
- .
- 3.To Learn
- to use
- NumPy
- for efficient numerical operations on
- datasets
- and array-based computations.

### Slide 3
- Explore
- Data Pre-processing Packages, Pandas, and
- Numpy
- for Data Analysis and AIML A
- lgorithms
- Topic 1
- . Data Pre-processing
- Topic 2
- . Data Pre-processing
- Packages
- Topic 3
- . AIML algorithms
- Figure-1 : Data Preprocessing
- Source:
- https://www.linkedin.com/pulse/how-preprocess-data-make-machine-learning-ready-using-gauransh-singh/

### Slide 4
- Data
- Pre-Processing
- Data pre-processing is a data mining technique that involves transforming raw data into a clean and usable format
- .
- It
- is the first and crucial step before applying any machine learning model.
- This
- step reduces noise, handles missing values, and standardizes formats.
- Additional / Recommended Readings:
- https://www.datacamp.com/blog/data-preprocessing
- Figure-2
- : Steps in Data Preprocessing
- Source:
- https://www.geeksforgeeks.org/data-preprocessing-in-data-mining/

### Slide 5
- Why is it important?
- Real-world data is often messy, incomplete, inconsistent, or contains outliers
- .
- Algorithms
- require numerical, structured data with minimal inconsistencies
- .
- Clean
- data improves the accuracy, robustness, and generalization ability of AI/ML models.

### Slide 6
- Common Steps in Data Pre-processing
- Data Cleaning
- :
- Handle
- missing values (e.g., fill with mean/median or drop rows
- )
- Remove
- duplicate
- records
- Fix
- inconsistent data
- formats
- Data Transformation
- :
- Encode
- categorical values (Label Encoding, One-Hot Encoding
- )
- Normalize
- or standardize numerical features (Min-Max, Z-score
- )
- Data Reduction
- :
- Dimensionality
- reduction using PCA, Feature
- Selection
- Data
- Integration
- :
- Combining
- data from multiple sources (e.g., CSV + SQL data)

### Slide 7
- Data Pre-processing Packages (Pandas & NumPy)
- Pandas:
- A
- powerful open-source Python
- library Provides
- intuitive, flexible, and fast tools for working with structured data
- (Data Frames).
- NumPy
- : Fundamental
- package for scientific computing with
- Python Works
- efficiently with large numerical arrays and
- matrices.
- Additional / Recommended Readings:
- https://www.geeksforgeeks.org/difference-between-pandas-vs-numpy/
- Figure-3
- : Python
- Libraries for Data Manipulation and Analysis
- Source:
- https
- ://www.scalablepath.com/python/python-libraries-machine-learning

### Slide 8
- AIML
- Algorithms
- Machine
- Learning (ML) is a subset of artificial intelligence (AI) that enables computers to learn from data and improve their performance on tasks without being explicitly programmed
- .
- Machine Learning algorithms are the programs that can learn the hidden patterns from the data, predict the output, and improve the performance from experiences on their own.
- Additional / Recommended Readings
- :
- https://www.datacamp.com/blog/top-machine-learning-use-cases-and-algorithms
- Figure-4
- : AI and Its
- Subfields
- Source:
- https://www.datacamp.com/blog/top-machine-learning-use-cases-and-algorithms

### Slide 9
- Machine Learning
- Categories
- Supervised
- Learning:
- Uses labeled
- data
- Classification
- (e.g., email spam detection
- )
- Regression
- (e.g., price prediction
- )
- Unsupervised
- Learning:
- Uses unlabeled
- data
- Clustering
- (e.g., customer segmentation
- )
- Association
- (e.g., market basket analysis
- )
- Reinforcement Learning:
- Agent
- learns by interacting with
- environment
- Used
- in gaming, robotics, self-driving
- cars

### Slide 10
- Applications of AIML
- Natural Language Processing (NLP
- )
- Image
- and Speech
- Recognition
- Fraud Detection
- Predictive Maintenance
- Recommendation
- Systems
- Figure-5 : Applications of AIML in various fields
- Source:
- https://www.edureka.co/blog/artificial-intelligence-applications/

### Slide 11
- Summary of the
- Experiment
- Data Pre-processing:
- Essential for converting messy data into model-ready
- form
- Pandas
- and
- NumPy
- :
- Core
- Python tools for structured and numerical data
- operations
- AIML Algorithms:
- Enable
- systems to learn patterns, classify data, and make predictions

### Slide 12
- Next
- Experiment
- T
- opic(s)
- Introduction to Data
- Visualization
- Importance of Data Visualization in
- AIML
- Basic Plot Types Using
- Matplotlib

### Slide 13
- Quiz/ FAQ’s
- •
- What
- is the difference between Pandas and
- NumPy
- ?
- •  How do you create a
- NumPy
- array from a list?
- •  What is
- NumPy
- and why is it used in data analysis?
- •  How do you read a CSV file in Pandas ?
- •
- What
- is the difference between a Pandas Series and a
- DataFrame
- ?

### Slide 14
- R
- eferences/ Articles/ Videos
- Reference/Articles
- McKinney, W. (2017).Python for Data Analysis: Data Wrangling with Pandas,
- NumPy
- , and
- IPython
- (2nd ed.). O'Reilly Media.— A foundational book covering practical applications of Pandas and
- NumPy
- .
- Harris, C. R., et al. (2020).Array programming with
- NumPy
- . Nature, 585(7825), 357–362.— A peer-reviewed article discussing
- NumPy's
- role in scientific computing and data processing
- .
- Videos
- Data Preprocessing in Machine learning
- https
- ://
- www.youtube.com/watch?v=UoYO
- MjqiVQ&list
- =PLg8h8Ej1e8l2u2Hdt2EIX86SFJpgvUUs3
- Data Analysis with Python
- Numpy
- &
- Pandas
- https://www.youtube.com/watch?v=GPVsHOlRBBI

### Slide 15
- Additional
- learning
- R
- esources
- Additional Resources for Learning Basics of python
- https
- ://www.kaggle.com/learn/python
- https
- ://www.w3schools.com/python/default.asp
- Additional Resources for Learning Pandas and
- NumPy
- https://
- www.kaggle.com/code/chats351/introduction-to-numpy-pandas-and-matplotlib
- https
- ://
- www.w3schools.com/python/default.asp

### Slide 16
- Class-Wise
- Feedback
- 11
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 17
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in
- 12


---


================================================================================


# Experiment-1.2 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-1.2
# Experiment-1.2

## Perform exploratory data analysis (EDA) on a real-world dataset to identify patterns, correlations, and trends by using descriptive statistics and visualizations.

CO2

Objective:

To perform Exploratory Data Analysis (EDA) on a real-world dataset using descriptive statistics and data visualization techniques in order to identify hidden patterns, detect correlations among features, and uncover trends that inform data-driven decision-making and model building in AIML applications.

Tools/Platforms Used:

Google Colaboratory

Theory:

Introduction to EDA

Exploratory data analysis (EDA) is a fundamental process in data science and machine learning. It involves analyzing datasets to summarize their main characteristics, often using visual methods. EDA helps in identifying the underlying structure, spotting anomalies, testing hypotheses, and checking assumptions before applying any modeling techniques, as shown in the figure 1 below.

It was popularized by John Tukey, a pioneering statistician who emphasized understanding data patterns visually and statistically, rather than relying solely on model-based approaches.

Figure 1: A typical EDA process.

1.      Objectives of EDA

- To understand the structure, distribution, and quality of data.

- To detect missing values, outliers, and inconsistencies.

- To identify relationships and correlations between variables.

- To reduce data dimensionality through visualization and feature analysis.

- To guide feature engineering and model selection decisions.

2.      Components of EDA

Descriptive Statistics

Descriptive statistics provide summary measures that capture essential properties of the data.

- Measures of Central Tendency: Mean, Median, Mode

- Measures of Dispersion: Range, Variance, Standard Deviation

- Shape of Distribution: Skewness and Kurtosis

- Frequency Distributions: Value counts, Percentages

3.      Data Types and Structure

Understanding data types is essential for choosing the right visualization and analysis method:

- Numerical Data: Age, Salary, Temperature

- Categorical Data: Gender, City, Product Category

- Boolean Data: True/False, Yes/No

- Datetime Data: Timestamps

4.      Handling Missing and Duplicate Data

Missing values can significantly affect model performance.

- Detection: Using Pandas & Numpy

- Handling Methods:

- Imputation (mean, median, mode)

- Forward/backward fill

- Deletion (if missingness is small and random)

5.      Visualization Techniques in EDA

Univariate Analysis (single variable)

- Histogram: Distribution of numerical features

- Box Plot: Outliers and spread

- Bar Chart: Frequency of categorical variables

Bivariate Analysis (two variables)

- Scatter Plot: Relationship between two numerical features

- Correlation Matrix/Heatmap: Strength of linear relationships

- Grouped Bar Plot: Compare subgroups in categorical data

Multivariate Analysis (more than two variables)

- Pairplot (Seaborn): Grid of scatterplots for each pair

- Facet Grids: Multiple plots split by a categorical variable

- 3D Plots (Advanced): For visualizing high-dimensional data

6.      Correlation and Trends

Correlation refers to the degree to which two variables move in relation to each other.

- Pearson Correlation Coefficient (linear relationship)

- Spearman Rank Correlation (monotonic relationship)

7.      Outlier Detection

Outliers can distort models and lead to incorrect conclusions.

- Box Plots: Visual detection

- Z-score and IQR Method: Statistical detection

8.      Feature Engineering Insights from EDA

EDA often reveals:

- Which features can be transformed, dropped, or combined

- Which features have predictive power

- Need for encoding or scaling

9.      Importance of EDA Before Modeling

EDA Task

Purpose

Understand distribution

Choose correct model (e.g., linear vs tree-based)

Detect missing/outliers

Prevent model errors

Spot relationships

Select important features

Visualize feature relevance

Improve interpretability

## Codes

## Code 1 :- Load Dataset

import pandas as pd

df = pd.read_csv('data.csv')

print(df.to_string())

Output

## Code 2:Display Basic Information

df.info()

Output

## Code 3:-Summary Statistics

df.describe()

Output:-

## Code 4:- Check for Missing Values

df.isnull().sum()

Output:-

## Code 5:- Correlation Matrix

df.corr()

Output:-

## Code 6:- Heatmap of Correlations

import seaborn as sns

import matplotlib.pyplot as plt

plt.figure(figsize=(8, 6))

sns.heatmap(df.corr(), annot=True, cmap='coolwarm')

plt.title("Correlation Heatmap")

plt.show()

Output:-

## Code 7:- Boxplot for Outlier Detection

sns.boxplot(data=df)

plt.title("Box Plot for All Numeric Columns")

plt.show()

Output:-

## Code 8:- Scatter Plot (Pulse vs Calories)

plt.scatter(df['Pulse'], df['Calories'], color='purple')

plt.title("Pulse vs Calories")

plt.xlabel("Pulse")

plt.ylabel("Calories")

plt.grid()

plt.show()

Output:-

## Video Links

Exploratory Data Analysis

Exploratory Data Analysis with Pandas Python

Learn Exploratory Data Analysis (EDA) from Scratch

## Practical Task Question

- Write a Python program to load a real-world dataset using Pandas and display the first five records.

- Write a Python program to perform descriptive statistics such as mean, median, mode, standard deviation, minimum, and maximum.

- Write a Python program to check the shape, column names, data types, and basic information of a dataset.

- Write a Python program to identify missing values and handle them using suitable methods.

- Write a Python program to find duplicate records in a dataset and remove them.

- Write a Python program to analyze numerical columns using summary statistics.

- Write a Python program to find correlation among numerical features in a dataset.

- Write a Python program to visualize data trends using line charts and bar charts.

- Write a Python program to create a heatmap or correlation matrix to identify relationships among variables.

- Write a Python program to perform exploratory data analysis and identify patterns, correlations, and trends using Pandas, NumPy, and Matplotlib.

## Additional learning Resources

https://www.guvi.in/blog/exploratory-data-analysis-eda-in-data-science/

https://botpenguin.com/glossary/exploratory-data-analysis

https://featrix.ai/blog/simplify-data-exploration-with-embeddings

TEXT BOOKS/REFERENCE BOOKS

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


# Experiment-1.2 - All Lecture Slides Text


## Exp 1.2
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
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 1                   Experiment No.1.2
- Topic
- :
- Perform Exploratory Data Analysis (EDA) on a real-world dataset to identify patterns, correlations, and trends by using Descriptive statistics and visualizations
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester July-Dec 2026

### Slide 2
- Learning Objectives
- To understand and apply descriptive statistical methods to summarize and interpret the key characteristics of a real-world
- dataset.
- To
- identify meaningful patterns, correlations, and trends through graphical techniques such as histograms, box plots, scatter plots, and
- heatmaps
- .
- To
- develop the ability to draw insights from data that inform
- feature selection to guide
- machine learning model development.

### Slide 3
- Recap of Previous
- Experiment
- Objective:
- To explore the role of data visualization in AIML and learn how to create basic plots using the
- Matplotlib
- library in Python.
- Activities Performed:
- Implemented line plots, bar charts, histograms, scatter plots, and pie charts to visualize sample data and understand trends, distributions, and relationships.
- Outcome:
- Gained hands-on experience in visualizing data, improving data interpretation, and enhancing decision-making in machine learning workflows.

### Slide 4
- Perform Exploratory Data Analysis (EDA) on a real-world dataset to identify patterns, correlations, and trends by using Descriptive statistics and
- visualizations
- Topic 1
- .
- Descriptive Statistics for
- EDA
- Topic 2
- .
- Handling Missing and Duplicate Data
- Topic 3
- .
- Data Visualization Techniques in EDA
- Figure-1 :
- Exploratory Data Analysis
- Source:
- https
- ://featrix.ai/blog/simplify-data-exploration-with-
- embeddings

### Slide 5
- Exploratory Data Analysis (EDA)
- Exploratory Data Analysis (EDA) is a
- process of diving into a dataset to understand its main characteristics, patterns, and peculiarities before applying more complex analytical techniques.
- Additional / Recommended Readings:
- https://
- featrix.ai/blog/simplify-data-exploration-with-embeddings
- Figure-2
- : Exploratory
- Data Analysis (EDA)
- Process
- Source:
- https://botpenguin.com/glossary/exploratory-data-analysis

### Slide 6
- Why is it important?
- 1. Understanding the Dataset
- EDA helps you
- familiarize yourself with the structure, distribution, and types of data
- (categorical, numerical, etc.) before applying any machine learning models.
- 2. Identifying Data Quality Issues
- EDA allows you to
- detect and address missing values, duplicates, and outliers
- which can otherwise distort model performance.
- 3. Uncovering Hidden Patterns and Relationships
- Using visualizations (scatter plots,
- heatmaps
- , etc.), you can discover
- correlations and trends
- that inform feature selection and hypothesis generation.
- 4. Enhancing Model Performance
- Clean and well-understood data
- leads to better model accuracy
- and generalization.

### Slide 7
- Descriptive Statistics for EDA
- Descriptive statistics summarize and organize characteristics of a dataset
- .
- Key
- Metrics:
- Central Tendency:
- Mean, Median, Mode
- Dispersion:
- Range, Variance, Standard Deviation
- Shape of Data:
- Skewness
- ,
- Kurtosis
- Summary Function in Pandas:
- df.describe
- ()
- Purpose in EDA
- :
- Understand
- the general structure of the
- data
- Identify
- outliers or unusual
- distributions
- Compare
- features on a statistical basis
- Figure-3:
- Descriptive Statistics for
- EDA
- Source:
- https
- ://www.guvi.in/blog/exploratory-data-analysis-eda-in-data-science/

### Slide 8
- Handling Missing and Duplicate Data
- Real-world data is often incomplete or contains redundant entries. Cleaning this is crucial for reliable analysis
- .
- Handling Missing Data:
- Detection:
- df.isnull
- ().sum()
- Imputation:
- Fill with mean/median/mode
- Removal
- :
- Drop rows/columns using
- df.dropna
- ()
- Handling
- Duplicates:
- Detection:
- df.duplicated
- ()
- Removal:
- df.drop_duplicates
- ()
- Additional / Recommended Readings:
- https://www.guvi.in/blog/exploratory-data-analysis-eda-in-data-science/
- Figure-4: Missing Values from the Dataset
- Source:
- https://www.geeksforgeeks.org/ml-handling-missing-values/

### Slide 9
- Data Visualization Techniques in EDA
- Visualizing data makes patterns, trends, and outliers easier to detect and interpret
- .
- Common Plot Types:
- Histogram:
- Distribution of a variable
- Boxplot:
- Spread and outliers
- Scatter Plot:
- Correlation between two variables
- Heatmap
- :
- Feature correlation
- Pairplot
- :
- Multivariate relationships
- Figure-5:
- Data Visualization Techniques in EDA
- Source:
- https://www.guvi.in/blog/exploratory-data-analysis-eda-in-data-science/

### Slide 10
- Applications of EDA
- Healthcare
- In the healthcare domain, EDA is used to analyze patient data, disease outbreaks, drug effectiveness, and more.
- E-commerce
- E-commerce businesses employ EDA to analyze customer shopping patterns and make effective recommendations.
- Finance
- Financial institutions apply EDA to identify trends and patterns in financial markets.
- Sports Analytics
- EDA has a foothold in sports analytics, where it provides insights into player performance, team dynamics, and game strategy.
- Social Media Analysis
- In the realm of social media, EDA is employed to understand
- trends
- , and interactive patterns.

### Slide 11
- Summary of the
- Experiment
- Objective:
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>To perform Exploratory Data Analysis (EDA) on a real-world dataset to identify patterns, correlations, and trends using descriptive statistics and data visualization techniques
- .
- Activities
- Performed:
- Computed statistical measures such as mean, median, standard deviation, and correlation.
- Handled missing and duplicate data using Pandas.
- Created visualizations including histograms, box plots, scatter plots, and
- heatmaps
- using
- Matplotlib
- and
- Seaborn
- .
- Outcome
- :
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Learners gained the ability to summarize and clean raw data, visualize hidden relationships, and prepare the dataset for machine learning models, improving the reliability of further analysis.

### Slide 12
- Next
- Experiment
- T
- opic(s)
- Introduction to
- Supervised ML
- Exploring the Dataset
- Cleaning and Converting
- Data
- Splitting and Summarizing Data

### Slide 13
- Quiz/ FAQ’s
- •What
- is the purpose of using describe () in exploratory data analysis
- ?
- •How
- does a heat map help in understanding the correlation between features
- ?
- •Why
- do we use boxplots during EDA and what insights can we draw from them
- ?
- •What
- is the significance of binning continuous variables like Duration
- ?
- •How
- a pair plot is useful compared to individual scatter plots?

### Slide 14
- R
- eferences/ Articles/ Videos
- Reference/Articles
- Zhang, Z. (2017).Data visualization in machine learning: A review
- . IEEE
- Access, 6, 41256–41268
- .
- Reviews various visualization techniques and their use in data analysis and ML workflows
- .
- Koehrsen
- , W. (2018).A Comprehensive Guide to Exploratory Data Analysis (EDA) in Python
- . Towards
- Data Science (Medium
- ).Great
- beginner guide using Pandas,
- Matplotlib
- , and
- Seaborn
- for EDA
- .
- Videos
- Exploratory Data Analysis
- https
- ://
- www.youtube.com/watch?v=QiqZliDXCCg
- Learn Exploratory Data Analysis (EDA) from
- Scratch
- https
- ://www.youtube.com/watch?v=xi0vhXFPegw

### Slide 15
- Additional
- learning
- R
- esources
- https://www.guvi.in/blog/exploratory-data-analysis-eda-in-data-science
- /
- https://
- botpenguin.com/glossary/exploratory-data-analysis
- https://featrix.ai/blog/simplify-data-exploration-with-embeddings

### Slide 16
- Class-Wise
- Feedback
- 11
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 17
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in
- 12


---


================================================================================


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


================================================================================


# Experiment-1.4 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-1.4
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

---


## 🖥️ PRESENTATION SLIDES


# Experiment-1.4 - All Lecture Slides Text


## Exp 1.4
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
- Unit No.
- 1
- Experiment No.1.4
- Topic
- :
- Build a classification model by using different machine learning
- algorithms
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec
- 2026

### Slide 2
- Learning
- Objectives
- Understand the fundamental concepts of classification in supervised machine learning
- , including the difference between binary and multiclass classification
- problems.
- Implement
- and compare multiple classification algorithms
- (such as Decision Tree, K-Nearest Neighbors, Support Vector Machine, Logistic Regression, and Random Forest) on a given dataset using appropriate libraries and tools
- .
- Evaluate model performance using metrics
- like accuracy, precision, recall, F1-score, and confusion matrix to determine the most suitable algorithm for a given classification task.

### Slide 3
- Recap
- of Previous Experiment
- Learn the concept of supervised learning
- and how it uses labeled data to train classification models.
- Apply algorithms like Logistic Regression, Decision Trees, and K-NN
- to build and train classifier models.
- Evaluate model performance
- using metrics such as accuracy, precision, recall, and confusion matrix.

### Slide 4
- Topic 1 :Overview of Classification and Machine Learning Algorithms
- Topic 2:Building and Training Classification Models
- Topic 3 :Evaluating and Comparing Model Performance
- Figure-1 :
- Machine Learning Algorithms for
- Classification
- Source:
- https
- ://towardsdatascience.com/top-machine-learning-algorithms-for-classification-2197870ff501/
- Build a classification model by using different
- Machine Learning Algorithms

### Slide 5
- Introduction to Classification Models
- Definition
- :
- Classification models predict discrete outcomes (e.g., spam vs. non-spam).
- Key Concepts in Classification
- Preprocessing:
- Data must be cleaned, normalized, and encoded (for categorical features) before training.
- Training
- and Testing Data:
- The dataset is split into training and testing sets to evaluate the model's performance on unseen data
- .
- Features and Target Variable:
- Features are the input variables (independent variables), and the target variable (dependent variable) is the class to be predicted
- .
- Evaluation Metrics:
- Accuracy, precision, recall, F1-score, confusion matrix, ROC-AUC, etc., are used to assess model performance
- .
- Figure-2:
- Steps in Building a Classifier Model
- Source:
- https
- ://www.techguruspeaks.com/classification-technique/

### Slide 6
- Popular Machine Learning Algorithms for Classification
- Logistic
- Regression Algorithm:
- Suitable for binary classification tasks; uses a logistic function to model the probability of a class.
- Additional/Recommended Readings
- https://www.geeksforgeeks.org/understanding-logistic-regression/
- Figure-3 : Linear Vs. Logistic Regression
- Source:
- https
- ://medium.com/@
- praveenraj.gowd
- /why-is-logistic-regression-called-logistic-regression-and-not-a-logistic-classification-5a418293040d

### Slide 7
- Decision
- Tree Algorithm
- Splits data based on feature values; provides interpretable results but can
- over fit
- on small datasets.
- Figure-4 : Decision Tree Algorithm
- Source:
- https
- ://blog.gopenai.com/decision-tree-algorithm-484ec33387f9

### Slide 8
- Random
- Forest
- Algorithm
- An ensemble of decision trees; reduces
- over fitting
- and improves generalization.
- Figure-5 : Random Forest Algorithm
- Source:
- https
- ://www.geeksforgeeks.org/random-forest-algorithm-in-machine-learning/

### Slide 9
- Support Vector Machine (SVM
- ) Algorithm
- Finds the optimal
- hyper plane
- to separate classes; works well with small datasets and high-dimensional spaces.
- Figure-6 : SVM Algorithm
- Source:
- https
- ://spotintelligence.com/2024/05/06/support-vector-machines-
- svm
- /

### Slide 10
- K-Nearest Neighbors (KNN
- ) Algorithm
- Classifies based on the majority vote of nearest neighbors; simple but computationally expensive for large datasets.
- Figure-7 : KNN Algorithm
- Source:
- https
- ://www.kaggle.com/code/tawfikelmetwally/knn-classification-model

### Slide 11
- Naive
- Bayes Algorithm
- Based on Bayes' Theorem; works well with categorical data and text classification.
- Figure-8 : NB Algorithm
- Source:
- https
- ://techntales.medium.com/na%C3%AFve-bayes-a-simple-yet-powerful-machine-learning-algorithm-7b0dca78b483

### Slide 12
- Training with Different Algorithms
- Train models using multiple algorithms:-
- Logistic
- Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- k-Nearest
- Neighbours
- (k-NN)

### Slide 13
- Model Evaluation Metrics
- Use metrics to evaluate performance:
- Accuracy
- Precision
- Recall
- F1-Score

### Slide 14
- Comparison of Algorithms
- Evaluate multiple algorithms and compare
- results:

### Slide 15
- Summary of the
- Experiment
- Dataset Preparation and Exploration
- : A labeled dataset is preprocessed and explored to identify key features and class distributions suitable for classification tasks
- .
- Model Implementation
- : Various machine learning classification algorithms such as Logistic Regression, Decision Tree, K-Nearest Neighbors, and Support Vector Machine are implemented using Python libraries like
- scikit
- -learn
- .
- Model Evaluation and Comparison
- : The performance of each model is assessed using metrics like accuracy, precision, recall, F1-score, and confusion matrix to determine the most effective classifier for the dataset.

### Slide 16
- Next
- Experiment
- T
- opic(s)
- Introduction to Emotion and Gesture
- Detection
- AI Model Design and
- Implementation
- Evaluation and Applications

### Slide 17
- Quiz/ FAQ’s
- What are the key steps involved in building a classification model, and why is data preprocessing essential?
- Explain the difference between Logistic Regression and Decision Trees as classification algorithms.
- What is the purpose of feature scaling, and which algorithms require it?
- How do you evaluate the performance of a classification model, and why are multiple metrics used?
- Can you explain the trade-offs between accuracy and other metrics like precision and recall in classification problems?

### Slide 18
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

### Slide 19
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

### Slide 20
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 21
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in


---


================================================================================


# Experiment-2.1 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-2.1
# Experiment-2.1

## Introduction to Artificial Intelligence and Machine Learning Concepts.

## CO1

##

## Aim

To study the basic concepts of Artificial Intelligence, including Generative AI, AI agents, Natural Language Processing, Speech AI, Computer Vision, Information Extraction, and Responsible AI, and to understand their real-world applications.

## Tool/Platform Used:

Microsoft Azure Cloud Platform

## Objectives

After performing this experiment, students will be able to:

- Understand the meaning and purpose of Artificial Intelligence.

- Explain how Generative AI works.

- Understand the role of AI agents.

- Identify applications of Natural Language Processing.

- Explain speech recognition and speech synthesis.

- Understand computer vision and its types.

- Explain how AI extracts information from documents, images, and recordings.

- Understand the importance of Responsible AI.

## Theory

## 1. Introduction to Artificial Intelligence

Artificial Intelligence, commonly known as AI, is a branch of computer science that enables machines or software systems to perform tasks that normally require human intelligence. These tasks include understanding language, recognizing images, making decisions, solving problems, learning from data, and interacting with users, as shown in Figure 1. AI is used in many areas of daily life, such as chatbots, voice assistants, recommendation systems, facial recognition, self-driving vehicles, fraud detection, medical diagnosis, and automatic translation.

The main purpose of AI is to make machines capable of learning from data and improving their performance without being explicitly programmed for every situation.

For example, an AI-based learning platform can understand a student’s question, give an answer, explain a topic, and even suggest what to study next.

##                  Figure 1 : AI includes machine learning, neural networks, NLP, and robotics to make machines intelligent.

## 2. Generative AI

Generative AI is a type of artificial intelligence that can create new content. This content may include text, images, audio, video, computer code, summaries, reports, or conversations. Generative AI works using models that are trained on large amounts of data. These models learn patterns, relationships, and meanings from the data. When a user gives a prompt, the model generates a suitable response based on what it has learned.

For example, if a user asks, “Explain machine learning in simple words,” a generative AI system can create a new explanation in natural language.

Generative AI is widely used for writing assistance, content creation, coding help, summarization, translation, report generation, and chatbot development.

Figure 2: Generative AI uses data to create new content like text, images, audio, and reports.

## 3. Large Language Models and Small Language Models

Large Language Models, also called LLMs, are AI models trained on huge amounts of text data. They can understand and generate human-like language. Examples of tasks performed by LLMs include answering questions, writing essays, summarizing documents, and generating code. Small Language Models, also called SLMs, are smaller models designed for specific tasks or limited domains. They require fewer resources and can be used in local devices, mobile applications, or specific business systems. The key differences are shown in Figure 3.

LLMs are more powerful and general-purpose, while SLMs are useful when the task is focused, cost-effective, or needs to run on smaller systems.

Figure 3: Comparison between Large Language Models and Small Language Models

## 4. AI Agents

AI agents are software applications built using generative AI. They can understand natural language, reason over information, use tools, and perform actions as shown in Figure 4.

An AI agent usually has three main components:

First, it has a language model, which acts like the brain of the agent. It helps the agent understand the user’s request and generate responses.

Second, it has instructions. These instructions define the role, behavior, and limits of the agent. For example, an AI agent may be instructed to behave like a teaching assistant, customer support agent, or personal planner.

Third, it has tools. These tools help the agent interact with the outside world. Tools may include search engines, databases, email systems, calendars, calculators, or business applications.

For example, an AI assistant can read a user’s message, check the calendar, schedule a meeting, send an email, and give confirmation to the user.

Figure 4: AI agents can plan, make decisions, learn, and assist users intelligently.

## 5. Natural Language Processing

Natural Language Processing, or NLP, is a branch of AI that deals with understanding and processing human language. It allows computers to read, understand, analyze, summarize, and generate text as shown in Figure 5.

NLP is the foundation of many AI systems, especially chatbots and language models. It helps machines understand the meaning of words, sentences, and documents. Common NLP tasks include language detection, text classification, sentiment analysis, keyword extraction, entity detection, summarization, and translation.

For example, an AI system can analyze product reviews and determine whether customers are happy or unhappy. It can also extract important names, dates, locations, and organizations from a document.

Figure 5: Natural Language Processing and its key applications

## 6. Text Analysis

Text analysis is the process of using AI to understand written content. It helps in extracting useful information from large amounts of text.

Important text analysis techniques include:

Language detection means identifying the language used in a text. For example, AI can detect whether a document is written in English, Hindi, French, or another language.

Text classification means assigning text to a category. For example, emails can be classified as spam or not spam.

Sentiment analysis means identifying whether a text expresses a positive, negative, or neutral opinion. For example, “This product is excellent” shows positive sentiment.

Key-term extraction means identifying important words or phrases in a document.

Entity detection means finding names of people, places, organizations, dates, phone numbers, or other specific information.

Summarization means reducing long text into a shorter version while keeping the main meaning.

Text analysis is useful in customer feedback analysis, social media monitoring, document processing, meeting summaries, and chatbot systems.

## 7. Speech in AI

Speech AI allows users to interact with machines using spoken language. It makes communication with computers more natural and user-friendly.

There are two major parts of speech AI: speech recognition and speech synthesis.

## Speech Recognition

Speech recognition is the ability of AI to understand spoken words and convert them into text. This is also called speech-to-text.

For example, when a user speaks into a mobile phone and the phone types the message automatically, speech recognition is being used.

Speech recognition is used in voice assistants, call center transcription, meeting transcription, voice search, dictation software, and automated customer support systems.

Modern speech recognition systems are becoming better at handling background noise, different accents, interruptions, and multiple speakers.

## Speech Synthesis

Speech synthesis is the ability of AI to convert written text into spoken voice. This is also called text-to-speech.

For example, when a navigation app reads directions aloud, it uses speech synthesis.

Speech synthesis is used in virtual assistants, screen readers, audiobooks, automated announcements educational tools, and accessibility applications.

Modern AI voices are becoming more natural, expressive, and human-like, as shown in Figure 6.

## Figure 6: Speech synthesis process using input audio, reference text, speaker recognition, and vocoder-based synthetic audio generation

## 8. Computer Vision

Computer vision is the area of AI that deals with analyzing and understanding visual input such as images, videos, and live camera feeds.

It enables machines to “see” and interpret visual information. Computer vision systems are trained using large numbers of images. The model learns patterns from these images and uses them to identify objects, people, text, scenes, or activities.

For example, a computer vision system can identify a car in an image, detect a face in a photograph, or recognize items in a supermarket, as shown in Figure 7.

## Figure 7: Object detection in computer vision identifying people, vehicles, traffic lights, signs, and animals in a street scene

## Types of Computer Vision

Image classification is used to identify the main subject of an image. For example, an image may be classified as a dog, car, laptop, or building.

Object detection is used to identify and locate objects within an image. It usually draws boxes around detected objects.

Semantic segmentation is an advanced technique that identifies the exact pixels belonging to an object. Instead of only drawing a box, it marks the complete shape of the object.

Multi-modal models combine image understanding with text understanding. They can describe images in natural language or answer questions about an image.

Computer vision is used in facial recognition, medical imaging, security monitoring, self-driving cars, robotics, quality inspection, retail checkout systems, and visual search.

## 9. Information Extraction

Information extraction is the process of using AI to find and collect useful information from unstructured data. Unstructured data includes scanned documents, handwritten forms, images, audio recordings, videos, and meeting transcripts.

A common technology used in information extraction is Optical Character Recognition, or OCR.

## Optical Character Recognition

OCR is a computer vision technique that identifies text from images or scanned documents. It converts printed or handwritten text into machine-readable text.

For example, when a receipt is scanned and the system automatically extracts the date, amount, shop name, and tax details, OCR and information extraction are being used as shown in Figure 8.

Figure 8: OCR process converting a scanned document image into editable text

Information extraction is useful in processing invoices, receipts, bank forms, ID cards, application forms, medical records, and business documents.

It is also used to index documents for search and to identify important points from meeting transcripts.

## 10. Responsible AI

Responsible AI means developing and using AI systems in a safe, fair, transparent, and accountable manner. Since AI systems can affect people’s lives, they must be designed carefully to avoid harm, bias, discrimination, privacy violations, and unsafe actions.

Responsible AI ensures that AI is not only powerful but also ethical and trustworthy.

The main principles of Responsible AI are fairness, reliability and safety, privacy and security, inclusiveness, transparency, and accountability.

## Principles of Responsible AI

Fairness means AI should not discriminate against people based on gender, caste, race, religion, disability, or other irrelevant factors. AI systems should be tested to reduce bias.

Reliability and safety means AI systems should work correctly and safely. Since AI can make mistakes, systems should include checks and safeguards.

Privacy and security means personal and sensitive data should be protected. AI systems should not expose private information.

Inclusiveness means AI should be usable by different types of people, including people with disabilities. For example, a speech-based AI system should also provide text captions for hearing-impaired users.

Transparency means users should know when they are interacting with AI. The system should also explain its limitations where necessary.

Accountability means the developers and organizations using AI are responsible for its outcomes. They must create rules and governance systems for safe AI usage.

## Codes: Demonstration of Responsible AI Principles

## 1. Fairness: Compare Selection Rates

import pandas as pd

data = {

"Name": ["Aman", "Rahul", "Neha", "Priya"],

"Gender": ["Male", "Male", "Female", "Female"],

"Selected": [1, 1, 1, 0]

}

df = pd.DataFrame(data)

selection_rate = df.groupby("Gender")["Selected"].mean() * 100

print(df)

print("\nSelection rate:")

print(selection_rate)

Males have a 100% selection rate while females have only 50%, the result indicates a possible fairness problem or gender bias.

## 2. Reliability: Check Whether AI Gives Consistent Results

import pandas as pd

data = {

"Test_Number": [1, 2, 3, 4, 5],

"AI_Prediction": [80, 81, 79, 80, 82]

}

df = pd.DataFrame(data)

average = df["AI_Prediction"].mean()

difference = df["AI_Prediction"].max() - df["AI_Prediction"].min()

print(df)

print("\nAverage prediction:", average)

print("Maximum variation:", difference)

if difference <= 5:

print("The AI system is reliable.")

else:

print("The AI system needs to be checked.")

Small variation indicates that the AI system is producing consistent results.

## 3. Safety: Detect Invalid Input Data

import pandas as pd

data = {

"Name": ["Aman", "Neha", "Rahul", "Priya"],

"Age": [25, -5, 150, 30]

}

df = pd.DataFrame(data)

invalid_data = df[(df["Age"] < 0) | (df["Age"] > 100)]

print("Complete data:")

print(df)

print("\nInvalid data:")

print(invalid_data)

##

The program identifies impossible values before they are given to an AI system.

## 4. Privacy: Hide Phone Numbers

import pandas as pd

data = {

"Name": ["Aman", "Neha", "Rahul"],

"Phone": ["9876543210", "9123456780", "9988776655"]

}

df = pd.DataFrame(data)

df["Protected_Phone"] = "XXXXXX" + df["Phone"].str[-4:]

print(df[["Name", "Protected_Phone"]])

Output will show only the last four digits of each phone number.

## 5. Security: Block Users After Multiple Failed Logins

import pandas as pd

data = {

"User": ["User1", "User2", "User3"],

"Failed_Login_Attempts": [1, 5, 2]

}

df = pd.DataFrame(data)

df["Access"] = df["Failed_Login_Attempts"].apply(

lambda attempts: "Blocked" if attempts >= 3 else "Allowed"

)

print(df)

Users with three or more failed login attempts are blocked.

## 6. Inclusiveness: Check Group Representation

import pandas as pd

data = {

"User": ["A", "B", "C", "D", "E", "F"],

"Language": ["English", "Hindi", "English", "Punjabi", "Hindi", "English"]

}

df = pd.DataFrame(data)

language_count = df["Language"].value_counts()

print(df)

print("\nUsers from each language group:")

print(language_count)

##

This checks whether users from different language groups are included in the data.

## 7. Transparency: Explain Why a Decision Was Made

import pandas as pd

data = {

"Name": ["Aman", "Neha", "Rahul"],

"Marks": [75, 45, 82]

}

df = pd.DataFrame(data)

df["Decision"] = df["Marks"].apply(

lambda marks: "Selected" if marks >= 60 else "Not Selected"

)

df["Explanation"] = df["Marks"].apply(

lambda marks: "Marks are 60 or above"

if marks >= 60

else "Marks are below 60"

)

print(df)

The rule is clearly visible: applicants with 60 or more marks are selected.

## 8. Accountability: Maintain an AI Decision Record

import pandas as pd

data = {

"Applicant": ["Aman", "Neha", "Rahul"],

"AI_Decision": ["Selected", "Rejected", "Selected"],

"Checked_By": ["Dr. Kumar", "Dr. Kumar", "Dr. Sharma"],

"Final_Status": ["Approved", "Review Required", "Approved"]

}

audit_record = pd.DataFrame(data)

print(audit_record)

audit_record.to_csv("AI_Decision_Record.csv", index=False)

print("\nAccountability record saved successfully.")

##

This keeps a record of the AI decision, the person responsible for checking it, and the final status.

## Practical Questions / Tasks

- Write a short note on Artificial Intelligence and its importance.

- Explain Generative AI with one real-life example.

- Write the difference between Large Language Models and Small Language Models.

- Explain the working of an AI agent.

- Write the main components of an AI agent.

- Explain Natural Language Processing and its applications.

- Write the difference between speech recognition and speech synthesis.

- Explain computer vision with the help of object detection.

- Explain OCR and its use in information extraction.

- Write the principles of Responsible AI.

## Video Links

Introduction to Artificial Intelligence

Introduction to Generative AI and LLMs

Full Course: AI Agents for Beginners

Object Detection with Python Full Course | Computer Vision

Principles of Responsible AI

## Additional Resources

- Microsoft Learn: Get started with AI applications and agents on Azure

https://learn.microsoft.com/en-us/training/paths/get-started-ai-apps-agents/

- Microsoft Learn: Introduction to AI concepts

https://learn.microsoft.com/en-us/training/modules/get-started-ai-fundamentals/

- Google Machine Learning Crash Course

https://developers.google.com/machine-learning/crash-course

- Google Cloud: Machine Learning and AI Training

https://cloud.google.com/learn/training/machinelearning-ai

- Google Skills: Introduction to Generative AI

https://www.skills.google/course_templates/536

- IBM: What is Machine Learning?

https://www.ibm.com/think/topics/machine-learning

- IBM: What is Responsible AI?

https://www.ibm.com/think/topics/responsible-ai

- Microsoft Azure AI Fundamentals Certification

https://learn.microsoft.com/en-us/credentials/certifications/azure-ai-fundamentals/

- Microsoft AI-900 Study Guide

https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ai-900

- IBM SkillsBuild: Artificial Intelligence

https://skillsbuild.org/college-students/artificial-intelligence

## Text Books

- Artificial Intelligence: Foundations of Computational Agents — David L. Poole & Alan K. Mackworth

PDF/Online: https://artint.info/3e/html/ArtInt3e.html

Useful for: AI basics, agents, intelligent systems.

- Speech and Language Processing — Daniel Jurafsky & James H. Martin

PDF: https://web.stanford.edu/~jurafsky/slp3/ed3book_jan26.pdf

Useful for: NLP, speech recognition, language models.

- Computer Vision: Algorithms and Applications — Richard Szeliski

Book/PDF page: https://szeliski.org/Book/

Useful for: computer vision, image classification, object detection.

- Dive into Deep Learning — Aston Zhang, Zachary C. Lipton, Mu Li, Alexander J. Smola

PDF: https://d2l.ai/d2l-en.pdf

Useful for: machine learning, neural networks, deep learning, AI models.

- Neural Networks and Deep Learning — Michael Nielsen

Online book: http://neuralnetworksanddeeplearning.com/

Useful for: neural networks and model training basics.

## Reference Books

- Responsible AI Standard — Microsoft

PDF: https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE5cmFl

Useful for: responsible AI, fairness, reliability, privacy, transparency.

- Artificial Intelligence Risk Management Framework — NIST

PDF: https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf

Useful for: AI safety, accountability, risk management.

- Towards Responsible AI for All — NITI Aayog

PDF: https://www.niti.gov.in/sites/default/files/2021-08/Part2-Responsible-AI-12082021.pdf

Useful for: Indian context of responsible AI and ethics.

- Google Machine Learning Crash Course

Online: https://developers.google.com/machine-learning/crash-course

Useful for: machine learning concepts and beginner AI learning.

- Microsoft Learn: Introduction to AI Concepts

Online: https://learn.microsoft.com/en-us/training/modules/get-started-ai-fundamentals/

Useful for: same experiment topics — generative AI, NLP, speech, vision, information extraction, and responsible AI.

---


## 🖥️ PRESENTATION SLIDES


# Experiment-2.1 - All Lecture Slides Text


## Exp 2.1
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
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 2                   Experiment No.2.1
- Topic
- :Introduction to Artificial Intelligence and Machine Learning Concepts
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning
- Objectives
- To understand
- the basic concept of Artificial Intelligence and its role in solving real-world problems.
- To
- study
- the working of Generative AI and how it creates new content such as text, images, audio, and code.
- To
- understand
- the concept of AI agents and their components such as language models, instructions, and tools
- .

### Slide 3
- Recap
- of Previous Experiment
- Learn the concept of supervised learning
- and how it uses labeled data to train classification models.
- Apply algorithms like Logistic Regression, Decision Trees, and K-NN
- to build and train classifier models.
- Evaluate model performance
- using metrics such as accuracy, precision, recall, and confusion matrix.

### Slide 4
- Topic 1: Introduction to
- AI
- Topic
- 2: Generative AI and
- Agents
- Topic
- 3: Text and Natural Language
- Processing
- Topic
- 4: Speech and Computer
- Vision
- Topic
- 5: Information Extraction and Responsible AI
- Figure-1 :
- AI concepts and common AI
- workloads
- Source :
- https://www.openxcell.com/artificial-intelligence/
- AI Concepts and Applications Covered

### Slide 5
- Introduction to AI
- Artificial Intelligence is a branch of computer science that enables machines to perform tasks that normally require human intelligence
- .
- AI systems can learn from data, understand language, recognize images, make decisions, and solve problems
- .
- Examples
- :
- Chabot's,
- voice assistants, recommendation systems, fraud detection, self-driving cars.
- Figure-2:
- Introduction to AI
- Source:
- https://www.linkedin.com/pulse/introduction-ai-dhruv-sharan-azipe/

### Slide 6
- Generative AI creates new content such as text, images, audio, video, code, and summaries
- .
- AI agents are intelligent software systems that use models, instructions, and tools to complete tasks
- .
- Examples:
- AI
- chatbot
- , email assistant, calendar assistant, document summarizer.
- Figure-3 :
- Flow Diagram of AI Agents
- Source:
- https://www.elixirclaw.ai/blog/what-are-ai-agents
- Generative AI and Agents

### Slide 7
- Natural Language Processing helps computers understand and process human language
- .
- It is used for language detection, sentiment analysis, text classification, entity detection, translation, and summarization
- .
- Example:
- An AI tool summarizing a long article into key points.
- Figure-4
- :Industrial Applications of
- NLP
- Source:
- https://www.elinext.com/solutions/ai/trends/the-future-of-natural-language-processing/
- Natural Language Processing

### Slide 8
- Speech AI allows machines to understand spoken language and generate spoken responses
- .
- Computer Vision enables machines to analyze images, videos, and camera feeds
- .
- Examples:
- Speech-to-text, text-to-speech, object detection, facial recognition, image classification.
- Figure-5
- :Computer Vision
- Source:
- https://iothook.com/en/computer-vision-cv/
- Speech and Computer Vision

### Slide 9
- Information extraction uses AI to collect useful information from documents, images, audio, and videos
- .
- OCR, or Optical Character Recognition, converts scanned documents or images into editable text.
- Example
- :
- Extracting amount, date, and merchant name from a scanned receipt.
- Figure-6 :
- Information Extraction and OCR
- Source:
- https://www.docsumo.com/blogs/data-extraction/ocr
- Information Extraction and OCR

### Slide 10
- Responsible AI means designing AI systems that are safe, fair, transparent, secure, inclusive, and accountable
- .
- Important principles include fairness, reliability, privacy, security, inclusiveness, transparency, and accountability.
- Figure-7
- :
- Key Principles of Responsible
- AI
- Source:
- https://insights.daffodilsw.com/blog/demystifying-responsible-ai-principles-and-best-practices-for-ethical-ai-implementation
- Responsible AI

### Slide 11
- Summary of the
- Experiment
- Artificial Intelligence enables machines to perform intelligent tasks such as learning, reasoning, decision-making, understanding language, and solving real-world problems
- .
- Generative
- AI, NLP, Speech AI, Computer Vision, and OCR help machines create content, process text, understand voice, analyze images, and extract useful information from documents
- .
- Responsible
- AI ensures that AI systems are developed and used in a safe, fair, transparent, secure, inclusive, and ethical manner.

### Slide 12
- Next
- Experiment
- T
- opic(s)
- Topic 1. Generative Artificial Intelligence
- Topic 2. Prompts and Prompt Types
- Topic 3. Large Language Models
- Topic 4. Retrieval Augmented Generation
- Topic 5. AI Agents

### Slide 13
- Quiz/ FAQ’s
- What is Artificial Intelligence
- ?
- What
- is Generative AI
- ?
- What
- are AI agents
- ?
- What
- is NLP
- ?
- What
- is OCR
- ?
- Why
- is Responsible AI important?

### Slide 14
- R
- eferences/ Articles/ Videos
- Reference/ Articles
- Microsoft Learn — Introduction to AI Concepts
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:hlinkClick r:id="rId3"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/modules/get-started-ai-fundamentals/
- Microsoft Learn — Introduction to Generative AI and Agents
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/modules/fundamentals-generative-ai/
- Microsoft Learn — Get Started with AI Applications and Agents on Azure
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:hlinkClick r:id="rId5"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/paths/get-started-ai-apps-agents/
- Videos
- Introduction to Generative AI and LLMs
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:hlinkClick r:id="rId6"/></a:rPr><a:t>https://learn.microsoft.com/en-us/shows/generative-ai-for-beginners/introduction-to-generative-ai-and-llms-generative-ai-for-beginners
- AI, Machine Learning, Deep Learning and Generative AI Explained
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:hlinkClick r:id="rId7"/></a:rPr><a:t>https://www.youtube.com/watch?v=qYNweeDHiyU
- Generative
- vs
- Agentic
- AI: Shaping the Future of AI Collaboration
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:hlinkClick r:id="rId8"/></a:rPr><a:t>https://www.youtube.com/watch?v=EDb37y_MhRw

### Slide 15
- Additional
- learning
- R
- esources
- Microsoft Learn — Introduction to AI Concepts
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId3"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/modules/get-started-ai-fundamentals/
- Microsoft Learn — Get Started with AI Applications and Agents
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/paths/get-started-ai-apps-agents/
- Microsoft Learn — Introduction to Generative AI and Agents
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId5"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/modules/fundamentals-generative-ai/
- Google Machine Learning Crash Course
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId6"/></a:rPr><a:t>https://developers.google.com/machine-learning/crash-course
- Microsoft AI for Beginners
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId7"/></a:rPr><a:t>https://microsoft.github.io/AI-For-Beginners/

### Slide 16
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 17
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in


---


================================================================================


# Experiment-2.2 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-2.2
# Experiment-2.2

##

## Understanding Azure Machine Learning, Generative AI Models, and AI Agent systems.

##

## CO1

##

## Aim

To study and understand the basic concepts of Generative Artificial Intelligence, prompts, Large Language Models, Retrieval Augmented Generation, and AI agents.

## Objective

The objective of this experiment is to understand how Generative AI works and how it is used to create human-like content. This experiment also explains how prompts are used to communicate with AI models, how Large Language Models process language, how Retrieval Augmented Generation improves the accuracy of AI responses, and how AI agents use tools to perform tasks.

## Introduction

Generative Artificial Intelligence, commonly called Generative AI, is a branch of artificial intelligence that can create new content as shown in Figure 1. This content may include text, images, poems, stories, summaries, computer code, and answers to questions. It is called “generative” because it can generate new output based on the input given by the user.

Figure 1: Overview of Generative Artificial Intelligence for creating audio, video, image, and text content.

Generative AI has become very popular because it can produce human-like responses. It may appear magical because it can write essays, explain difficult concepts, generate code, or summarize large documents within seconds. However, Generative AI does not work by magic. It works through mathematical techniques, statistics, machine learning, data science, and large-scale training on data.

The main idea behind Generative AI is that it learns patterns from large amounts of information. After learning these patterns, it can predict and generate suitable responses. For example, if a user asks a question, the AI model understands the language of the question and generates a meaningful answer.

Generative AI is used in many areas such as education, research, business, programming, content writing, customer support, and automation. It helps users complete work faster and understand complex topics in simple language.

## Theory

Generative AI works with the help of advanced AI models known as "Large Language Models." These models are trained to understand and generate natural language as shown in Figure 2. Natural language means the language used by humans in daily communication, such as English, Hindi, or any other spoken or written language.

Figure 2: Working process of a Large Language Model, showing training data, tokenization, contextual understanding, and text generation.

A Large Language Model learns the relationship between words, phrases, and sentences. It does not simply copy answers. Instead, it predicts the most suitable next word or token based on the input given to it. This input is called a prompt, and the answer generated by the model is called a completion.

For example, if we write:

“I heard a dog…”

The model may predict the next word as

“bark”

This is because the model has learned that the word “dog” is commonly related to the sound “bark.” In this way, the model generates meaningful text step by step.

## Large Language Models

A Large Language Model, or LLM, is the core technology behind many Generative AI systems. LLMs are trained on very large amounts of text data. This training helps them understand grammar, sentence structure, word meaning, and context.

LLMs work like very advanced predictive text systems. In mobile phones, predictive text suggests the next word while typing. Similarly, LLMs predict the next token, but they are much more powerful because they have learned from huge amounts of data.

The working of an LLM includes several important steps:

First, the input text is broken into smaller units called tokens. Then, these tokens are converted into numerical forms so that the computer can process them. After that, the model understands the relationship between tokens using a transformer architecture. Finally, it predicts the next most suitable token and generates a response.

## Tokenization

Tokenization is the process of breaking text into smaller parts called tokens. Tokens may be complete words, parts of words, punctuation marks, or characters.

For example, the sentence:

“I heard a dog bark loudly.”

can be divided into tokens as follows:

Token

Explanation

I

Pronoun

heard

Action related to sound

a

Article

dog

Animal

bark

Sound made by a dog

loudly

Describes the sound

Each token is assigned a unique numerical value. This is necessary because computers do not directly understand human language. They process numbers, so words must be converted into numerical form.

Tokenization is important because it helps the AI model read, process, and understand the input text.

## Embeddings

After tokenization, the tokens are converted into numerical vectors. These vectors are called embeddings. An embedding represents the meaning of a token in mathematical form.

Embeddings help the model understand relationships between words. For example, the words "dog," "puppy," and "cat" may have similar meanings because all are related to animals. On the other hand, words like "car" or "skateboard" are different because they belong to another category.

Embeddings allow the model to understand not only the word itself but also its context. This is important because the same word can have different meanings in different sentences.

For example:

“The bank is near the river.”

Here, “bank” means the side of a river.

“I deposited money in the bank.”

Here, “bank” means a financial institution.

The model uses context to understand the correct meaning.

## Transformer Model

Modern Large Language Models use a technology called a transformer. A transformer helps the model understand the relationship between words in a sentence.

The transformer uses a technique called attention. Attention helps the model focus on the most important words in a sentence, as shown in Figure 3.

Figure 3: Transformer architecture showing how input text is converted into embeddings, processed by a decoder, and generated as output text.

For example, in the sentence:

“I heard a dog bark.”

The words "heard" and "dog" are important for understanding the word "bark." The model gives more attention to these words because they provide strong clues about the meaning.

This attention mechanism allows the model to understand context and generate accurate responses. It helps the model decide which words are more important and how they are related to each other.

Transformers are very powerful because they can process long sentences, understand complex relationships, and generate human-like answers.

## Prompts

A prompt is the input given to an AI model, as shown in Figure 4. It may be a question, command, instruction, or statement. The model reads the prompt and generates a response.

Figure 4: Comparison between a good prompt and a bad prompt based on clarity, specificity, context, and details.

For example:

“Explain Generative AI in simple words.”

This is a prompt because it tells the AI model what to do.

The quality of the prompt directly affects the quality of the response. A clear and specific prompt usually produces a better answer. A vague prompt may produce a general or unclear answer.

For example:

Weak prompt:

“Tell me about AI.”

Better prompt:

“Explain Artificial Intelligence in five simple points for beginner-level students.”

The second prompt is better because it clearly mentions the topic, format, and audience.

## Types of Prompts

There are mainly two types of prompts:

## 1. System Prompt

A system prompt sets the behavior, tone, role, and rules of the AI model. It is usually written by the application developer.

Example:

“You are a helpful assistant. Explain answers in a simple and friendly manner.”

This tells the model how it should behave while answering.

## 2. User Prompt

A user prompt is the actual question or instruction given by the user.

Example:

“Summarize the topic of AI agents in simple language.”

The user prompt tells the model what specific task it should perform.

## Difference Between System Prompt and User Prompt

System Prompt

User Prompt

Defines the behavior of the model

Gives a specific question or instruction

Usually written by the application developer

Written by the user

Controls tone, style, and rules

Controls the task to be completed

Example: “You are a helpful assistant.”

Example: “Explain Generative AI.”

##

## Conversation History

Generative AI applications often use conversation history to maintain context. Conversation history means the previous messages exchanged between the user and the AI model.

For example, if a user first asks the following:

“What is Generative AI?”

and then asks:

“What are its advantages?”

The model understands that the word “its” refers to Generative AI. This happens because the model uses previous conversation history as context.

Conversation history makes AI interactions more natural. It allows users to ask follow-up questions without repeating the full topic again.

## Retrieval-Augmented Generation

Retrieval Augmented Generation, or RAG, is a technique used to improve the accuracy of AI responses as shown in Figure 5. In this method, the AI system retrieves relevant information from documents, databases, emails, websites, or search engines and adds that information to the prompt.

Figure 5: Retrieval-Augmented Generation process showing how a user query is searched in data sources to retrieve relevant information and generate an enriched answer.

Without RAG, the AI model may give a general answer based on its training. With RAG, the model can give a more specific and accurate answer based on the retrieved information.

For example, if a user asks the following:

“What is the maximum travel allowance in my company?”

A normal AI model may answer the following:

“Please check your company travel policy.”

But a RAG-based system first searches the company travel policy document, finds the relevant section, and then gives the correct answer based on that document.

RAG is useful because it grounds the response in real information. It reduces the chances of incorrect or imaginary answers.

## AI Agents

AI agents are advanced AI systems that can not only answer questions but also perform actions. They are built using Generative AI and can use tools to complete tasks.

An AI agent can understand instructions, make decisions, use tools, and act according to the situation. For example, an AI agent may search the internet, summarize information, create an email, update a calendar, or retrieve information from a database.

AI agents have three main components:

Component

Explanation

Large Language Model

Acts as the brain of the agent

Instructions

Define the role and behavior of the agent

Tools

Help the agent perform actions

The Large Language Model helps the agent understand language and reason over information. Instructions tell the agent what role it should follow. Tools allow the agent to interact with the outside world.

## Multi-Agent Systems

Sometimes, more than one AI agent can work together. This is called a multi-agent system.

In a multi-agent system, different agents may have different responsibilities. One agent may collect data, another may analyze it, and another may take action. Together, they can complete complex workflows.

For example, in a business system:

One agent may collect customer feedback.

Another agent may analyze the feedback.

A third agent may create a report.

A fourth agent may send the report by email.

This makes multi-agent systems useful for automation and complex problem-solving.

## Codes:

## 1. Tokenization: breaking a sentence into words

## text = "I love artificial intelligence"

## tokens = text.split()

## print(tokens)

##

“We divide the sentence into smaller pieces.” This is a simple word split; actual LLM tokenizers may split words further.

## 2. Token IDs: assigning numbers to tokens

## tokens = ["I", "love", "AI"]

## vocabulary = {"I": 0, "love": 1, "AI": 2}

## for token in tokens:

##     print(token, "=", vocabulary[token])

“Each token has an ID. The ID identifies the token; it does not represent its meaning.”

## 3. Next-word prediction: choosing the most frequent word

## # Words observed after "I drink"

## examples = ["tea", "coffee", "tea"]

## prediction = max(examples, key=examples.count)

## print("I drink", prediction)

“Tea appears most often, so this program predicts tea.” An LLM uses a trained neural network rather than this counting rule.

## 4. Embeddings: representing words with lists of numbers

## import numpy as np

## # Manually assigned teaching vectors

## # Dimensions roughly represent: animal-related, vehicle-related

## embeddings = {

##     "dog": np.array([1.0, 0.1]),

##     "puppy": np.array([0.9, 0.1]),

##     "car": np.array([0.1, 1.0])

## }

## def similarity(a, b):

##     return np.dot(a, b) / (np.linalg.norm(a) * np.linalg.norm(b))

## print("Dog and puppy:",

##       round(similarity(embeddings["dog"], embeddings["puppy"]), 3))

## print("Dog and car:",

##       round(similarity(embeddings["dog"], embeddings["car"]), 3))

Similar vectors point in similar directions, producing a higher cosine similarity.

## 5. Prompts: giving instructions

## system_prompt = "You are a teacher. Use simple language."

## user_prompt = "Explain AI in two sentences."

## print("SYSTEM:", system_prompt)

## print("USER:", user_prompt)

## “The system message sets the behavior. The user message gives the task.”

## 6. Conversation history: keeping previous messages

## history = [

##     "User: What is AI?",

##     "Assistant: AI means Artificial Intelligence.",

##     "User: Give me an example of it."

## ]

## for message in history:

##     print(message)

## “Providing earlier messages helps a model identify what ‘it’ refers to.” This code stores and displays the conversation.

##

## 7. RAG: finding information before answering

## # Sample college document

## document = "Students must maintain at least 75% attendance."

## # Student's question

## question = "What is the minimum attendance required?"

## # Retrieve the relevant information

## context = document

## # Prepare the prompt for an AI model

## prompt = f"""

## Answer the question using the information below.

## Information: {context}

## Question: {question}

## """

## print(prompt)

##

## RAG first retrieves relevant information, then gives it to an LLM with the question.

## 8.Tool use: a simple rule-based assistant

## # Tool

## def calculate_average(numbers):

##     return sum(numbers) / len(numbers)

## # User request

## request = "Calculate the average of these marks"

## marks = [72, 85, 91]

## print("User request:", request)

## # A fixed rule selects the tool

## if "average" in request.lower():

##     print("Selected tool: calculate_average")

##     result = calculate_average(marks)

##     print("Tool result:", result)

##     print(f"Assistant: The average mark is {result:.2f}.")

## else:

##     print("No suitable tool available.")

## The assistant calls a function to perform a task and uses its result in the response.

## 9. Single agent: selects an action

## def agent(task):

##     if task == "greet":

##         return "Hello, student!"

##     elif task == "add":

##         return 5 + 3

##     else:

##         return "I cannot do this task."

## print(agent("greet"))

## print(agent("add"))

## “We give a task, and the agent selects an action. Here, fixed rules control its choice.”

## 10. Multiple agents: divide the work

## # Agent 1 adds the numbers

## def agent1(a, b):

##     return a + b

## # Agent 2 prepares a message

## def agent2(answer):

##     return f"The answer is {answer}"

## # Agent 1 passes its result to Agent 2

## result = agent1(5, 3)

## message = agent2(result)

## print(message)

## “Agent 1 calculates. Agent 2 presents the answer. They complete the task together by passing information.”

## Practice Task Questions

- Write a Python program to display a simple prompt and its AI-generated completion.

- Write a Python program to take a sentence from the user and divide it into tokens using the split() function.

- Write a Python program to count the total number of tokens present in a given sentence.

- Write a Python program to assign a unique token ID to each word in a sentence.

- Write a Python program to show the difference between a good prompt and a bad prompt.

- Write a Python program to predict the next word in a sentence using simple if-else conditions.

- Write a Python program to create a small dictionary of AI-related topics such as Generative AI, LLM, RAG, and AI Agent.

- Write a Python program to retrieve relevant information from the dictionary based on a user question, showing a basic RAG concept.

- Write a Python program to create a simple AI agent that selects a tool, such as a search engine or calculator, based on the user request.

- Write a Python program to display the final conclusion of the experiment explaining prompts, tokenization, RAG, and AI agents.

Video Links

Generative AI Full Course 2026: From LLM Basics to RAG

Learn RAG From Scratch – Python AI Tutorial

Improve your Generative AI Application with RAG

How to Build a Production-Ready RAG AI Agent in Python

Build Your First RAG Application with LLMs

## Additional Resources

- Google Cloud Skills Boost – Introduction to Generative AI

URL: https://www.skills.google/course_templates/536

- Google Cloud – Introduction to Generative AI Learning Path

URL: https://www.skills.google/paths/118

- Google Cloud – Generative AI Resources

URL: https://cloud.google.com/ai/generative-ai

- IBM – What is Generative AI?

URL: https://www.ibm.com/think/topics/generative-ai

- IBM – What is Retrieval Augmented Generation?

URL: https://www.ibm.com/think/topics/retrieval-augmented-generation

- IBM – What Are AI Agents?

URL: https://www.ibm.com/think/topics/ai-agents

- Coursera – Introduction to Generative AI by Google Cloud

URL: https://www.coursera.org/learn/introduction-to-generative-ai

- Coursera – IBM RAG and Agentic AI Professional Certificate

URL: https://www.coursera.org/professional-certificates/ibm-rag-and-agentic-ai

- edX – Mastering Generative AI: Agents with RAG and LangChain

URL: https://www.edx.org/learn/computer-science/ibm-mastering-generative-ai-agents-with-rag-and-langchain

- IBM Video Resource – What is Retrieval-Augmented Generation?

URL: https://mediacenter.ibm.com/media/What%2Bis%2BRetrieval-Augmented%2BGeneration%2B%28RAG%29/1_4huqwyq1

## Text Books

- Generative AI Foundations in Python

PDF URL: https://d15k2d11r6t6rl.cloudfront.net/pub/40qd/gy9g2422/rk0/66s/hxt/Free%20PDF%20-%20Generative%20AI%20Foundations%20in%20Python.pdf

Useful for: Generative AI basics, LLMs, Python examples.

- Foundations of Large Language Models

PDF/Book Page URL: https://arxiv.org/abs/2501.09223

Useful for: LLM foundations, pre-training, prompting, alignment, inference.

- Information Retrieval and Retrieval-Augmented Generation

PDF URL: https://web.stanford.edu/~jurafsky/slp3/11.pdf

Useful for: RAG, retrieval, document search, question answering.

- Hands-On Large Language Models

PDF URL: https://elibrary-dev.nusamandiri.ac.id/assets/fileebook/250153.pdf

Useful for: Practical LLM understanding, diagrams, embeddings, transformers, and applications.

- Prompt Engineering Guide / Lecture Material

PDF URL: https://github.com/dair-ai/Prompt-Engineering-Guide/blob/main/lecture/Prompt-Engineering-Lecture-Elvis.pdf

Useful for: Prompting techniques, LLM use cases, and prompt design.

## Reference Books

- Prompt Engineering – Google Whitepaper by Lee Boonstra

PDF URL: https://www.gptaiflow.com/assets/files/2025-01-18-pdf-1-TechAI-Goolge-whitepaper_Prompt%20Engineering_v4-af36dcc7a49bb7269a58b1c9b89a8ae1.pdf

Useful for: Prompt engineering, prompt structure, and LLM output improvement.

- A Practical Guide to Building Agents – OpenAI

PDF URL: https://cdn.openai.com/business-guides-and-resources/a-practical-guide-to-building-agents.pdf

Useful for: AI agents, agent design, tools, orchestration, and safety.

- RAG Meets LLM: Towards Retrieval-Augmented Large Language Models

PDF URL: https://advanced-recommender-systems.github.io/RAG-Meets-LLMs/2024-KDD-RAG-Meets-LLM-tutorial-Part1.pdf

Useful for: RAG architecture, retrieval-based LLM systems, and advanced RAG concepts.

- Prompt Engineering – IIT Delhi Lecture Notes

PDF URL: https://www.cse.iitd.ac.in/~mausam/courses/col772/spring2023/lectures/22-promptengg.pdf

Useful for: Academic explanation of prompt engineering and language model usage.

- Free AI Agents Resources – GitHub Collection

URL: https://github.com/avinash201199/free-ai-agents-resources

Useful for: AI agents, autonomous agents, LLM-powered agents, and multi-agent systems.

---


## 🖥️ PRESENTATION SLIDES


# Experiment-2.2 - All Lecture Slides Text


## Exp 2.2
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
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 2                   Experiment No.2.2
- Topic
- : Understanding Azure Machine Learning, Generative AI Models, and AI Agent
- Systems
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning
- Objectives
- To understand the basic concept of Generative Artificial Intelligence and its role in creating new content
- .
- To
- learn the meaning of prompts and understand the difference between system prompts and user prompts
- .
- To
- understand the basic working of Large Language Models, including tokens,
- embedding's,
- transformers, and attention
- .
- To
- explore the concept of Retrieval Augmented Generation and how it improves AI responses
- .

### Slide 3
- Recap
- of Previous Experiment
- Artificial Intelligence enables machines to perform intelligent tasks such as learning, reasoning, decision-making, understanding language, and solving real-world problems.
- Generative AI, NLP, Speech AI, Computer Vision, and OCR help machines create content, process text, understand voice, analyze images, and extract useful information from documents.
- Responsible AI ensures that AI systems are developed and used in a safe, fair, transparent, secure, inclusive, and ethical manner.

### Slide 4
- Topic 1. Generative Artificial
- Intelligence
- Topic 2. Prompts and Prompt
- Types
- Topic 3. Large Language
- Models
- Topic 4. Retrieval Augmented
- Generation
- Topic 5. AI Agents
- Figure-1 :
- Introduction to Generative AI
- Source :
- https://cogentinfo.com/resources/the-role-of-generative-
- ai
- -in-the-modern-workplace#
- Introduction to Generative AI

### Slide 5
- Figure-2:Generative Artificial Intelligence
- Source:
- https://www.webcluesinfotech.com/what-is-generative-ai-everything-you-need-to-know/
- Generative Artificial Intelligence
- Generative Artificial Intelligence is a branch of artificial intelligence that can create new content such as text, images, audio, video, summaries, stories, poems, and computer code
- .
- It is called “generative” because it generates new output based on the input provided by the user
- .
- It
- is widely used in education, business, research, programming, customer support, and content creation.

### Slide 6
- A prompt is the input given to a Generative AI model to receive a response
- .
- A prompt can be a question, command, instruction, statement, or casual message
- .
- A
- clear and specific prompt helps the model generate better and more accurate responses
- .
- Example of a simple prompt:
- Explain Artificial Intelligence in simple words.
- Example of a better prompt:
- Explain Artificial Intelligence in five simple points for beginner-level students.
- Figure-3
- :Prompt Engineering
- Source:
- https://www.linkedin.com/pulse/what-prompt-engineering-why-useful-generative-ai-models-cloudkitect-hbldc/
- Prompts in Generative AI

### Slide 7
- There are two main types of prompts in Generative AI:
- System Prompt:
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>A system prompt defines the behavior, role, tone, and rules of the AI model. It is usually written by the application developer.
- Example:
- You are a helpful assistant. Explain all answers in simple and friendly language.
- User Prompt:
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>A user prompt is the actual question or instruction given by the user.
- Example:
- Summarize the topic of AI agents in simple language.
- Figure-4
- :Types of Prompts
- Source:
- https://hatchworks.com/blog/gen-
- ai
- /generative-
- ai
- -prompt-guide/
- Types of Prompts

### Slide 8
- A Large Language Model, also called an LLM, is the core technology behind many Generative AI systems
- .
- They
- generate responses by predicting the next most suitable word or token based on the given prompt
- .
- For
- example, if the input is:
- I heard a dog...
- The model may predict:
- bark
- This happens because the model has learned that dogs commonly bark.
- Figure-5
- :Large Language Models
- Source:
- https://otrs.com/blog/
- ai
- -automation/large-language-models-
- llms
- /
- Large Language Models

### Slide 9
- Tokenization is the process of breaking text into smaller units called tokens.
- Tokens may be complete words, parts of words, punctuation marks, or characters.
- Example:
- Sentence:
- I heard a dog bark loudly.
- Tokens:
- I, heard, a, dog, bark,
- loudly
- After
- tokenization, tokens are converted into numerical vectors called
- embedding's.
- Embedding's
- help the model understand the meaning and relationship between words
- .
- For example, the words
- dog
- ,
- puppy
- , and
- cat
- may be closer in meaning than
- dog
- and
- car
- .
- Figure-6
- :Tokenization and Embedding's
- Source:
- https://airbyte.com/data-engineering-resources/tokenization-
- vs
- -
- embeddings
- Tokenization and
- Embedding's

### Slide 10
- A
- transformer helps the model understand relationships between tokens in a sentence
- .
- The transformer uses a technique called attention.
- Attention helps the model focus on important words in the input
- .
- For example, in the sentence:
- I heard a dog bark
- The words
- heard
- and
- dog
- are important for understanding the word
- bark
- .
- Because of attention, the model can understand context and generate meaningful responses.
- Figure-7 :Attention
- Mechanism
- Source:
- https://www.linkedin.com/pulse/attention-mechanism-secret-behind-how-transformers-satishkumar-80cfc/
- Transformer and Attention Mechanism

### Slide 11
- Retrieval Augmented Generation, or RAG, is a technique used to improve AI responses by adding relevant external information.
- In RAG, the AI system first retrieves useful information from documents, databases, emails, websites, or search engines.
- Then the retrieved information is added to the prompt so that the AI model can generate a more accurate answer.
- Example
- :
- User question:
- What is the maximum travel allowance in my company?
- A RAG-based system searches the company policy document and answers using that document.
- Figure-8 :Retrieval Augmented Generation
- Source:
- https://bradsol.com/resources/blogs/retrieval-augmented-generation-rag-for-llms-a-guide-to-enhanced-accuracy-and-trust/
- Retrieval Augmented Generation

### Slide 12
- AI agents are software applications built using Generative AI.
- They can understand instructions, reason over information, use tools, and perform actions
- .
- For
- example, an AI agent can search information, summarize a document, draft an email, update a calendar, or retrieve data from a database
- .
- AI agents have three main components:
- Large Language Model:
- Acts as the brain of the agent.
- Instructions:
- Define the role, behavior, and rules of the agent.
- Tools:
- Help the agent interact with the world and perform actions.
- Figure-9
- :
- AI Agents
- Source:
- https://builder.aws.com/content/30PvUImLL3LehFlOZpZ5SU6Bavn/agentic-ai-series-part-1-what-are-ai-agents-and-why-do-they-matter
- AI Agents

### Slide 13
- A multi-agent system is a system where multiple AI agents work together to complete complex tasks
- .
- Each agent may have a different role or specialization
- .
- For example:
- One agent may collect data.
- Another agent may analyze the data.
- Another agent may prepare a report.
- Another agent may send the report by email.
- Figure-10 :Multi-Agent Systems
- Source:
- https://www.geeksforgeeks.org/artificial-intelligence/multiagent-planning-in-ai/
- Multi-Agent Systems

### Slide 14
- Summary of the
- Experiment
- Generative AI can create new content such as text, images, audio, video, and code
- .
- Prompts are inputs given to AI models, and better prompts produce better responses
- .
- Large Language Models process language using tokens,
- embedding's,
- transformers, and attention mechanisms
- .
- Retrieval Augmented Generation improves AI responses by retrieving relevant external information
- .

### Slide 15
- Next
- Experiment
- T
- opic(s)
- Topic 1:
- Introduction to Text
- Analysis
- Topic 2:
- Tokenization and Text
- Preprocessing
- Topic 3:
- Statistical Text
- Analysis
- Topic 4:
- Semantic Language Models

### Slide 16
- Quiz/ FAQ’s
- What is Generative AI
- ?
- What
- is a prompt
- ?
- What
- is the difference between a system prompt and a user prompt
- ?
- What
- is a Large Language Model
- ?
- What
- is tokenization
- ?
- What
- are
- embedding's?
- What
- is transformer architecture
- ?
- What
- is Retrieval Augmented Generation
- ?

### Slide 17
- R
- eferences/ Articles/ Videos
- Reference / Articles
- Google Cloud – Generative AI Resources
- https://cloud.google.com/ai/generative-ai
- IBM – What is Generative AI?
- https://www.ibm.com/think/topics/generative-ai
- IBM – What is Retrieval Augmented Generation?
- https://www.ibm.com/think/topics/retrieval-augmented-generation
- IBM – What Are AI Agents?
- https://
- www.ibm.com/think/topics/ai-agents
- Videos
- Generative AI Full Course 2026: From LLM Basics to RAG
- https://www.youtube.com/watch?v=ofGKKLVTM9o
- Learn RAG From Scratch – Python AI Tutorial
- https://www.youtube.com/watch?v=sVcwVQRHIc8

### Slide 18
- Additional
- learning
- R
- esources
- Additional Resources for Learning Generative AI
- https://www.skills.google/course_templates/536
- https://
- www.coursera.org/learn/introduction-to-generative-ai
- Additional Resources for Learning RAG and AI Agents
- https://www.ibm.com/think/topics/retrieval-augmented-generation
- https://
- www.ibm.com/think/topics/ai-agents
- Additional Resources for Prompt Engineering
- https://github.com/dair-ai/Prompt-Engineering-Guide

### Slide 19
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 20
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in


---


================================================================================


# Experiment-2.3 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-2.3
# Experiment-2.3

## Exploring Generative AI , Natural Language Processing, and Azure AI tools.

##      CO4

##

## Aim

To study and implement the basic concepts of Text Analysis using Natural Language Processing, including tokenization, text normalization, stop word removal, stemming, lemmatization, POS tagging, frequency analysis, TF-IDF, bag-of-words, TextRank, and semantic language models.

## Objectives

The objectives of this experiment are:

- To understand the meaning and importance of text analysis in Artificial Intelligence.

- To learn how unstructured text is converted into meaningful structured information.

- To perform tokenization on a given text corpus.

- To apply text preprocessing techniques such as normalization, stop word removal, stemming, and lemmatization.

- To understand statistical text analysis using frequency analysis and TF-IDF.

- To understand bag-of-words representation for machine learning.

- To study TextRank for text summarization and keyword extraction.

- To understand semantic language models, embeddings, and cosine similarity.

- To identify real-world applications of NLP-based text analysis.

## Theory

## Introduction to Text Analysis

Text analysis is a part of Natural Language Processing, also called NLP. NLP is a branch of Artificial Intelligence that helps computers understand, process, and analyze human language as shown in Figure 1.

Figure 1: Common NLP tasks, including speech recognition, speech tagging, word sense disambiguation, named entity recognition, coreference resolution, and natural language generation.

Most real-world data is available in unstructured form, such as emails, reviews, social media posts, contracts, news articles, support tickets, and documents. Since this data is not arranged in rows and columns like a database, computers cannot directly understand it. Text analysis helps convert this unstructured text into useful information.

For example, a company may receive thousands of customer reviews. By using text analysis, the company can find whether customers are happy or unhappy, what products are being discussed, and what common complaints are appearing.

Common uses of text analysis include:

Use Case

Meaning

Language detection

Identifying the language of the text

Key term extraction

Finding important words or phrases

Entity detection

Finding names of people, places, dates, and organizations

PII detection

Detecting sensitive information like phone numbers or addresses

Text classification

Categorizing text into classes

Sentiment analysis

Finding whether text is positive, negative, or neutral

Text summarization

Creating a short summary from a large text

Text analysis is challenging because human language is complex. The same word can have different meanings in different contexts. For example, the word banks can refer to financial institutions or the sides of a river. This is why NLP techniques are required to extract meaning from text. The provided module explains text analysis as an NLP subset used to extract meaning, structure, and insights from unstructured text.

## Tokenization

## Meaning of Tokenization

Tokenization is the first step in text analysis. It means breaking a sentence, paragraph, or document into smaller units called tokens.

Usually, tokens are words, but they can also be punctuation marks, subwords, or phrases.

## Example

Sentence:

## We choose to go to the moon

Tokens:

## We

choose

to

go

to

the

moon

Here, the sentence is broken into individual words. Each word is treated as a token.

## Importance of Tokenization

Tokenization is important because computers cannot directly understand full sentences. By breaking text into smaller tokens, we can count words, remove unnecessary words, find important terms, and prepare text for machine learning models.

## Text Preprocessing Techniques

Before applying machine learning or text analysis, text must be cleaned and prepared. This process is called text preprocessing, as shown in Figure 2.

Figure 2: Text preprocessing techniques such as tokenization, lowercasing, stopword removal, punctuation removal, stemming, lemmatization, spelling correction, and normalization.

## Text Normalization

Text normalization means converting text into a standard format.

It may include:

- Converting words to lowercase.

- Removing punctuation.

- Removing special characters.

- Removing extra spaces.

## Example

Original text:

## Artificial Intelligence is Powerful!

Normalized text:

## artificial intelligence is powerful

## Importance

Normalization helps reduce duplicate forms of the same word. For example, AI, ai, and Ai may be treated as different words unless they are normalized.

However, sometimes normalization may remove useful meaning. For example, Mr. Banks as a person and banks as financial institutions may need to be treated differently.

## Stop Word Removal

Stop words are common words that usually do not carry strong meaning.

Examples:

## the, is, am, are, a, an, it, of, and, to

## Example

Sentence:

## AI is transforming the world.

After stopword removal:

## AI transforming world

## Importance

Stopword removal helps reduce noise and keeps only meaningful words for analysis.

## N-Gram Extraction

An n-gram is a group of one or more words appearing together.

Type

Meaning

Example

Unigram

One word

artificial

Bigram

Two words

artificial intelligence

Trigram

Three words

natural language processing

##

## Importance

Sometimes a group of words has more meaning than individual words.

For example:

## artificial intelligence

natural language processing

machine learning

These phrases should be understood together rather than as separate words.

## Stemming

Stemming is the process of reducing words to their root form by cutting word endings.

## Example

## playing → play

played → play

player → play

Another example:

## powering, powered, powerful → power

## Limitation

Stemming may produce words that are not valid dictionary words.

Example:

## intelligence → intellig

So, stemming is fast but not always accurate.

## Lemmatization

Lemmatization also converts words into their base form, but it uses grammar and vocabulary rules.

## Example

## running → run

businesses → business

experiences → experience

## Difference between Stemming and Lemmatization

Stemming

Lemmatization

Cuts word endings

Uses grammar rules

Faster

More accurate

May produce invalid words

Produces valid dictionary words

Example: intelligence → intellig

Example: running → run

## Parts of Speech Tagging

Parts of Speech tagging, also called POS tagging, means identifying the grammatical category of each word.

Examples of POS tags:

POS

Meaning

Noun

Name of person, place, thing

Verb

Action word

Adjective

Describing word

Adverb

Modifies verb/adjective

Pronoun

Replaces noun

##

## Example

Sentence:

## AI improves business performance.

POS tagging:

## AI → Noun

improves → Verb

business → Noun

performance → Noun

POS tagging helps the computer understand the role of each word in a sentence.

## Statistical Text Analysis

After tokenization and preprocessing, statistical methods can be used to understand text.

## Frequency Analysis

Frequency analysis means counting how many times each word appears in a document.

## Example

Text:

## AI improves business. AI improves decision-making.

Frequency table:

Term

Frequency

AI

2

improves

2

business

1

decision-making

1

##

## Importance

Words that appear frequently often indicate the main topic of the document.

For example, if words like AI, business, customer, and decision appear many times, the document is probably about AI in business.

Frequency analysis is useful for identifying the most common words in a document, but it may not always show the most meaningful words because common words may appear in many documents.

## TF-IDF

TF-IDF stands for "Term Frequency-Inverse Document Frequency."

It is used to find important words in a document compared to a group of documents.

## Term Frequency

Term Frequency means how many times a word appears in a document.

Formula:

## TF = Number of times a term appears in a document

Example:

If the word "agent" appears 6 times, then:

## TF(agent) = 6

## Inverse Document Frequency

Inverse Document Frequency checks whether a word is common or rare across all documents.

Formula:

## IDF(t) = log(N / df(t))

Where:

Symbol

Meaning

N

Total number of documents

df(t)

Number of documents containing term t

If a word appears in every document, it is not very special. If it appears in only one document, it becomes more important.

## TF-IDF Formula

## TF-IDF = TF × IDF

A high TF-IDF score means the word is important in one document but not common in all documents.

## Example

Suppose there are two documents:

Document A talks about Copilot Studio.

Document B talks about Microsoft Foundry.

Common words like AI, Microsoft, and agent may appear in both documents. So, they are not useful for distinguishing the documents.

But words like:

## copilot

studio

declarative

may be important for Document A.

Words like:

## foundry

code

develop

may be important for Document B.

Therefore, TF-IDF helps identify the special terms of each document. The provided module explains that TF-IDF gives high importance to words that appear frequently in one document but rarely across other documents.

## Bag-of-Words Model

Bag-of-Words is a text representation technique. It represents text as a collection of word counts.

In this model, grammar and word order are ignored. Only the presence or frequency of words is considered.

## Example

Sentence 1:

## AI improves business

Sentence 2:

## AI improves learning

Vocabulary:

## AI, improves, business, learning

Bag-of-words representation:

Sentence

AI

improves

business

learning

Sentence 1

1

1

1

0

Sentence 2

1

1

0

1

##

## Importance

Bag-of-words is useful for machine learning tasks such as:

- Spam detection.

- Sentiment analysis.

- Topic classification.

- Document categorization.

## Example Use Case

In spam email detection, words like

## free

winner

lottery

miracle cure

lose weight fast

may appear more frequently in spam emails. A machine learning model can use these words to classify emails as spam or not spam.

## TextRank

TextRank is an unsupervised graph-based algorithm used for text summarization and keyword extraction.

It is inspired by Google’s PageRank algorithm.

## TextRank for Summarization

In TextRank, each sentence is treated as a node in a graph. Connections between sentences are called edges. These edges are based on similarity between sentences.

## Steps in TextRank

- Split the document into sentences.

- Treat each sentence as a node.

- Calculate similarity between sentences.

- Create edges between similar sentences.

- Rank the sentences.

- Select the highest-ranked sentences as the summary.

## Example Text

## Cloud computing provides on-demand access to computing resources.

Computing resources include servers, storage, and networking.

Azure is Microsoft's cloud computing platform.

Organizations use cloud platforms to reduce infrastructure costs.

Cloud computing enables scalability and flexibility.

Important sentences may be:

## Cloud computing provides on-demand access to computing resources.

Azure is Microsoft's cloud computing platform.

Cloud computing enables scalability and flexibility.

So, the summary becomes:

## Cloud computing provides on-demand access to computing resources.

Azure is Microsoft's cloud computing platform.

Cloud computing enables scalability and flexibility.

This is called extractive summarization because the summary is created by selecting original sentences from the document.

TextRank can also be used for keyword extraction, where words are treated as nodes and important words are selected as keywords.

## Semantic Language Models

Older NLP methods mainly used word counts and statistics. Modern NLP uses semantic language models.

Semantic models try to understand the meaning of words and sentences.

## Word Embeddings

Word embeddings represent words as vectors.

A vector is a list of numbers.

Example:

Word

Vector

dog

[0.8, 0.6, 0.1]

cat

[0.7, 0.5, 0.2]

tree

[0.2, 0.1, 0.9]

Words with similar meanings have similar vector directions.

For example:

## dog and cat

are more similar than:

## dog and tree

because dog and cat are both animals.

The uploaded module explains that embeddings are multi-valued arrays of numbers that encode semantic relationships between tokens.

## Cosine Similarity

Cosine similarity is used to measure similarity between two vectors.

Formula:

## cosine similarity = A · B / ||A|| × ||B||

Where:

Symbol

Meaning

A · B

Dot product of vectors

If cosine similarity is close to 1, the words are highly similar.

If it is close to 0, the words are not very similar.

## Example

The similarity between dog and cat may be high because both are animals.

The similarity between dog and tree may be low because they belong to different categories.

## Vector Arithmetic

Semantic models can also perform vector operations.

Example:

## dog + young = puppy

cat + young = kitten

This means the model understands the relationship between adult animals and young animals.

Another example:

## kitten - puppy + dog = cat

This shows analogy-based reasoning.

## Contextual Embeddings

Modern models such as GPT use contextual embeddings. This means the meaning of a word is understood based on its surrounding words.

Example:

## I deposited money in the bank.

Here, bank means financial institution.

## The children sat near the river bank.

Here, bank means side of a river.

Contextual embeddings help models understand the correct meaning based on context.

Code

# Install necessary libraries

!pip install transformers datasets torch

# Import required libraries

import pandas as pd

import torch

from transformers import AutoTokenizer, AutoModelForSequenceClassification, pipeline

from datasets import Dataset

# Load sample dataset (you can upload your CSV file in Colab later)

# Simulating a tweet dataset

data = {

"tweet": [

"I love AI! It's making life so much easier.",

"I hate traffic jams. They ruin my mood.",

"This new phone is amazing! Best purchase ever.",

"I am feeling neutral about today's meeting.",

"Why is the internet so slow? It's frustrating."

]

}

# Save the dataset as a CSV file

tweet_df = pd.DataFrame(data)

tweet_df.to_csv("tweets.csv", index=False)

print("Sample dataset created: tweets.csv")

# Load the dataset into a DataFrame

df = pd.read_csv("tweets.csv")

print("Loaded dataset:")

print(df)

# Load pre-trained BERT model and tokenizer

model_name = "distilbert-base-uncased-finetuned-sst-2-english"

tokenizer = AutoTokenizer.from_pretrained(model_name)

model = AutoModelForSequenceClassification.from_pretrained(model_name)

# Create a sentiment analysis pipeline

sentiment_pipeline = pipeline("sentiment-analysis", model=model, tokenizer=tokenizer)

# Perform sentiment analysis on the tweets

results = sentiment_pipeline(df["tweet"].tolist())

# Convert results to a DataFrame

results_df = pd.DataFrame(results)

df["label"] = results_df["label"]

df["score"] = results_df["score"]

# Display results

print("Sentiment Analysis Results:")

print(df)

# Save the results to a CSV file

df.to_csv("sentiment_analysis_results.csv", index=False)

print("Results saved to sentiment_analysis_results.csv")

# Visualize results

import seaborn as sns

import matplotlib.pyplot as plt

sns.countplot(data=df, x="label", palette="viridis")

plt.title("Sentiment Distribution")

plt.show()

##

##

## Practical Task Questions

- Write a Python program to perform tokenization on a given paragraph and display all tokens.

- Write a Python program to convert a given text into lowercase and remove all punctuation marks.

- Write a Python program to remove stop words from a given paragraph using the NLTK library.

- Write a Python program to perform stemming on the following words:

playing, played, player, studies, studying, powerful

- Write a Python program to perform lemmatization on a list of words and compare the output with stemming.

- Write a Python program to apply Part-of-Speech tagging to a sentence and identify nouns, verbs, and adjectives.

- Write a Python program to count the frequency of each word in a given text corpus.

- Write a Python program to create a Bag-of-Words model for three short documents.

- Write a Python program to calculate TF-IDF values for multiple text documents and display the important terms.

- Write a Python program to generate a simple extractive summary by selecting the most important sentences from a paragraph.

## Video Links

Basic Preprocessing—Case Folding, Stopword Removal, Stemming and Lemmatization

Natural Language Processing - Tokenization

Stemming and Lemmatization

Introduction to NLP | Bag of Words Model

Text Representation Using TF-IDF

## Additional Resources

- NLTK Official Documentation

URL: https://www.nltk.org/

Useful for tokenization, stemming, tagging, parsing, and text classification.

- NLTK Book — Natural Language Processing with Python

URL: https://www.nltk.org/book/

Useful for learning NLP basics with Python examples.

- Scikit-learn: Feature Extraction Documentation

URL: https://scikit-learn.org/stable/modules/feature_extraction.html

Useful for text feature extraction, Bag-of-Words, and TF-IDF.

- Scikit-learn: Working with Text Data

URL: https://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html

Useful for text classification and practical NLP pipelines.

- Scikit-learn: TfidfVectorizer Documentation

URL: https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html

Useful for converting text documents into TF-IDF feature matrices.

- GeeksforGeeks: Text Preprocessing in NLP

URL: https://www.geeksforgeeks.org/nlp/text-preprocessing-for-nlp-tasks/

Useful for tokenization, stopword removal, stemming, lemmatization, and POS tagging.

- Sanfoundry: Text Preprocessing in NLP

URL: https://www.sanfoundry.com/text-preprocessing-in-nlp-tokenization-stemming-lemmatization/

Useful for basic explanation and Python workflow of NLP preprocessing.

- RPI: Bag-of-Words Using Scikit-learn

URL: https://pages.github.rpi.edu/kuruzj/website_introml_rpi/notebooks/08-intro-nlp/03-scikit-learn-text.html

Useful for understanding Bag-of-Words with Scikit-learn.

- ResearchGate: An Interpretation of Lemmatization and Stemming in NLP

URL: https://www.researchgate.net/publication/348306833_An_Interpretation_of_Lemmatization_and_Stemming_in_Natural_Language_Processing

Useful for theoretical understanding of stemming and lemmatization.

- Dev.to: Complete Guide to NLP Text Preprocessing

URL: https://dev.to/themustaphatijani/the-complete-guide-to-nlp-text-preprocessing-tokenization-normalization-stemming-lemmatization-50ap

Useful for tokenization, normalization, stemming, and lemmatization examples.

## Textbooks

- Natural Language Processing with Python — Steven Bird, Ewan Klein, Edward Loper

URL: https://www.nltk.org/book/

- Speech and Language Processing, 3rd Edition — Daniel Jurafsky and James H. Martin

URL: https://web.stanford.edu/~jurafsky/slp3/

- Introduction to Information Retrieval — Christopher D. Manning, Prabhakar Raghavan, Hinrich Schütze

URL: https://nlp.stanford.edu/IR-book/pdf/irbookonlinereading.pdf

- Foundations of Statistical Natural Language Processing — Christopher D. Manning and Hinrich Schütze

URL: https://nlp.stanford.edu/fsnlp/

- Deep Learning for Natural Language Processing: A Gentle Introduction — Michael Roth, Mihai Surdeanu, and others

URL: https://clulab.org/gentlenlp/book/gentlenlp-book-12232022.pdf

## Reference Books

- A Primer on Neural Network Models for Natural Language Processing — Yoav Goldberg

URL: https://u.cs.biu.ac.il/~yogo/nnlp.pdf

- Neural Network Methods for Natural Language Processing — Yoav Goldberg

URL: https://link.springer.com/book/10.1007/978-3-031-02165-7

- Information Theory, Inference, and Learning Algorithms — David J. C. MacKay

URL: https://www.inference.org.uk/itprnn/book.pdf

- Taming Text: How to Find, Organize, and Manipulate It — Grant S. Ingersoll, Thomas S. Morton, Drew Farris

URL: https://www.manning.com/books/taming-text

- Introduction to Information Retrieval — Cambridge Book Information — Manning, Raghavan, Schütze

URL: https://assets.cambridge.org/97805218/65715/frontmatter/9780521865715_frontmatter.pdf

---


## 🖥️ PRESENTATION SLIDES


# Experiment-2.3 - All Lecture Slides Text


## Exp 2.3
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
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 2                   Experiment No.2.3
- Topic
- : Exploring Generative AI, Natural Language Processing and Azure
- AI
- Tools.
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning
- Objectives
- To understand the role of text analysis in Artificial Intelligence and Natural Language Processing
- .
- To
- learn how unstructured text is converted into meaningful and structured information
- .
- To
- understand tokenization and different text preprocessing techniques
- .
- To
- study statistical text analysis methods such as frequency analysis, Bag-of-Words, and TF-IDF
- .
- To
- understand semantic language models, word
- embedding's,
- and cosine similarity.

### Slide 3
- Recap
- of Previous Experiment
- Generative AI can create new content such as text, images, audio, video, and code.
- Prompts are inputs given to AI models, and better prompts produce better responses.
- Large Language Models process language using tokens, embedding's, transformers, and attention mechanisms.
- Retrieval Augmented Generation improves AI responses by retrieving relevant external information.

### Slide 4
- Topic 1:
- Introduction to Text
- Analysis
- Topic 2:
- Tokenization and Text
- Preprocessing
- Topic 3:
- Statistical Text
- Analysis
- Topic 4:
- Semantic Language Models
- Figure-1 :
- Text Analysis using NLP
- Source :
- https://pagadala-saiteja.medium.com/an-introduction-to-natural-language-processing-for-text-analysis-7856267266d5
- Text Analysis using NLP

### Slide 5
- Figure-2:
- Text analysis Techniques
- Source:
- https
- ://
- forms.app
- /en/blog/text-analysis
- Introduction to Text Analysis
- Text analysis is a subset of
- Natural Language Processing
- that enables machines to extract meaning, structure, and useful insights from unstructured text
- .
- Text analysis helps convert raw text into actionable information for decision-making
- .
- Common use cases include:
- Language detection
- Key term extraction
- Entity detection
- PII detection
- Text classification
- Sentiment analysis
- Text summarization

### Slide 6
- Tokenization is the first step in text analysis.
- It is the process of breaking a sentence, paragraph, or document into smaller units called
- tokens
- .
- Example
- :
- </a:r><a:br><a:rPr lang="en-US" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Sentence: “We choose to go to the moon”
- Tokens:
- </a:r><a:br><a:rPr lang="en-US" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>We
- choose
- to
- go
- to
- the
- moon
- Figure-3
- :Tokenization in
- NLP
- Source:
- https
- ://www.geeksforgeeks.org/nlp/nlp-how-tokenizing-text-sentence-words-works/
- Tokenization

### Slide 7
- Common
- preprocessing techniques include:
- Text Normalization:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Converting text into lowercase and removing punctuation or special symbols.
- Stop Word Removal:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Removing common words such as “the”, “is”, “a”, “an”, and “of”.
- N-Gram Extraction:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Finding word groups such as “artificial intelligence” or “natural language processing”.
- Stemming:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Reducing words to their root form by removing endings.
- Lemmatization:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Converting words into their valid dictionary form.
- POS Tagging:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Identifying grammatical roles such as noun, verb, adjective, or adverb.
- Figure-4
- :Text Pre-processing Techniques
- Source:
- https
- ://www.linkedin.com/pulse/unlocking-power-text-deep-dive-nlp-its-preprocessing-dr-hesam-akhtar-rkgsc/
- Text
- Pre-processing
- Techniques

### Slide 8
- After tokenization and preprocessing, statistical techniques are used to identify patterns and meaning from text.
- Frequency Analysis:
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Counts how many times each word appears in a document.
- Frequently
- occurring words often indicate the main topic of the document.
- Bag-of-Words:
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Represents text as word counts or word occurrences.
- It ignores grammar and word order but is useful for machine learning tasks.
- TF-IDF:
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Term Frequency-Inverse Document Frequency identifies important words in a document compared with other documents.
- A high TF-IDF score means a word is important in one document but not common in all documents.
- Figure-5
- :Statistical Text Analysis
- Source:
- https
- ://loganix.com/what-is-
- tf
- -
- idf
- /
- Statistical Text Analysis

### Slide 9
- Bag-of-Words Model
- Bag-of-Words converts text into numerical form by counting word occurrences.
- It is commonly used in:
- Spam detection
- Sentiment analysis
- Text classification
- Document
- categorization
- TF-IDF
- TF-IDF gives importance to words that appear frequently in one document but rarely across other documents.
- Formula:
- </a:r><a:br><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1500" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>TF-IDF = Term Frequency × Inverse Document Frequency
- TF-IDF is useful for keyword extraction and document comparison.
- Figure-6
- :
- Bag-of-Words
- Source:
- https
- ://ayselaydin.medium.com/4-bag-of-words-model-in-nlp-434cb38cdd1b
- Bag-of-Words and TF-IDF

### Slide 10
- Text Rank
- Text Rank
- is an unsupervised graph-based algorithm used for text summarization and keyword extraction
- .
- In Text Rank,
- each sentence is treated as a node in a graph.
- Connections between sentences are created based on similarity
- .
- Steps
- in
- Text Rank:
- Split the document into sentences
- Create sentence nodes
- Calculate similarity between sentences
- Rank the sentences
- Select top-ranked sentences for
- summary
- Figure-7
- :
- Text Rank for Text Summarization
- Source:
- https
- ://www.analyticsvidhya.com/blog/2018/11/introduction-text-summarization-textrank-python/
- Text Rank
- for Text Summarization

### Slide 11
- Word
- Embedding's
- and Cosine Similarity
- Word
- embedding's
- represent words as vectors.
- A vector is a list of numbers that captures the meaning of a word
- .
- Example:
- dog = [0.8, 0.6, 0.1]
- cat = [0.7, 0.5, 0.2]
- tree = [0.2, 0.1, 0.9]
- Cosine similarity is used to measure similarity between two vectors.
- If cosine similarity is close to 1, the words are highly similar.
- If cosine similarity is close to 0, the words are less similar.
- Figure-8
- :
- Word Embedding's and Cosine Similarity
- Source:
- https
- ://www.geeksforgeeks.org/nlp/tokenization-vs-embeddings/
- Word
- Embedding's
- and Cosine Similarity

### Slide 12
- Semantic Language Models
- Semantic language models understand the meaning and context of words
- .
- Modern NLP models represent words as numerical vectors called
- embedding's
- .
- Words with similar meanings have similar vector directions
- .
- Example:
- Dog and cat have similar meanings because both are animals.
- Dog and tree have less similarity because they belong to different categories
- .
- Figure-9:
- Semantic Language Models
- Source:
- https
- ://se-rwth.github.io/research/Semantics/
- Semantic Language Models

### Slide 13
- Summary of the
- Experiment
- Text analysis is an important application of Artificial Intelligence and Natural Language Processing
- .
- Tokenization breaks text into smaller units called tokens
- .
- Frequency analysis, Bag-of-Words, and TF-IDF are statistical techniques for text representation
- .
- Text Rank
- is used for extractive summarization and keyword extraction
- .
- Semantic language models use
- embedding's
- to understand meaning and context
- .
- Text analysis is useful in sentiment analysis, spam detection,
- Chabot's,
- search engines, and summarization.

### Slide 14
- Next
- Experiment
- T
- opic(s)
- Introduction to Speech AI
- Speech-to-Text
- and Automatic Speech
- Recognition
- Text-to-Speech
- and Speech
- Synthesis
- Voice
- Assistants and Real-World Applications

### Slide 15
- Quiz/ FAQ’s
- What is text analysis
- ?
- What
- is tokenization
- ?
- What
- is the difference between stemming and lemmatization
- ?
- What
- are stop words
- ?
- What
- is Bag-of-Words
- ?
- What
- is TF-IDF
- ?
- What
- are word
- embedding's?
- What
- is cosine similarity
- ?

### Slide 16
- R
- eferences/ Articles/ Videos
- Reference / Articles
- Natural Language Processing with Python
- https://www.nltk.org/book/
- Speech and Language Processing
- https://web.stanford.edu/~jurafsky/slp3/
- Scikit
- -learn Text Feature Extraction
- https://
- scikit-learn.org/stable/modules/feature_extraction.html
- Videos
- Natural Language Processing - Tokenization
- https://www.youtube.com/watch?v=O2jGzHSJzpg
- Text Representation using TF-IDF
- https://www.youtube.com/watch?v=ATK6fm3cYfI
- Introduction to NLP Bag-of-Words Model
- https://www.youtube.com/watch?v=8Mlc4-3tgzc

### Slide 17
- Additional
- learning
- R
- esources
- Additional Resources for Learning NLP Basics
- https://www.nltk.org/
- </a:r><a:br><a:rPr lang="en-US" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://www.nltk.org/book/
- Additional Resources for Text Preprocessing
- https://www.geeksforgeeks.org/nlp/text-preprocessing-for-nlp-tasks/
- Additional Resources for Bag-of-Words and TF-IDF
- https://scikit-learn.org/stable/tutorial/text_analytics/working_with_text_data.html
- Additional Resources for Semantic Models
- https://web.stanford.edu/~jurafsky/slp3/

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


================================================================================


# Experiment-2.4 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-2.4
# Experiment-2.4

- Course Outcome to be mentioned which is mapped with this experiment.

- Manual of the experiment.

- Relevant Demonstrative Video LINK.

- Relevant Book/Standard Code.

- Other Resource materials or Web Links.

---


================================================================================


# Experiment-3.1 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-3.1
# Experiment-3.1

## Understanding Natural Language Processing and Speech AI with Microsoft Tools.

##  CO5

##

## Aim

To study the concept of speech-enabled AI applications and understand how speech recognition and speech synthesis are used to create intelligent voice-based systems.

## Objectives

The objectives of this experiment are:

- To understand the meaning of speech-enabled AI solutions.

- To study the working of speech recognition or speech-to-text technology.

- To study the working of speech synthesis or text-to-speech technology.

- To understand the role of speech technologies in conversational AI systems.

- To identify the real-world applications, advantages, and limitations of speech-enabled AI systems.

## Theory

Speech is one of the most natural and important methods of human communication. Humans normally communicate with each other through spoken language, and when the same ability is added to AI applications, machines become easier and more natural to use. Speech-enabled AI solutions allow users to interact with computers, mobile applications, smart devices, and AI agents using voice commands instead of typing text or clicking buttons.

Speech-enabled solutions mainly depend on two important technologies: speech recognition and speech synthesis. Speech recognition converts spoken words into written text, while speech synthesis converts written text into spoken audio. These two technologies work together to create voice-based AI systems such as virtual assistants, customer service bots, smart speakers, navigation systems, healthcare dictation tools, and e-learning platforms.

Speech capabilities make AI applications more accessible and user-friendly. They are especially useful for people with visual impairments, reading difficulties, or mobility challenges. They also help users perform tasks hands-free, such as giving voice commands while driving, cooking, working, or using smart devices. Speech technologies can support multiple languages and dialects, which helps AI systems reach a wider audience.

## Speech-Enabled AI Solutions

Speech-enabled AI solutions are applications that can understand spoken input or generate spoken output, as shown in Figure 1. These systems make human-computer interaction more natural because users can communicate with machines in the same way they communicate with people.

For example, when a user says, “What is the weather today?”, a voice assistant listens to the spoken command, converts it into text, processes the meaning, retrieves the answer, and then speaks the response back to the user. This complete process involves speech recognition, natural language processing, and speech synthesis.

Speech-enabled AI solutions are useful in many areas. In customer service, they can transcribe customer calls, route callers to the correct department, and support automated voice responses. In education, they can read lessons aloud and help students with different learning needs. In healthcare, doctors can dictate patient notes instead of typing them manually. In accessibility tools, speech systems can read documents and websites aloud for visually impaired users.

The main goal of speech-enabled AI is to make technology easier, faster, and more inclusive for users.

Figure 1: Speech-enabled voice assistant system.

## Speech Recognition

Speech recognition is also called speech-to-text. It is the process of converting spoken language into written text as shown in Figure 2. This technology allows AI systems to listen to human speech and convert it into a form that computers can process.

For example, when a person says, “Open the calendar,” the speech recognition system converts the spoken sentence into written text: “Open the calendar.” After that, the AI system can understand the command and perform the required action.

Speech recognition is used in voice assistants, call centers, meeting transcription tools, healthcare documentation systems, smart home devices, and language learning applications.

Figure 2: Speech recognition processing pipeline.

## Working of Speech Recognition

Speech recognition works through a series of stages. Each stage plays an important role in converting sound into accurate text.

## 1. Audio Capture

The first stage is audio capture. In this stage, a microphone records the user’s voice. Human speech is produced as sound waves, but computers cannot directly understand sound waves. Therefore, the microphone converts the analog sound waves into digital signals.

The quality of audio capture is very important. If there is background noise, poor microphone quality, or the speaker is too far from the microphone, the accuracy of speech recognition may decrease. Clear audio input improves the performance of the system.

## 2. Pre-Processing

After audio capture, the recorded audio is cleaned and prepared for further processing. This stage is called pre-processing. The system may remove background noise, unwanted clicks, hums, and other disturbances from the audio signal.

Pre-processing helps the system focus only on useful speech information. It improves the quality of input given to the speech recognition model.

## 3. Feature Extraction

Raw audio contains a large amount of information. It is difficult for the AI model to process raw audio directly. Therefore, the system extracts important features from the audio signal.

One common method used for feature extraction is Mel-Frequency Cepstral Coefficients, also called MFCC. MFCC represents the important characteristics of speech in a compact numerical form. It is inspired by the way the human ear hears sound. MFCC focuses more on the frequency ranges that are important for human speech.

In simple words, MFCC helps convert the speech signal into useful numbers that the machine learning model can understand.

## 4. Acoustic Modeling

Acoustic modeling is the stage where the system identifies the sounds present in speech. These small sound units are called phonemes. A phoneme is the smallest unit of sound that can change the meaning of a word.

For example, the word “cat” contains three phonemes: /k/, /æ/, and /t/. The acoustic model studies the extracted audio features and predicts which phonemes are being spoken.

Modern speech recognition systems use deep learning models such as transformer-based models. These models can understand speech patterns more accurately by analyzing the surrounding audio context. This helps the system recognize words even when pronunciation, accent, or speaking speed varies.

## 5. Language Modeling

After identifying phonemes, the system uses language modeling to predict the most meaningful word sequence. Language models understand vocabulary, grammar, sentence structure, and common word patterns.

This stage is important because some words sound the same but have different meanings. For example, “their” and “there” have similar pronunciations, but their meanings are different. The language model uses context to select the correct word.

For example, in the sentence “The weather is nice,” the model can understand that “weather” is more suitable than “whether.”

## 6. Decoding

Decoding is the process of selecting the best possible text output from many possible word combinations. The system compares different possibilities and chooses the sentence that best matches the audio input and language rules.

For example, if the user says, “Please send the report by Friday,” the decoder may compare different possible sentences and finally select the most accurate one.

## 7. Post-Processing

The final stage is post-processing. In this stage, the raw text is improved and formatted properly. The system adds capitalization, punctuation, number formatting, and other corrections.

For example, raw output like “hello my name is sam” can be converted into “Hello, my name is Sam.” Similarly, “three p m” can be converted into “3 PM.”

Post-processing makes the output easier to read and understand.

## Speech Synthesis

Speech synthesis is also called text-to-speech. It is the process of converting written text into spoken audio. This technology allows AI systems to speak responses to users, as shown in Figure 3.

For example, if the text is “Your appointment is at 3 PM,” the speech synthesis system converts this text into natural-sounding speech.

Speech synthesis is used in virtual assistants, chatbots, navigation systems, screen readers, e-learning platforms, audio notifications, and entertainment applications.

## Figure 3: Text-to-speech synthesis process.

## Working of Speech Synthesis

Speech synthesis also works through several stages. These stages convert written text into meaningful and natural-sounding voice output.

## 1. Text Normalization

The first stage of speech synthesis is text normalization. In this stage, the system converts written symbols, abbreviations, dates, numbers, and special characters into spoken form.

For example, the sentence “Dr. Smith ordered 3 items for $25.50” is converted into “Doctor Smith ordered three items for twenty-five dollars and fifty cents.”

Text normalization is important because computers must know how to pronounce numbers, abbreviations, and symbols properly. Without normalization, the speech may sound unnatural or incorrect.

## 2. Linguistic Analysis

After normalization, the system performs linguistic analysis. In this stage, the text is divided into words, syllables, and phonemes. The system analyzes how each word should be pronounced.

This stage may use pronunciation dictionaries and AI models to decide the correct pronunciation of words. It is especially important in English because spelling and pronunciation are often different.

For example, the words “though,” “through,” and “cough” contain similar letters, but they are pronounced differently.

## 3. Grapheme-to-Phoneme Conversion

Grapheme-to-phoneme conversion, also called G2P conversion, converts written letters into sound units. A grapheme is a written letter or group of letters, and a phoneme is a sound unit.

For example, the word “phone” is written with the letters “p-h-o-n-e,” but it is pronounced using the /f/ sound at the beginning. The G2P system helps the AI model decide the correct sound for each word.

Modern speech synthesis systems use neural networks to perform G2P conversion more accurately, especially for proper names, uncommon words, and regional pronunciations.

## 4. Prosody Generation

Prosody means the natural rhythm, pitch, stress, pauses, and intonation used in speech. Prosody is very important because it makes speech sound human-like.

A sentence can have different meanings depending on how it is spoken. For example, the sentence “I never said he ate the cake” can express different meanings depending on which word is stressed.

Prosody generation decides where to pause, which words to emphasize, how fast to speak, and whether the pitch should rise or fall. Without proper prosody, the voice may sound robotic or flat.

## 5. Audio Waveform Generation

The final stage is audio waveform generation. In this stage, the system produces the actual speech audio. Modern systems use neural vocoders such as WaveNet, WaveGlow, and HiFi-GAN to generate high-quality and natural-sounding speech.

The system converts phoneme and prosody information into audio signals. These signals are then played through speakers or headphones so that the user can hear the spoken output.

## Combining Speech Recognition and Speech Synthesis

Speech recognition and speech synthesis are often combined to create conversational AI systems. Speech recognition allows the system to listen and understand the user’s spoken input. Speech synthesis allows the system to respond using spoken output.

For example, in a voice assistant:

The user says, “Set an alarm for 6 AM.”

The system uses speech recognition to convert this voice command into text.

The AI system understands the command and sets the alarm.

Then speech synthesis is used to reply, “Your alarm has been set for 6 AM.”

This combination creates a two-way conversation between humans and machines. It is used in smart speakers, IVR systems, customer service bots, language learning apps, and voice-controlled vehicles.

## Figure 4: Voice interaction flow using speech recognition, natural language processing, and text-to-speech.

##

## Real-World Applications

Speech recognition and speech synthesis are used in many real-world applications.

## 1. Voice Assistants

Voice assistants such as Siri, Alexa, and Google Assistant use speech recognition to understand user commands and speech synthesis to reply. Users can ask questions, set reminders, play music, check the weather, and control smart devices using voice.

## 2. Customer Service

Call centers use speech recognition to transcribe customer calls and analyze customer issues. Speech synthesis is used in automated phone systems to guide customers through options.

## 3. Meeting Transcription

Speech recognition is used to convert meetings, interviews, and lectures into written notes. This saves time and helps create searchable records.

## 4. Healthcare Documentation

Doctors and healthcare professionals use speech recognition to dictate patient notes. This reduces typing work and allows doctors to focus more on patient care.

## 5. Accessibility Tools

Speech synthesis helps visually impaired users by reading text aloud. It also supports users with reading difficulties such as dyslexia.

## 6. E-Learning

Educational platforms use speech synthesis to create narrated lessons, audio learning materials, and pronunciation examples. Speech recognition can also be used to evaluate spoken answers and language practice.

## 7. Navigation Systems

Navigation apps use speech synthesis to speak directions, alerts, and route updates. This allows users to receive information without looking at the screen.

## 8. Smart Home Devices

Smart home systems use speech recognition to accept commands such as turning lights on, adjusting temperature, or playing music.

## Code

# Install only the required libraries

!pip -q install SpeechRecognition gTTS

!apt-get -qq install ffmpeg > /dev/null

import subprocess

import speech_recognition as sr

from gtts import gTTS

from google.colab import files

from IPython.display import Audio, display

def assistant():

print("Upload a short voice recording: WAV, MP3 or M4A")

uploaded = files.upload()

if not uploaded:

print("No recording uploaded.")

return

filename = next(iter(uploaded))

# Convert the recording to a compatible WAV file

result = subprocess.run(

["ffmpeg", "-y", "-i", filename,

"-ar", "16000", "-ac", "1", "-c:a", "pcm_s16le",

"/tmp/voice_input.wav"],

capture_output=True

)

if result.returncode != 0:

print("Could not open this audio file. Try WAV or MP3.")

return

# Voice to text

recognizer = sr.Recognizer()

recognizer.operation_timeout = 20

try:

with sr.AudioFile("/tmp/voice_input.wav") as source:

recording = recognizer.record(source)

text = recognizer.recognize_google(

recording, language="en-IN"

)

print("You said:", text)

except sr.UnknownValueError:

print("Speech was unclear. Try a clearer recording.")

return

except sr.RequestError as error:

print("Speech service error:", error)

return

# Choose an answer

question = text.lower()

if "hello" in question:

reply = "Hello! Welcome to our AI class."

elif "your name" in question:

reply = "I am your classroom voice assistant."

elif "artificial intelligence" in question:

reply = "AI helps computers perform tasks that require intelligence."

else:

reply = "You said: " + text

print("Assistant:", reply)

# Text to voice

try:

gTTS(reply, lang="en").save("/tmp/reply.mp3")

display(Audio("/tmp/reply.mp3", autoplay=True))

except Exception as error:

print("Could not generate speech:", error)

assistant()

## Practice Task Questions

Write a short note on speech-enabled AI solutions.

Differentiate between speech recognition and speech synthesis.

Explain the working of speech recognition in simple words.

Write the main stages involved in the speech recognition process.

Explain the role of MFCC in speech recognition.

What are phonemes? Explain with one example.

Explain the working of speech synthesis in simple words.

What is text normalization? Give one example.

Explain the importance of prosody in speech synthesis.

Write five real-world applications of speech-enabled AI systems.

## Video Links

Creating Speech-Enabled Apps with Azure AI Services

Recognize & Synthesize Speech with Azure AI Speech Service

How Does Speech Recognition Work? Learn about Speech to Text, Voice Recognition and Speech Synthesis

Azure AI Speech Explained — Speech Recognition

Microsoft Azure AI Services—Get Started With Text-To-Speech

## Additional Resources

Azure Speech Documentation

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/

What is Azure Speech?

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/overview

Speech-to-Text Documentation — Azure AI Speech

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/index-speech-to-text

Text-to-Speech Documentation — Azure AI Speech

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/index-text-to-speech

Text-to-Speech Overview — Azure AI Speech

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/text-to-speech

About the Speech SDK — Azure AI Speech

URL: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-sdk

Azure Speech SDK Samples — GitHub

URL: https://github.com/Azure-Samples/cognitive-services-speech-sdk

Azure AI Speech Product Page

URL: https://azure.microsoft.com/en-us/products/ai-foundry/tools/speech

Google Cloud Speech-to-Text

URL: https://cloud.google.com/speech-to-text

Text-to-Speech Technology: What It Is and How It Works

URL: https://www.readingrockets.org/topics/assistive-technology/articles/text-speech-technology-what-it-and-how-it-works

## Text Books

Speech and Language Processing

Authors: Daniel Jurafsky and James H. Martin

PDF/Access Link: https://web.stanford.edu/~jurafsky/slp3/ed3book.pdf

Useful for: Speech recognition, language modelling, NLP, and modern AI-based language systems.

Speech and Language Processing — Official Book Page

Authors: Daniel Jurafsky and James H. Martin

PDF/Access Link: https://web.stanford.edu/~jurafsky/slp3/

Useful for: Updated chapters on speech recognition, language models, and NLP concepts.

Speech Signal Processing by Praat

Author: David Weenink

PDF/Access Link: https://www.fon.hum.uva.nl/david/sspbook/sspbook.pdf

Useful for: Basic speech signal processing, waveform analysis, pitch, formants, and speech features.

Introduction to Digital Speech Processing

Author: Lawrence R. Rabiner

PDF/Access Link: https://elupu.utcluj.ro/wp-content/uploads/2024/03/Rabiner.pdf

Useful for: Digital speech processing, speech production, speech analysis, and speech recognition basics.

Fundamentals of Speech Recognition

Authors: Lawrence Rabiner and Biing-Hwang Juang

PDF/Access Link: https://external.dandelon.com/download/attachments/dandelon/ids/DE0066927926FFD6878FAC1257A3600449F90.pdf

Useful for: Speech recognition pipeline, acoustic modeling, language modeling, and recognition systems.

## Reference Books / Reference Resources

Spoken Language Processing: A Guide to Theory, Algorithm, and System Development

Authors: Xuedong Huang, Alex Acero, and Hsiao-Wuen Hon

Access Link: https://www.microsoft.com/en-us/research/publication/spoken-language-processing/

Useful for: Speech recognition, speech synthesis, spoken dialogue systems, and real-world speech applications.

Springer Handbook of Speech Processing

Editors: Jacob Benesty, M. M. Sondhi, and Yiteng Huang

PDF/Access Link: https://jontalle.web.engr.illinois.edu/Public/HandbookSpeechProcessing.08.pdf

Useful for: Advanced speech processing, speech coding, recognition, synthesis, and speaker analysis.

Neural Text-to-Speech Synthesis

Authors: Xu Tan and others

Access Link: https://link.springer.com/book/10.1007/978-981-99-0827-1

Useful for: Modern neural TTS, deep learning-based speech synthesis, and vocoder-based speech generation.

Text-to-Speech Synthesis — Cambridge Core Chapter

Author: Paul Taylor

Access Link: https://www.cambridge.org/core/books/texttospeech-synthesis/introduction/0F0A5AE0427A0B4EBB779B634CF77752

Useful for: Basic understanding of text-to-speech systems, pronunciation, prosody, and synthesis process.

Azure AI Speech Documentation

Publisher: Microsoft Learn

Access Link: https://learn.microsoft.com/en-us/azure/ai-services/speech-service/

Useful for: Practical implementation of speech-to-text, text-to-speech, speech SDK, and AI speech services.

---


## 🖥️ PRESENTATION SLIDES


# Experiment-3.1 - All Lecture Slides Text


## Exp 3.1
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
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 3                   Experiment No.3.1
- Topic
- : Understanding Natural Language Processing and Speech AI Concepts with Microsoft
- Tools
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning
- Objectives
- After
- completing this experiment, students will be able to
- :
- Understand the concept of speech-enabled AI applications
- .
- Study the working of speech recognition or speech-to-text technology
- .
- Understand the working of speech synthesis or text-to-speech technology
- .
- Identify the role of speech technologies in conversational AI systems
- .

### Slide 3
- Recap
- of Previous Experiment
- Text analysis is an important application of Artificial Intelligence and Natural Language Processing.
- Tokenization breaks text into smaller units called tokens.
- Frequency analysis, Bag-of-Words, and TF-IDF are statistical techniques for text representation.
- Text Rank is used for extractive summarization and keyword extraction.
- Semantic language models use embedding's to understand meaning and context.
- Text analysis is useful in sentiment analysis, spam detection, Chabot's, search engines, and summarization.

### Slide 4
- Figure-1 :
- Speech Processing Workflow using NLP
- Source
- :
- https://www.linkedin.com/pulse/speech-recognition-synthesis-next-frontier-conversational-cjiyc/
- Speech Recognition and Speech Synthesis
- in
- AI
- Topic(s
- )
- Introduction to Speech AI
- Speech-to-Text and Automatic Speech Recognition
- Text-to-Speech and Speech
- Synthesis
- Combining Speech Recognition
- and
- Speech Synthesis

### Slide 5
- Figure-2:
- Next-Generation Voice Assisted
- Solutions
- Source:
- https
- ://embeddedcomputing.com/technology/
- ai
- -machine-learning/computer-vision-speech-processing/next-generation-voice-assisted-solutions
- Speech-enabled AI solutions allow users to interact with machines using voice commands
- .
- These systems make human-computer interaction more natural because humans commonly communicate through spoken language
- .
- Speech-enabled AI applications use voice input and voice output to support intelligent interaction
- .
- Examples include voice assistants, smart speakers, customer service bots, navigation systems, healthcare dictation tools, and e-learning platforms.
- Speech-Enabled AI Solutions

### Slide 6
- Speech is one of the most natural forms of human communication
- .
- Speech AI helps users perform tasks hands-free while driving, cooking, working, or using smart devices
- .
- It also improves accessibility for visually impaired users, people with reading difficulties, and users with mobility challenges.
- Figure-3
- :Benefits of AI Communication for Speech Therapy
- Source:
- https
- ://emitrr.com/blog/
- ai
- -for-speech-therapy/
- Importance of Speech in AI

### Slide 7
- Speech recognition is also called
- speech-to-text
- .
- It is the process of converting spoken language into written text
- .
- For example, when a user says, “Open the calendar,” the system converts the speech into text: “Open the calendar
- .”
- Figure-4
- :Speech Recognition
- Source:
- https
- ://nordvpn.com/blog/what-is-speech-recognition/?
- srsltid
- =AfmBOopjpbgTA9UZ6fC33XUfJfo5WIDIZ-5JxMTGrCnKwZB-kuxsgJS8
- Speech Recognition

### Slide 8
- Speech recognition works through different stages
- :
- First, the microphone captures the user’s voice as an audio signal.
- Then pre-processing removes background noise and improves the quality of the audio.
- Feature extraction converts the audio signal into useful numerical features such as MFCC.
- The acoustic model identifies small sound units called phonemes.
- The language model predicts the most meaningful sequence of words.
- Finally, decoding and post-processing generate properly formatted text with punctuation and capitalization.
- Figure-5
- :Working of Speech Recognition
- Source:
- https
- ://www.techtarget.com/searchcustomerexperience/definition/speech-recognition
- Working of Speech Recognition

### Slide 9
- Speech synthesis is also called
- text-to-speech
- .
- It is the process of converting written text into spoken audio
- .
- For example, the text “Your appointment is at 3 PM” can be converted into natural-sounding speech
- .
- Figure-6
- :Speech
- Synthesis
- Source:
- https
- ://en.wikipedia.org/wiki/
- Speech_synthesis
- Speech Synthesis

### Slide 10
- Speech synthesis converts text into speech through several stages.
- Text normalization converts symbols, numbers, dates, and abbreviations into spoken form.
- Linguistic analysis divides the text into words, syllables, and phonemes.
- Grapheme-to-phoneme conversion changes written letters into sound units.
- Prosody generation adds rhythm, pitch, stress, pauses, and intonation.
- Finally, audio waveform generation creates the final speech audio using modern neural
- vocoders
- .
- Figure-7 :
- Working of Speech Synthesis
- Source:
- https
- ://www.researchgate.net/publication/304601298_Development_of_Text-to-Speech_Synthesizer_for_Pali_Language/figures?lo=1
- Working of Speech Synthesis

### Slide 11
- Speech recognition and speech synthesis are often combined to create conversational AI systems.
- Speech recognition helps the system listen to the user’s spoken input.
- Natural Language Processing helps the system understand the meaning of the input.
- Speech synthesis helps the system respond using spoken output.
- Example:
- The user says, “Set an alarm for 6 AM.”
- The system converts speech into text, understands the command, sets the alarm, and replies, “Your alarm has been set for 6 AM.”
- Figure-8 :
- Combining Speech Recognition
- and Speech Synthesis
- Source:
- https
- ://iprobe.cse.msu.edu/
- project_detail.php?id
- =20&?title=DeepTalk:_Vocal_Style_Encoding_for_Speaker_Recognition_and_Speech_Synthesis
- Combining Speech Recognition
- and
- Speech Synthesis

### Slide 12
- Summary of the
- Experiment
- Speech-enabled AI applications allow users to interact with machines using voice.
- Speech recognition converts spoken language into written text.
- Speech synthesis converts written text into spoken audio.
- Together, speech recognition, NLP, and speech synthesis create conversational AI systems.
- These systems are widely used in voice assistants, customer support, healthcare, education, accessibility tools, navigation, and smart homes
- .

### Slide 13
- Next
- Experiment
- T
- opic(s)
- Topic 1: Computer
- Vision
- Topic
- 2: Image
- Classification
- Topic
- 3: Object
- Detection
- Topic
- 4: Optical Character
- Recognition

### Slide 14
- Quiz/ FAQ’s
- What is speech-enabled AI?
- What is speech recognition?
- What is speech synthesis?
- What is the difference between speech-to-text and text-to-speech?
- Why is pre-processing important in speech recognition?
- What is the role of NLP in conversational AI?
- Give two real-world applications of speech-enabled AI.
- Why is speech AI important for accessibility?

### Slide 15
- R
- eferences/ Articles/ Videos
- References / Articles
- Microsoft Learn — Introduction to Azure AI Speech
- https://learn.microsoft.com/en-us/azure/ai-services/speech-service/overview
- Microsoft Learn — Speech to Text
- https://learn.microsoft.com/en-us/azure/ai-services/speech-service/speech-to-text
- Microsoft Learn — Text to Speech
- https://
- learn.microsoft.com/en-us/azure/ai-services/speech-service/text-to-speech
- Videos
- How Does Speech Recognition Work? Speech-to-Text, Voice Recognition and Speech Synthesis
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:hlinkClick r:id="rId6"/></a:rPr><a:t>https://www.youtube.com/watch?v=6altVgTOf9s
- Speech-to-Text & Text-to-Speech
- Conversion
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:hlinkClick r:id="rId7"/></a:rPr><a:t>https://www.youtube.com/watch?v=7uFycTtMwdk
- Text-to-Speech Explained: The Future of Digital Interactions
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"/></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:hlinkClick r:id="rId8"/></a:rPr><a:t>https://www.youtube.com/watch?v=257RtqWDa0Q

### Slide 16
- Additional
- learning
- R
- esources
- Microsoft Learn — Azure AI Speech Documentation
- https://learn.microsoft.com/en-us/azure/ai-services/speech-service/
- Google Cloud — Text-to-Speech
- https://cloud.google.com/text-to-speech
- AWS — Amazon Transcribe
- https://aws.amazon.com/transcribe/
- AWS — Amazon Polly
- https://aws.amazon.com/polly/
- Mozilla
- Deep Speech
- Project
- https://github.com/mozilla/DeepSpeech
- Hugging Face — Speech Processing Models
- https://huggingface.co/tasks/automatic-speech-recognition

### Slide 17
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 18
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in


---


================================================================================


# Experiment-3.2 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-3.2
# Experiment-3.2

## Analysis of Speech Processing Workflows and Vision AI Architectures Using Microsoft Foundry.

## CO5

##

## Aim

To study the basic concepts of Computer Vision in Artificial Intelligence and understand how AI systems process, analyze, classify, detect, segment, interpret, and generate images.

## Objectives

The objectives of this experiment are:

- To understand the meaning and importance of computer vision.

- To study how images are represented using pixels and RGB channels.

- To understand filters, kernels, and convolution in image processing.

- To explain image classification, object detection, semantic segmentation, and contextual image analysis.

- To understand the basic workings of Convolutional Neural Networks.

- To study Vision Transformers and multimodal AI models.

- To understand image generation using diffusion models.

- To identify real-life applications of computer vision.

## Introduction

Computer vision is an important branch of Artificial Intelligence that enables computers to process and understand visual information from images, videos, and live camera feeds. It helps machines identify objects, detect locations, understand scenes, and generate descriptions from visual data.

Computer vision is used in many real-life applications such as autonomous vehicles, smart checkout systems, doorbell cameras, medical imaging, security systems, agriculture, robotics, and image generation tools.

A computer does not see an image like a human. It reads an image as numerical data made up of pixels. By analyzing these pixel values, AI models can understand objects, colors, shapes, textures, and patterns.

## Theory

## Computer Vision

Computer vision is the field of AI that allows machines to interpret and understand visual information. Its main purpose is to extract meaningful information from images or videos, as shown in Figure 1.

For example, a self-driving car uses computer vision to detect traffic lights, pedestrians, vehicles, and road signs. A smart checkout system uses computer vision to identify products automatically. A doorbell camera uses it to detect people at the door.

Computer vision combines image processing, machine learning, deep learning, pattern recognition, and neural networks.

## Figure 1: Comparison between human vision and computer vision systems.

## Image Representation

An image is made up of tiny units called pixels. A pixel is the smallest part of a digital image. Each pixel stores numerical information about brightness or color.

In a grayscale image, each pixel has a value from 0 to 255.

0 represents black.

255 represents white.

Values between 0 and 255 represent different shades of gray.

A color image usually has three channels: Red, Green, and Blue. This is called the RGB model.

Different combinations of red, green, and blue values create different colors. For example, red and green together can form yellow, while all three channels at maximum value form white.

## Image Processing

Image processing means applying operations on an image to improve it or extract useful information. It is used before applying AI models so that images become clearer and easier to analyze.

Common image processing tasks include:

Image enhancement

Noise removal

Edge detection

Blurring

Sharpening

Color correction

Conversion from color to grayscale

Image processing is important because raw images may contain noise, poor lighting, blur, or unwanted background information.

## Filters, Kernels, and Convolution

A filter is used to modify an image or extract features from it. A filter is represented by a small matrix called a kernel.

A kernel moves across the image and performs mathematical calculations on pixel values. This process is called convolution.

Different kernels create different effects. For example:

A blur kernel smooths the image.

A sharpening kernel makes details clearer.

An edge detection kernel highlights boundaries.

A Laplace filter detects sharp changes in pixel intensity.

Convolution is important because it helps identify visual features such as edges, lines, corners, shapes, and textures as shown in Figure 2.

Figure 2: Image filtering operation showing blurring and pixel shifting using convolution kernels.

## Image Classification

Image classification is a computer vision task in which an AI model predicts the label of an image.

For example, if an image contains an apple, the model may classify it as “apple.” If it contains a banana, the model may classify it as “banana.”

Image classification gives one main label for the entire image. It is used in fruit recognition, medical diagnosis, animal classification, face recognition, and document classification, as shown in Figure 3.

## Figure 3: Image classification process showing how a computer interprets image pixels and predicts object categories.

## Object Detection

Object detection is used to identify multiple objects in an image and show their locations. It gives both the name of the object and its position.

Object detection uses bounding boxes. A bounding box is a rectangular box drawn around an object.

For example, in an image containing an apple, banana, and orange, object detection can identify all three objects and draw separate boxes around them.

Object detection is used in self-driving cars, CCTV cameras, smart checkout systems, face detection, and traffic monitoring as shown in Figure 4.

## Figure 4: Object detection in a street scene using computer vision.

## Semantic Segmentation

Semantic segmentation is a more detailed computer vision task. In this technique, every pixel in an image is classified into a category.

Unlike object detection, which uses boxes, semantic segmentation marks the exact area of an object.

For example, in a road image, segmentation can mark road pixels, vehicle pixels, pedestrian pixels, and sky pixels separately.

Semantic segmentation is useful in medical imaging, autonomous vehicles, satellite image analysis, agriculture, and robotics, as shown in Figure 5.

## Figure 5: Image segmentation showing object-wise labeling of cat, cow, sky, trees, and grass.

## Contextual Image Analysis

Contextual image analysis means understanding not only objects in an image but also the relationship between them.

For example, if an image shows a person eating an apple, the system can understand the activity and generate the description:

“A person eating an apple.”

This technique is used in image captioning, visual question answering, AI assistants, content tagging, and accessibility tools.

## Convolutional Neural Network

A Convolutional Neural Network, or CNN, is a deep learning model widely used in computer vision. CNNs are designed to automatically learn important features from images.

A CNN usually contains:

Input layer

Convolutional layer

Activation function

Pooling layer

Flattening layer

Fully connected layer

Output layer

The convolutional layer applies filters to extract features. The pooling layer reduces the size of feature maps. The flattening layer converts feature maps into a one-dimensional array. The fully connected layer makes the final prediction.

CNNs are used for image classification, object recognition, face recognition, handwritten digit recognition, medical image analysis, and defect detection, as shown in Figure 6.

## Figure 6: Convolutional Neural Network architecture for image classification.

## Feature Maps and Training of CNN

When a filter is applied to an image, it creates a feature map. A feature map shows where important features such as edges, lines, or shapes are present.

During training, a CNN is given many labeled images. The model first makes predictions and compares them with the correct labels. If the prediction is wrong, it calculates the loss and adjusts its weights.

This process is repeated for many epochs. After training, the CNN learns useful patterns and can classify new images.

## Vision Transformers

Vision Transformers, also called ViTs, are modern computer vision models based on transformer architecture.

In Vision Transformers, an image is divided into small patches. Each patch is converted into a numerical vector. The model then uses attention to understand the relationship between different patches.

CNNs focus mainly on local features using filters, while Vision Transformers can understand global relationships in the image.

Vision Transformers are used in image classification, object recognition, medical image analysis, and multimodal AI systems as shown in Figure 7.

## Figure 7: Patch embedding and self-attention mechanism in Vision Transformer.

## Multimodal Models

Multimodal models are AI models that can process more than one type of data, such as text and images.

A vision model understands image features, while a language model understands words and sentences. When both are combined, the model can understand the relationship between images and text.

For example, if an image shows a person in a park with a hat and a backpack, a multimodal model can generate a description like:

“A person in a park with a hat and a backpack.”

Multimodal models are used in image captioning, visual question answering, AI assistants, image search, and text-to-image generation.

## Image Captioning and Visual Question Answering

Image captioning is the process of generating a text description for an image.

For example, an image of a dog running in a garden may be described as:

“A dog is running in a garden.”

Visual Question Answering, or VQA, allows a model to answer questions about an image.

For example, if an image shows a red car and the question is “What color is the car?”, the model may answer “red.”

Both tasks use computer vision and natural language processing together, as shown in Figure 8.

##

## Figure 8: Image captioning and visual question answering using a language model.

## Image Generation

Image generation is a modern AI technique in which models create new images from text prompts.

For example, if the prompt is:

“A dog carrying a stick in its mouth”

The AI model can generate an image matching the description.

Image generation models learn the relationship between words and visual features. They are used in design, education, advertising, entertainment, storytelling, and research visualization.

## Diffusion Models

Most modern image generation models use diffusion. A diffusion model starts with random noise and gradually removes the noise to create a meaningful image.

The process begins with random pixels. Then the model slowly forms shapes, colors, objects, and backgrounds according to the text prompt.

Diffusion models are powerful because they can generate realistic and creative images from natural language descriptions.

## Video Generation

Video generation is similar to image generation, but it creates a sequence of frames. These frames must follow a logical order to show motion.

Video generation is more complex because the model must understand movement, time, object behavior, and scene consistency.

It is used in animation, simulation, education, advertising, and entertainment.

## Difference Between CNN and Vision Transformer

CNN and Vision Transformer are both used in computer vision, but they work differently.

A CNN uses filters and convolution to extract features from images. It is effective for detecting edges, shapes, textures, and object parts.

A Vision Transformer divides an image into patches and uses attention to understand relationships between patches. It is useful for understanding the global context of an image.

In simple words:

CNN learns images using filters.

Vision Transformer learns images using patches and attention.

## Applications

Computer vision is used in many fields:

- Autonomous vehicles for detecting roads, traffic lights, vehicles, and pedestrians.

- Healthcare for analyzing X-rays, MRI scans, CT scans, and medical images.

- Smart checkout systems for recognizing products automatically.

- Security and surveillance for face detection and activity monitoring.

- Agriculture for crop monitoring and disease detection.

- Manufacturing for defect detection and quality inspection.

- Robotics for object recognition and navigation.

- Education for smart learning and image-based teaching.

- Accessibility tools for describing images to visually impaired users.

- Media and entertainment for image editing, AR, VR, and image generation.

## Code

# Import DeepFace for facial analysis

!pip install deepface  &> /dev/null

from deepface import DeepFace

# Import OpenCV for image handling

import cv2

# Import Matplotlib for image visualization

import matplotlib.pyplot as plt

# Load the input image using OpenCV

img1 = cv2.imread("/content/rachit.jpg")  # Reads the image file and stores it as an array

# Display the loaded image using Matplotlib

plt.imshow(img1)  # Converts the array back to an image format for visualization

plt.show()        # Displays the image on the screen

# Analyze the image using DeepFace for specific attributes

obj = DeepFace.analyze(img1, actions=['age', 'gender', 'race', 'emotion'])

# DeepFace analyzes the image to determine age, gender, race, and emotion

# 'actions' parameter specifies which attributes to analyze

# Print the entire analysis result as a dictionary

print(obj)  # Displays the results including all detected attributes

obj_first = obj[0]  # Get the first element if it's a list

print("Your age is", obj_first["age"],

"and you are", obj_first["dominant_race"],

"and current emotion is", obj_first["dominant_emotion"],

"and your gender capture is", obj_first["gender"])

## Practice Task Questions

- Write a short note on computer vision and explain any three real-life applications of it.

- Explain how an image is represented in a computer using pixels and numerical values.

- Differentiate between grayscale images and RGB color images with suitable examples.

- Explain the role of filters, kernels, and convolution in image processing.

- Describe image classification with an example of a fruit recognition system.

- Explain object detection and the use of bounding boxes in identifying objects.

- Differentiate between object detection and semantic segmentation.

- Draw and explain the basic architecture of a Convolutional Neural Network.

- Explain the difference between CNN and Vision Transformer in simple words.

- Write a short note on multimodal models and image generation using diffusion models.

## Video Links

Image classification vs Object detection vs Image segmentation

Introduction to Mask R-CNN for Image Segmentation

Vision Transformers Explained | The ViT Paper

Diffusion Models for AI Image Generation

Introduction to Image Generation

## Additional Resources

- Microsoft Learn: Introduction to Computer Vision Concepts

https://learn.microsoft.com/en-us/training/modules/introduction-computer-vision/

This resource covers computer vision tasks, filters, CNNs, Vision Transformers, and image generation.

- Azure AI Vision Documentation

https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/

Useful for understanding cloud-based computer vision services for image analysis and visual AI applications.

- Microsoft Azure: What is Computer Vision?

https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-computer-vision

This explains computer vision in simple terms and describes how computers process and understand images/videos.

- TensorFlow Tutorial: Convolutional Neural Network

https://www.tensorflow.org/tutorials/images/cnn

Useful for learning how CNNs classify images using TensorFlow and Keras.

- TensorFlow Tutorial: Image Classification

https://www.tensorflow.org/tutorials/images/classification

This explains a basic image classification workflow, including dataset preparation, model building, training, and evaluation.

- PyTorch: Transfer Learning for Computer Vision Tutorial

https://docs.pytorch.org/tutorials/beginner/transfer_learning_tutorial.html

Useful for learning how pretrained CNN models can be used for image classification tasks.

- PyTorch: TorchVision Object Detection Finetuning Tutorial

https://docs.pytorch.org/tutorials/intermediate/torchvision_tutorial.html

Useful for object detection and segmentation using a pretrained Mask R-CNN model.

- Google Machine Learning Crash Course

https://developers.google.com/machine-learning/crash-course

Helpful for understanding machine learning basics before studying CNNs and computer vision models.

- Keras Example: Image Classification from Scratch

https://keras.io/examples/vision/image_classification_from_scratch/

Useful for learning how to create an image classification model from image files.

- Learn PyTorch: Computer Vision

https://www.learnpytorch.io/03_pytorch_computer_vision/

This resource explains computer vision problems such as binary classification, multiclass classification, object detection, and segmentation.

## Textbooks

- Computer Vision: Algorithms and Applications — Richard Szeliski

PDF / Online Link: https://szeliski.org/Book/download.php

- Deep Learning — Ian Goodfellow, Yoshua Bengio, Aaron Courville

Online Link: https://www.deeplearningbook.org/

- Dive into Deep Learning — Aston Zhang, Zachary C. Lipton, Mu Li, Alexander J. Smola

PDF / Online Link: https://d2l.ai/

- Learning OpenCV — Gary Bradski and Adrian Kaehler

PDF Link: https://www.eecs.yorku.ca/course_archive/2010-11/W/4421/doc/LearningOpenCV_1_2.pdf

- First Principles of Computer Vision — Shree K. Nayar, Columbia University

PDF / Online Link: https://fpcv.cs.columbia.edu/Monographs

## Reference Books / Reference Resources

-  Deep Learning for Computer Vision—Stanford University

Online Notes Link: https://cs231n.github.io/

- Introduction to Computer Vision — Shree K. Nayar, Columbia University

PDF Link: https://cave.cs.columbia.edu/Statics/monographs/Introduction%20FPCV-0-1.pdf

- OpenCV-Python Tutorial — TutorialsPoint

PDF Link: https://www.tutorialspoint.com/opencv_python/opencv_python_tutorial.pdf

- TensorFlow Tutorial: Convolutional Neural Network

Online Link: https://www.tensorflow.org/tutorials/images/cnn

- PyTorch Tutorial: TorchVision Object Detection Finetuning

Online Link: https://docs.pytorch.org/tutorials/intermediate/torchvision_tutorial.html

---


## 🖥️ PRESENTATION SLIDES


# Experiment-3.2 - All Lecture Slides Text


## Exp 3.2
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
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 3                   Experiment No.3.2
- Topic
- : Analysis of Speech Processing Workflows and Vision AI Architectures Using Microsoft Foundry
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning
- Objectives
- After
- completing this experiment, students will be able
- to:
- Understand
- computer vision concepts
- .
- Study
- image representation using pixels and RGB channels
- .
- Understand
- image classification, object detection and segmentation
- .
- Explain
- CNNs, Vision Transformers and multimodal models
- .
- Understand
- image generation using diffusion models.

### Slide 3
- Recap
- of Previous Experiment
- Speech-enabled AI applications allow users to interact with machines using voice.
- Speech recognition converts spoken language into written text.
- Speech synthesis converts written text into spoken audio.
- Together, speech recognition, NLP, and speech synthesis create conversational AI systems.
- These systems are widely used in voice assistants, customer support, healthcare, education, accessibility tools, navigation, and smart homes.

### Slide 4
- Figure-1 :
- Applications of
- Computer
- Vision in AI
- Source:
- https
- ://www.upgrad.com/blog/what-are-the-applications-of-computer-vision-in-ai/
- Topic(s
- )
- Topic 1: Computer Vision
- Topic 2: Image Classification
- Topic 3: Object Detection
- Topic 4: Optical Character Recognition
- Computer Vision
- and
- AI-Based Image Intelligence

### Slide 5
- Figure-2:
- Computer Vision in AI
- Source:
- https
- ://www.almabetter.com/bytes/tutorials/artificial-intelligence/computer-vision-in-ai
- Computer Vision in AI
- Computer vision is a branch of AI that helps machines understand visual information
- .
- It
- processes images, videos and live camera feeds
- .
- It
- is used in autonomous vehicles, smart checkout systems, medical imaging, doorbell cameras and surveillance systems.

### Slide 6
- A digital image is made up of pixels.
- Each pixel stores numerical
- information.
- Gray scale
- images use values from 0 to
- 255.
- Color
- images use RGB channels: Red, Green and
- Blue.
- Different
- RGB values
- create different
- colors.
- Figure-3
- :A rasterized form of the letter 'a' magnified 16 times using pixel doubling
- Source:
- https
- ://pippin.gimp.org/image-processing/chap_dir.html
- Image Representation

### Slide 7
- Image processing improves or extracts information from
- images.
- Filters
- are used for blurring, sharpening and edge
- detection.
- A
- kernel is a small matrix used to process pixel
- values.
- Convolution
- means moving the kernel over the image to extract features.
- Figure-4
- :Convolution Kernel
- Example
- Source:
- https
- ://muneebsa.medium.com/deep-learning-101-lesson-20-convolution-kernels-40641dda695d
- Image Processing, Filters and Kernels

### Slide 8
- Image classification predicts the main label of an image
- .
- Example
- : apple, banana, orange, dog or car.
- The
- model is trained using labeled images
- .
- It
- is used in fruit recognition, medical diagnosis, face recognition and document classification.
- Figure-5
- :Image Classification
- Source:
- https
- ://www.superannotate.com/blog/image-classification-basics
- Image Classification

### Slide 9
- Object detection identifies multiple objects and shows their locations using bounding boxes
- .
- Semantic
- segmentation classifies every pixel of an image
- .
- Object
- detection gives rectangular boxes.
- Semantic segmentation gives exact object regions
- .
- Both
- are useful in self-driving cars, healthcare and robotics.
- Figure-6
- :Object Detection
- and Semantic
- Segmentation
- Source:
- https
- ://manipulation.csail.mit.edu/segmentation.html
- Object Detection
- and
- Semantic Segmentation

### Slide 10
- CNNs are deep learning models used for image-related tasks
- .
- They
- automatically learn features from images
- .
- Main
- layers include input layer, convolutional layer, pooling layer, flattening layer, fully connected layer and output layer
- .
- CNNs
- are used in image classification, object recognition and medical image analysis.
- Figure-7 :
- Convolutional Neural Networks
- Source:
- https
- ://www.dragon1.com/terms/convolutional-neural-networks-definition
- Convolutional Neural Networks

### Slide 11
- Vision Transformers divide images into small patches
- .
- They
- use attention to understand relationships between image parts
- .
- Multimodal
- models combine image and text understanding
- .
- They
- are used in image captioning, visual question answering and AI assistants.
- Figure-8 :
- Vision Transformers and
- Multimodal Models
- Source:
- https
- ://www.linkedin.com/pulse/vision-transformers-vit-rise-multi-modal-deep-dr-satupati-jamalaiah-rvdqc/
- Vision Transformers and
- Multimodal
- Models

### Slide 12
- Image generation creates images from text prompts
- .
- Example
- : “A dog carrying a stick in its mouth
- .”
- Diffusion
- models start with random noise and gradually create a meaningful image
- .
- They
- are used in design, education, advertising, entertainment and research visualization.
- Figure-9
- :
- Image Generation and Diffusion Models
- Source:
- https
- ://www.geeksforgeeks.org/artificial-intelligence/diffusion-models-in-machine-learning/
- Image Generation and Diffusion Models

### Slide 13
- Summary of the
- Experiment
- Computer vision is a branch of Artificial Intelligence that helps machines understand images, videos, and camera inputs
- .
- Images
- are represented using pixels,
- gray scale
- values, and RGB color channels
- .
- Image
- processing uses filters, kernels, and convolution to improve images and extract important features
- .
- Major
- computer vision tasks include image classification, object detection, semantic segmentation, and contextual image analysis
- .
- CNNs
- and Vision Transformers are used to learn visual features and recognize patterns in images
- .

### Slide 14
- Next
- Experiment
- T
- opic(s)
- Introduction to Information
- Extraction
- Optical
- Character
- Recognition
- OCR Pipeline
- Field
- Extraction and Field Mapping

### Slide 15
- Quiz/ FAQ’s
- What is computer vision
- ?
- What
- is a pixel in a digital image
- ?
- What
- is the full form of RGB
- ?
- What
- is the difference between
- gray scale
- and RGB images
- ?
- What
- is the role of filters in image processing
- ?
- What
- is convolution in computer vision
- ?
- What
- is image
- classification? What
- is object detection
- ?
- What
- is the use of a bounding box
- ?
- What
- is the difference between CNN and Vision Transformer?

### Slide 16
- R
- eferences/ Articles/ Videos
- References / Articles
- Microsoft
- Learn — Introduction to Computer Vision Concepts
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId3"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/modules/introduction-computer-vision
- /
- Microsoft
- Learn — What is Image Analysis?
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://
- learn.microsoft.com/en-us/azure/ai-services/computer-vision/overview-image-analysis
- Microsoft
- Learn — Get Started with Computer Vision in Azure
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId5"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/modules/get-started-vision-azure
- /
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" b="1" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Videos
- Computer Vision Explained | What is Computer Vision?
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId6"/></a:rPr><a:t>https://www.youtube.com/watch?v=OcycT1Jwsns
- Image Classification
- vs
- Object Detection
- vs
- Image Segmentation
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId7"/></a:rPr><a:t>https://www.youtube.com/watch?v=taC5pMCm70U
- Convolutional Neural Networks Explained
- </a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId8"/></a:rPr><a:t>https://www.youtube.com/watch?v=YRhxdVk_sIs

### Slide 17
- Additional
- learning
- R
- esources
- TensorFlow
- — Computer Vision Tutorials
- </a:r><a:br><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId3"/></a:rPr><a:t>https://
- www.tensorflow.org/tutorials/images
- PyTorch
- —
- TorchVision
- Object Detection
- Fine tuning
- Tutorial
- </a:r><a:br><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://
- docs.pytorch.org/tutorials/intermediate/torchvision_tutorial.html
- Hugging
- Face — Diffusion Models Course
- </a:r><a:br><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId5"/></a:rPr><a:t>https://
- huggingface.co/learn/diffusion-course/en/unit0/1
- Microsoft
- Learn — Introduction to Computer Vision Concepts
- </a:r><a:br><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId6"/></a:rPr><a:t>https://learn.microsoft.com/en-us/training/modules/introduction-computer-vision/

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


================================================================================


# Experiment-3.3 - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Experiment-3.3
# Experiment-3.3

##

## Understanding Vision AI and Information Extraction workflows with Microsoft Foundry Tools.

##

## CO5

##

## Aim

To study AI-based information extraction and understand how structured data can be extracted from unstructured documents and images using OCR, field extraction, field mapping, and data normalization techniques.

## Objectives

- To understand the concept of information extraction in artificial intelligence.

- To study the role of OCR in converting image-based text into machine-readable text.

- To understand field extraction and field mapping.

- To learn how extracted data is normalized, validated, and used in business systems.

- To study applications of information extraction in finance, healthcare, legal, logistics, and business automation.

## Theory

## Introduction to Information Extraction

Information extraction is an important application of artificial intelligence that is used to extract useful and meaningful data from unstructured or semi-structured content, as shown in Figure 1. Unstructured data may be present in scanned documents, images, receipts, invoices, contracts, medical records, business cards, and forms.

AI-based information extraction converts this unstructured data into structured data fields. For example, from an invoice, AI can extract vendor name, invoice number, date, tax amount, payment terms, product details, and total amount. This extracted information can then be stored in a database, spreadsheet, or business application.

The main purpose of information extraction is to reduce manual work, save time, improve accuracy, and support automation in document-based processes.

## Figure 1: Types of information extraction from text, image, audio, and video data.

## Need for Information Extraction

Many organizations process a large number of documents every day. Manual processing of these documents is slow, costly, and may contain human errors. Information extraction helps solve this problem by automatically reading documents and extracting important information.

For example, in finance, it can be used to process invoices and receipts. In healthcare, it can extract patient details and medical information. In logistics, it can extract shipment numbers, addresses, and delivery details. Therefore, information extraction is useful for digital transformation and business workflow automation.

## Working Concept of Information Extraction

AI-based information extraction generally works in two main stages. The first stage is text extraction, and the second stage is field extraction.

In text extraction, the system reads text from documents or images using Optical Character Recognition, also called OCR. In field extraction, the system understands the meaning of the extracted text and maps it to proper data fields.

For example, OCR may extract the text “Invoice No: 12345.” Field extraction identifies “12345” as the invoice number. Similarly, “Total: ₹5000” is mapped as the total amount.

## Optical Character Recognition

Optical Character Recognition, or OCR, is a technology that converts visual text into editable and searchable digital text. Visual text may be present in scanned documents, images, PDFs, screenshots, handwritten forms, receipts, and business cards as shown in Figure 2.

OCR is an important part of information extraction because the accuracy of field extraction depends on the quality of OCR output. If OCR extracts incorrect text, the final extracted fields may also be incorrect.

## Figure 2: Optical Character Recognition for converting images, PDFs, and scanned documents into editable text.

## OCR Pipeline

The OCR pipeline consists of the following stages:

- Image acquisition and input

- Preprocessing and image enhancement

- Text region detection

- Character recognition and classification

- Output generation and post-processing

These stages work together to convert image-based text into usable digital text, as shown in Figure 3.

## Figure 3: OCR workflow for extracting text from an input image.

##

## Image Acquisition and Input

Image acquisition is the first stage of OCR. In this stage, the system receives an input image or document containing text. The input may be a scanned document, mobile photograph, screenshot, PDF page, or video frame.

The quality of the input image is very important. Clear, properly aligned, and high-resolution images give better OCR results, while blurred, tilted, or low-light images may reduce accuracy.

## Preprocessing and Image Enhancement

Preprocessing is used to improve the quality of the input image before text recognition. It helps the OCR system read the text more clearly.

Important preprocessing techniques include noise reduction, contrast adjustment, skew correction, and resolution optimization. Noise reduction removes unwanted marks and dust. Contrast adjustment makes the text more visible. Skew correction straightens tilted documents. Resolution optimization improves low-quality images.

Good preprocessing improves OCR accuracy.

## Text Region Detection

Text region detection is the stage where the system identifies areas of the document that contain text. A document may contain text, images, logos, signatures, tables, stamps, and blank spaces. The OCR system must separate text regions from non-text areas.

This stage also identifies headings, paragraphs, captions, table text, and reading order. Correct reading order is important because the wrong order can change the meaning of the extracted text.

## Character Recognition and Classification

Character recognition is the main stage of OCR. In this stage, the system recognizes letters, numbers, and symbols from the detected text regions.

The system analyzes the shape and pattern of each character and identifies it using trained models. Modern OCR systems use machine learning and deep learning models such as CNNs and transformers. These models can recognize text more accurately even when fonts, sizes, or layouts are different.

Context analysis may also be used to correct mistakes. For example, if OCR reads “Invo1ce,” the system may correct it as “Invoice.”

## Output Generation and Post-Processing

After recognizing the characters, the OCR system generates digital text output. This output may include words, sentences, paragraphs, line breaks, tables, and layout details.

Post-processing improves the final result by applying spelling correction, grammar checking, formatting, confidence scoring, and structure preservation. Confidence scores show how certain the system is about the recognized text.

## Field Extraction

Field extraction is the process of identifying meaningful data fields from OCR output. OCR only tells what text is present, but field extraction tells what the text means.

For example, OCR may extract:

Fourth Coffee

2024-08-15

Subtotal: $6.48

Tax: $0.49

Total: $6.97

Field extraction identifies these as:

Vendor: Fourth Coffee

Date: 2024-08-15

Subtotal: $6.48

Tax: $0.49

Total: $6.97

Thus, field extraction converts raw OCR text into labeled and structured information.

## Difference Between OCR and Field Extraction

OCR and field extraction are connected but different. OCR extracts text from images or documents, while field extraction gives meaning to that text.

For example, OCR may detect the value “₹10,500.” Field extraction identifies whether it is the total amount, tax amount, unit price, or balance amount. Therefore, OCR reads the text, and field extraction understands the text.

## Field Extraction Pipeline

The field extraction pipeline includes:

- OCR output ingestion

- Field detection and candidate identification

- Field mapping and association

- Data normalization and standardization

- Integration with business systems

These steps help convert raw OCR output into useful structured data, as shown in Figure 3.

## Figure 3: Intelligent document processing pipeline for document classification, data extraction, validation, and integration.

## OCR Output Ingestion

OCR output ingestion means taking the text extracted by OCR as input for field extraction. This output may include raw text, text position, confidence scores, page number, layout information, and reading order.

The position of text is very important. For example, a number near the label “Invoice Number” is likely to be an invoice number, while a number near “Total” is likely to be the total amount.

## Field Detection and Candidate Identification

Field detection identifies possible field values from OCR output. A document may contain many names, dates, numbers, and amounts. The system must identify which values are useful.

There are three common approaches:

Template-based detection uses fixed rules and known document layouts. It works well for standard forms.

Machine learning-based detection uses trained models to identify fields from different document formats.

Generative AI-based extraction uses large language models to extract fields according to a given schema, such as vendor name, date, invoice number, and total amount.

## Field Mapping and Association

Field mapping connects extracted values with correct field names. For example, it maps “Fourth Coffee” to vendor name and “$6.97” to total amount.

Field mapping may use proximity analysis, key-value pairing, reading order, named entity recognition, and table processing. Proximity analysis checks how close a value is to its label. Key-value pairing identifies pairs such as “Name: Rachit” or “Date: 15-08-2024.”

## Table and Structured Content Extraction

Many documents contain tables, especially invoices and receipts. These tables may include item names, quantities, unit prices, tax, discounts, and totals.

Table extraction identifies rows, columns, headers, and cell values. It helps map table data correctly. For example, in an invoice table, each row may represent one product, and each column may represent item description, quantity, price, and total.

## Confidence Scoring and Validation

Confidence scoring shows how reliable the extracted text or field value is. A high confidence score means the system is more certain about the result. A low confidence score may require human review.

Validation checks whether the extracted data is correct. For example, in an invoice, the system can check whether item totals and tax match the final total. This improves the accuracy and reliability of information extraction.

## Data Normalization and Standardization

Data normalization converts extracted values into a common and standard format.

For example, dates such as 15/08/2024, 08-15-2024, and August 15, 2024 can be converted into a standard format like 2024-08-15. Currency values such as ₹5,000 and Rs. 5000 can also be standardized.

Text standardization may include correcting capitalization, removing extra spaces, and expanding abbreviations.

## Integration with Business Systems

After extraction, mapping, validation, and normalization, the structured data can be sent to business systems such as databases, accounting software, ERP systems, hospital management systems, or workflow automation tools.

For example, invoice data can be sent to accounting software, patient information can be sent to hospital systems, and shipment data can be sent to logistics tracking systems.

## Applications of Information Extraction

Information extraction is used in many areas. In finance, it is used for invoice processing, receipt scanning, expense claims, and bank statement analysis. In legal work, it is used for contract processing and compliance documents. In healthcare, it is used to extract patient details, diagnosis, medication lists, and billing codes.

It is also used in logistics for shipping documents, purchase orders, tracking numbers, customs forms, and delivery instructions. Business card scanning is another common application where name, company, phone number, email, and job title are extracted.

## Code

# 1. Install OCR tools

!apt-get -qq install tesseract-ocr > /dev/null

!pip -q install pytesseract

# 2. Import libraries

import pytesseract

from PIL import Image, ImageOps

from google.colab import files

from IPython.display import display

# 3. Upload an image

print("Upload an image containing printed English text:")

uploaded = files.upload()

if uploaded:

filename = next(iter(uploaded))

# 4. Open and display the image

image = ImageOps.exif_transpose(Image.open(filename))

display(image)

# 5. Convert to grayscale and extract text

gray_image = ImageOps.grayscale(image)

text = pytesseract.image_to_string(gray_image, lang="eng")

# 6. Display extracted text

print("\nEXTRACTED TEXT:\n")

print(text.strip() or "No text detected. Try a clearer image.")

## Practice Task Questions

- Take a sample invoice image and identify the fields that can be extracted from it, such as invoice number, date, vendor name, tax amount, and total amount.

- Collect a receipt image and list the information that an AI system can extract from it, such as merchant name, purchased items, price, tax, and payment method.

- Take a business card image and identify the structured fields such as name, designation, company name, phone number, email address, and website.

- Prepare a sample scanned document and explain how OCR can convert the text present in the image into editable digital text.

- Take any form or application document and mark the key-value pairs present in it, such as name, address, date of birth, ID number, and contact number.

- Compare a clear document image and a blurred document image, and write how image quality affects OCR accuracy.

- Create a small table showing the difference between OCR and field extraction using any one example document.

- Take an invoice containing line items and identify the table fields such as item name, quantity, unit price, tax, discount, and total.

- Choose any extracted values from a document and normalize them into standard formats, such as date format, currency format, and phone number format.

- Prepare a short report explaining how AI-based information extraction can be used in any one field, such as finance, healthcare, legal documents, logistics, or education.

## Video Links

Azure AI Document Intelligence Hands-On: Analyze, Extract

Azure AI Document Intelligence is awesome! A simple intro.

Introduction to Optical Character Recognition (OCR)

Text detection with Python and OpenCV | OCR using EasyOCR | Computer Vision Tutorial

How to use Document AI

## Additional Resources

- Microsoft Learn: Azure AI Document Intelligence Documentation

Link: https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/

Useful for learning OCR, key-value pair extraction, tables, forms, and document processing using Azure AI.

- Microsoft Learn: Document Intelligence Read OCR Model

Link: https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/prebuilt/read

Useful for understanding how OCR extracts printed and handwritten text from scanned and digital documents.

- Google Cloud: Document AI

Link: https://cloud.google.com/document-ai

Useful for learning document OCR, document classification, layout extraction, and entity extraction.

- Google Cloud: Document AI Extraction Overview

Link: https://docs.cloud.google.com/document-ai/docs/extracting-overview

Useful for understanding custom field extraction, schema-based extraction, and document entity extraction.

- Google Cloud: Enterprise Document OCR

Link: https://docs.cloud.google.com/document-ai/docs/enterprise-document-ocr

Useful for learning how OCR detects text and layout information from different document types.

- AWS: Amazon Textract

Link: https://aws.amazon.com/textract/

Useful for learning automatic extraction of text, handwriting, layout elements, tables, and forms from scanned documents.

- AWS Documentation: Amazon Textract Tables

Link: https://docs.aws.amazon.com/textract/latest/dg/how-it-works-tables.html

Useful for understanding how tables are detected and extracted from documents.

- IBM: What is Intelligent Document Processing?

Link: https://www.ibm.com/think/topics/intelligent-document-processing

Useful for understanding how AI extracts business-critical data from documents for faster decision-making.

- IBM watsonx: Understanding Documents

Link: https://www.ibm.com/docs/en/watsonx/saas?topic=generation-understanding-documents

Useful for learning key-value pair classification and extraction from structured and domain-specific documents.

- IBM watsonx: Text Extraction

Link: https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-api-text-extraction.html?context=wx

Useful for understanding OCR-based text extraction from scanned PDFs and images.

## Textbooks

- Speech and Language Processing — Daniel Jurafsky and James H. Martin

PDF/Online Link: https://web.stanford.edu/~jurafsky/slp3/

- Introduction to Information Retrieval — Christopher D. Manning, Prabhakar Raghavan, Hinrich Schütze

PDF Link: https://nlp.stanford.edu/IR-book/pdf/irbookonlinereading.pdf

- Computer Vision: Algorithms and Applications — Richard Szeliski

PDF/Online Link: https://szeliski.org/Book/

- Dive into Deep Learning—Aston Zhang, Zachary C. Lipton, Mu Li, Alexander J. Smola

PDF Link: https://d2l.ai/d2l-en.pdf

- Artificial Intelligence: Foundations of Computational Agents — David L. Poole and Alan K. Mackworth

Online Book Link: https://artint.info/3e/html/ArtInt3e.html

## Reference Books / Reference Materials

- Optical Character Recognition—Line Eikvil

PDF Link: https://home.nr.no/~eikvil/OCR.pdf

- OCR — Optical Character Recognition Technology — United Nations Statistics Division

PDF Link: https://unstats.un.org/unsd/demographic/sources/census/wphc/dataCapture/docs/Data-Capture_ch06-ABS.pdf

- Natural Language Processing for Information Extraction — Sonit Singh

PDF Link: https://arxiv.org/pdf/1807.02383

- Open Information Extraction — Duc-Thuan Vo and Ebrahim Bagheri

PDF Link: https://arxiv.org/pdf/1607.02784

- LexNLP: Natural Language Processing and Information Extraction for Legal and Regulatory Texts — Michael J. Bommarito II, Daniel Martin Katz, Eric M. Detterman

PDF Link: https://arxiv.org/pdf/1806.03688

---


## 🖥️ PRESENTATION SLIDES


# Experiment-3.3 - All Lecture Slides Text


## Exp 3.3
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
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Unit No. 3                   Experiment No.3.3
- Topic
- : Understanding Vision AI and Information Extraction Workflows with Microsoft Foundry
- Tools
- .
- Dr.Rachit
- Manchanda
- (E-7089)                                     Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026

### Slide 2
- Learning
- Objectives
- After
- completing this experiment, students will be able
- to:
- Understand information extraction in
- AI
- Study
- OCR and its working
- Learn
- field extraction and
- mapping
- Understand
- normalization and validation
- Explore real-world
- applications

### Slide 3
- Recap
- of Previous Experiment
- Computer vision is a branch of Artificial Intelligence that helps machines understand images, videos, and camera inputs.
- Images are represented using pixels, gray scale values, and RGB color channels.
- Image processing uses filters, kernels, and convolution to improve images and extract important features.
- Major computer vision tasks include image classification, object detection, semantic segmentation, and contextual image analysis.
- CNNs and Vision Transformers are used to learn visual features and recognize patterns in images.

### Slide 4
- Figure-1 :
- OCR and Translation Pipeline
- Source
- :
- https://medium.com/towards-applied-generative-
- ai
- /moving-on-to-vlms-from-ocr-though-not-totally-649f32aa0729
- Topic(s
- )
- Introduction to Information Extraction
- Optical Character Recognition
- OCR Pipeline
- Field Extraction and Field Mapping
- Information Extraction and OCR Pipeline in AI

### Slide 5
- Figure-2:
- Information
- Extraction
- Source:
- https
- ://www.researchgate.net/publication/220135843_A_strategy_for_extracting_information_from_semi-structured_web_pages/figures
- Information extraction is an AI technique used to convert
- unstructured data into structured data
- Works on documents like invoices, receipts, contracts, and forms
- Example:
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Invoice → Vendor name, date, total
- amount
- Benefits:
- Reduces manual effort
- Saves time
- Improves accuracy
- Enables automation
- Information Extraction

### Slide 6
- OCR converts
- image-based text into machine-readable text
- Works on scanned documents, PDFs, screenshots, and photos
- Uses:
- Receipt scanning
- Form processing
- Business card reading
- Important Point:
- </a:r><a:br><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Higher image quality → Better OCR accuracy
- Figure-3
- : Optical Character Recognition (OCR)
- Source:
- https
- ://www.globe3.com/news/ocr-integration-in-erp/
- Optical Character Recognition (OCR)

### Slide 7
- OCR works in multiple stages
- :
- Image acquisition (input image)
- Pre-processing
- (improve quality)
- Text detection (locate text regions)
- Character recognition (identify text)
- Output generation (digital text)
- This
- pipeline converts images into usable text data
- Figure-4
- :OCR Pipeline
- Source:
- https
- ://theailearner.com/2019/05/28/optical-character-recognition-pipeline/
- OCR Pipeline

### Slide 8
- Preprocessing:
- Removes noise and improves contrast
- Corrects tilted images
- Text Detection:
- Identifies areas containing text
- Separates text from
- images/logos
- Recognition:
- Uses AI models to read characters
- Post-processing:
- Corrects errors and formats output
- Figure-5
- :Key OCR Stages
- Source:
- https
- ://www.highradius.com/resources/Blog/3-steps-to-measuring-effectiveness-of-ocr-and-cash-application-automation/
- Key OCR Stages

### Slide 9
- Field extraction converts OCR text into
- meaningful structured data
- Example:
- Raw Text:
- Date: 15/08/2024
- Structured Field:
- Date →
- 2024-08-15
- Helps systems understand and use extracted data
- Figure-6
- : Field Extraction
- Source:
- https
- ://www.geeksforgeeks.org/nlp/information-extraction-in-nlp/
- Field Extraction

### Slide 10
- Figure-7 :
- OCR
- vs
- Field Extraction
- Source:
- https
- ://parseur.com/blog/
- ocr
- -
- vs
- -document-processing
- OCR
- vs
- Field Extraction
- OCR
- Field Extraction
- Reads text
- Understands meaning
- Output = raw text
- Output = structured data
- Example:
- </a:r><a:br><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1800" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>₹5000 →
- OCR: value
- Field Extraction: total
- amount
- Both
- are required for complete document processing

### Slide 11
- Steps involved:
- OCR output ingestion
- Field detection (find useful values)
- Field mapping (assign labels)
- Data normalization (standard format)
- Validation (check correctness)
- Integration with systems
- Converts
- raw text into business-ready data
- Figure-8 :
- PDF Data
- Extraction
- Source:
- https
- ://www.docupipe.ai/blog/pdf-data-extraction
- Field Extraction Pipeline

### Slide 12
- Summary of the
- Experiment
- Information extraction is an AI technique that converts unstructured data (documents, images) into structured and usable data fields for automation
- .
- OCR plays a key role by extracting text from images and documents, forming the foundation for further data processing.
- Field extraction and mapping help in understanding the meaning of extracted text and organizing it into structured formats like names, dates, and amounts.
- The complete pipeline includes OCR, detection, mapping, normalization, and validation, ensuring accurate and reliable data extraction.

### Slide 13
- Quiz/ FAQ’s
- What is information extraction in artificial intelligence?
- What
- type of data is converted into structured form using information extraction?
- What
- is the full form of OCR?
- What
- is the main purpose of Optical Character Recognition?
- Name
- any two stages of the OCR pipeline.
- What
- is preprocessing in OCR? Why is it important?
- What
- is field extraction? What is the difference between OCR and field extraction?

### Slide 14
- R
- eferences/ Articles/ Videos
- References / Articles
- Microsoft Learn – Introduction to Document Intelligence
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId3"/></a:rPr><a:t>https://learn.microsoft.com/en-us/azure/ai-services/document-intelligence/overview
- Microsoft
- Learn – Optical Character Recognition (OCR)
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/overview-ocr
- IBM
- – What is Optical Character
- Recognition?
- https://www.ibm.com/topics/ocr
- </a:r><a:br><a:rPr lang="en-US" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1700" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t/></a:r><a:br><a:rPr lang="en-IN" sz="1700" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" b="1" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>Videos
- What is OCR? | Optical Character Recognition
- Explained
- https://www.youtube.com/watch?v=5qg4j8zqZ3k
- </a:r><a:br><a:rPr lang="en-IN" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1600" b="1" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>AI
- Explained | Intelligent Document
- Processing
- https://www.youtube.com/watch?v=Gm8Qd9Xv7hY
- </a:r><a:br><a:rPr lang="en-IN" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1600" b="1" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>OCR
- Tutorial using Python and
- Tesseract
- </a:r><a:br><a:rPr lang="en-IN" sz="1600" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="1600" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId8"/></a:rPr><a:t>https://www.youtube.com/watch?v=Hj1d9T9UQ9Q

### Slide 15
- Additional
- learning
- R
- esources
- TensorFlow
- – Image and Document Processing Tutorials
- </a:r><a:br><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId3"/></a:rPr><a:t>https://
- www.tensorflow.org/tutorials
- PyTorch
- – Computer Vision and OCR Tutorials
- </a:r><a:br><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId4"/></a:rPr><a:t>https://pytorch.org/tutorials/
- Hugging
- Face – Document AI and NLP Course
- </a:r><a:br><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId5"/></a:rPr><a:t>https://huggingface.co/learn
- OpenCV
- Documentation – Image Processing and OCR Basics
- </a:r><a:br><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/><a:hlinkClick r:id="rId6"/></a:rPr><a:t>https://docs.opencv.org/

### Slide 16
- Class-Wise
- Feedback
- We value your feedback! Please take a moment to share your experience in today's session. Your responses will help us improve future classes.

### Slide 17
- Thank You
- For queries
- Email:
- rachit.ece@cumail.in


---


================================================================================


# Course Overview - Complete Study Material


## 📘 LECTURE NOTES & EXPLANATIONS


### Computer Requirements
# Computer Requirements

## Practical Course Environment and Tools

This practical course is designed to provide hands-on experience in data preprocessing, exploratory data analysis, supervised machine learning, and Azure-based AI applications. The course is aligned with Microsoft AI-901 fundamentals and real-world engineering use cases. All experiments will be implemented using Python in Google Colab and Microsoft Azure / Microsoft Foundry tools, enabling students to work in a cloud-based, collaborative, and hardware-independent environment suitable for modern AIML and Azure AI-based applications.

## Development Environments

Primary AIML Platform: Google Colaboratory / Google Colab

Cloud and AI Platform: Microsoft Azure Portal and Microsoft Foundry Tools

Certification Alignment: Microsoft Azure AI-901

## Programming Language

Python 3

## Libraries and Tools Used

✅ Data Preprocessing and Analysis

pandas, NumPy

✅ Data Visualization

Matplotlib

✅ Supervised Machine Learning

scikit-learn

✅ AI and Machine Learning Fundamentals

Artificial Intelligence concepts

Machine Learning concepts

Generative AI models

AI agent systems

✅ Azure AI Tools and Services

Azure Machine Learning

Azure AI services

Natural Language Processing tools

Speech AI tools

Computer Vision tools

Information Extraction workflows

Microsoft Foundry tools

✅ Generative AI and NLP Applications

Text analysis

Prompt-based AI applications

Language understanding

Sentiment-based applications

Document and information extraction

✅ Speech and Vision AI Applications

Speech processing workflows

Vision AI architecture

Image-based AI applications

Computer vision-based analysis

✅ Hardware–Software Integration

No physical hardware is required. The course uses cloud-based platforms, APIs, AI services, and Microsoft Foundry tools for practical AI implementation, analysis, and deployment readiness.

---


### Course Information
# Course Information

SN

Course

Code:

Course Name:

AI Applications Lab

L

T

P

S

C

CH

Course Type

1

0

0

0

3

1

3

Practical

26ECP-

102

Course Coordinator:

Dr. Rachit Manchanda

Pre-requisites:

Mathematics

Co-Requisite

Nil

Anti-Requisite

Nil

---


### Course Introduction, Objectives and Outcomes
# Course Introduction, Objectives and Outcomes

## A.     COURSE DESCRIPTION

This course provides hands-on exposure to data preprocessing, exploratory data analysis, and supervised machine learning algorithms, forming the foundation of AI and machine learning workflows. Students learn to analyze real-world datasets, build and evaluate classification models, and understand core concepts of Artificial Intelligence, Machine Learning, and Generative AI. The course also introduces Azure AI tools and services, including NLP, speech processing, computer vision, and information extraction using Microsoft Foundry, enabling learners to develop practical and scalable AI-driven solutions aligned with AI-901 fundamentals.

## B.     COURSE OBJECTIVES

The objective of this course is to equip students with foundational knowledge and practical skills in data preprocessing, exploratory data analysis, and supervised machine learning, along with an understanding of core Artificial Intelligence, Machine Learning, and Generative AI concepts. The course aims to develop competency in using Azure AI tools and services for NLP, speech, vision, and information extraction, enabling learners to design and implement scalable AI-driven solutions aligned with industry practices and AI-901 fundamentals.

## C.     COURSE OUTCOMES

##

## CO No

##

## Statement

##

## CO1

## Recognize fundamental concepts of AI, ML, Generative AI, and Azure services, including NLP, speech, vision, and AI agents.

## CO2

## Describe and apply data analysis techniques by performing EDA and generating meaningful visualizations using Matplotlib, NumPy, and Pandas.

##   CO3

## Apply supervised learning methods to build, train, and evaluate classification models using AIML techniques and model comparison frameworks.

##

## CO4

## Evaluate and examine Azure AI/ML services, including AutoML, NLP, speech AI, computer vision, and information extraction workflows.

##

## CO5

## Implement AI-driven solutions using Azure and Microsoft Foundry across generative AI, NLP, speech, vision, and information extraction tasks.

---


### Course Syllabus and Suggestive Readings
# Course Syllabus and Suggestive Readings

Unit

Course Content / Experiment

Contact Hours

CO Mapping

Unit-1

Data Pre-processing and AIML Algorithms

15

Experiment No. 1

Introduction to Data Pre-processing, Pandas, NumPy & Matplotlib for Data Analysis.

CO1, CO2

Experiment No. 2

Perform exploratory data analysis (EDA) on a real-world dataset to identify patterns, correlations, and trends using descriptive statistics and visualizations.

CO2

Experiment No. 3

Understand supervised learning to train and develop classifier models.

CO3

Experiment No. 4

Build a classification model by using different machine learning algorithms.

CO3

Unit-2

AI and Machine Learning Fundamentals with Azure AI Tools

15

Experiment No. 1

Introduction to Artificial Intelligence and Machine Learning Concepts.

CO1

Experiment No. 2

Understanding Azure Machine Learning, Generative AI Models, and AI Agent Systems.

CO1

Experiment No. 3

Exploring Generative AI, Natural Language Processing and Azure AI Tools.

CO4

Unit-3

Azure AI Services for NLP, Speech Processing, and Computer Vision

15

Experiment No. 1

Understanding Natural Language Processing and Speech AI Concepts with Microsoft Tools.

CO5

Experiment No. 2

Analysis of Speech Processing Workflows and Vision AI Architectures Using Microsoft Foundry.

CO5

Experiment No. 3

Understanding Vision AI and Information Extraction Workflows with Microsoft Foundry Tools.

CO5

TEXT BOOKS

T1: Data Science from Scratch, Joel Grus, Shroff Publisher Publisher /O’Reilly Publisher Media, 2019.

https://drive.google.com/file/d/1qv89LVaEshX9hcmSS9KDMsvBP-UYC78h/view?usp=sharing

T2: Artificial Intelligence: A Modern Approach, 3rd Edition, by Stuart Russell and Peter Norvig, Pearson Publisher, 2010.

https://drive.google.com/file/d/1G-s5fsBh5rLMdWmIYvyeI2zclcDCAA_D/view?usp=sharing

T3: Machine Learning, Tom Mitchell, McGraw Hill, 2017.

https://drive.google.com/file/d/1IBgLq2GvyEXURAPfSDm-Eep94X0vYXDb/view?usp=sharing

T5: Microsoft Azure Fundamentals AZ-900 Guide by Jim Cheshire, 3rd Edition (2023), Microsoft Press

T6: Exam Ref AZ-900 Microsoft Azure Fundamentals by Michael Collier & Robin Shahan, 2nd Edition (2020), Microsoft Press

REFERENCE BOOKS

RB1: Philipp Janert, Data Analysis with Open-Source Tools, Shroff Publisher Publisher /O’Reilly Publisher Media.

https://drive.google.com/file/d/1SVtjE5XEih7_aU433_cAJKiDF41-KuzU/view?usp=sharing

RB2: Andreas C. Müller & Sarah Guido ,Introduction to Machine Learning with Python,published by O'Reilly Media

https://www.nrigroupindia.com/e-book/Introduction%20to%20Machine%20Learning%20with%20Python%20(%20PDFDrive.com%20)-min.pdf

RB3: Ms.Anitha Patibandla, Dr.B.Jyothi, Ms.K.Bhavana,ARTIFICIAL INTELLIGENCE & MACHINE LEARNING,Lecture notes

https://mrcet.com/downloads/digital_notes/ECE/III%20Year/AI%20&%20ML%20DIGITAL%20NOTES.pdf

---


### Netiquette Guidelines
# Netiquette Guidelines

Netiquette is etiquette for the internet, guidelines and good practices for online communication in emails, discussion forums, and chat rooms.

Please practice the following guidelines when posting comments in the course:

- Format your text so it is easy to read. Try to use standard paragraph spacing, indentation, and legible font. Try to be consistent with your formatting, including font size, color, etc.

- Be concise and to the point in your communication. Limit discussion forum posts to a few paragraphs. Proofread and edit your work before posting.

- AVOID THE USE OF ALL CAPS as this may be interpreted as shouting. All lowercase letters also make text more difficult to read. Use standard punctuation. Remember what your teacher taught you in primary school about good punctuation and spelling.

- Avoid 'texting' abbreviations such as OMG.

- Avoid using humor and sarcasm, as they are often difficult to detect in written communication. It is okay to sparingly use emoticons to communicate subtleties or emotions that are more obvious in spoken communication.

- Flaming is not proper in our courses (a rant about someone or some topic). Practice civil discussion.

- Respect the privacy of communication within a course. Do not publicly forward the comments of classmates to others outside of the course.

- Stay on topic in a discussion.

- Be respectful.

- Participants have varying degrees of sensitivity, and that even some well-meaning constructive suggestions (e.g., comments about broken links, typo, and misspellings) may be misconstrued as public criticism. Therefore, please refrain from sharing comments in ways that might be misinterpreted, or do so privately when appropriate.

(Any violation to the above points if reported by the teacher may lead to disciplinary action against the student)

---


## 🖥️ PRESENTATION SLIDES


# Course Overview - All Lecture Slides Text


## 1. Day-1 (Zero Lecture)
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
- /
- SEMESTER:Ist
- SUBJECT
- NAME-AI APPLICATIONS LAB
- (SUBJECT
- CODE-26ECP-102
- )
- Dr.Rachit
- Manchanda
- (E-7089)
- Designation:-Assistant Professor
- Academic Session
- 2026-27
- Odd
- Semester
- July-Dec 2026
- CUmail
- -ID :
- rachit.ece@cumail.in

### Slide 2
- Vision of University
- “To be globally recognized as a Centre of Excellence for Research, Innovation, Entrepreneurship and disseminating knowledge by providing inspirational learning to produce professional leaders for serving the society.”
- 1

### Slide 3
- Mission of University
- M1 :
- Providing world class infrastructure, renowned academicians and ideal environment for Research, Innovation, Consultancy and Entrepreneurship relevant to the society.
- M2 :
- Offering programs & courses in consonance with National policies for nation building and meeting global challenges.
- 2

### Slide 4
- Mission of University
- M3
- :	Designing Curriculum to match International standards, needs of Industry, civil 	society and for inculcation of traits of Creative Thinking and Critical Analysis as well as Human and Ethical values.
- M4
- :	Ensuring students delight by meeting their aspirations through blended learning, corporate mentoring, professional grooming, flexible curriculum and healthy atmosphere based on co-curricular and extra-curricular activities.
- 3

### Slide 5
- Mission of University
- M5
- :	Creating a scientific, transparent and objective examination/evaluation system to ensure an ideal certification.
- M6
- :	Establishing strategic relationships with leading National and International corporates and universities for academic as well as research collaborations.
- 4

### Slide 6
- Mission of University
- M7:
- Contributing for creation of healthy, vibrant and sustainable society by involving in Institutional Social Responsibility (ISR) activities like rural development, welfare of 	senior citizens, women empowerment, community service, health and hygiene awareness and environmental protection.
- 5

### Slide 7
- Vision of Department
- To be recognized as a leading
- engineering
- department through effective teaching practices and excellence in research and innovation for creating competent professionals with ethics, values and entrepreneurial attitude to deliver service to society and to meet the current industry standards at the global level.
- 6

### Slide 8
- Mission of Department
- M1
- :	To provide practical knowledge using state-of-the-art technological support for the experiential learning of our students.
- M2
- :	To provide industry recommended curriculum and transparent assessment for quality learning experiences.
- M3
- :	To create global linkages for interdisciplinary collaborative learning and research.
- 7

### Slide 9
- Program Educational Objectives (PEOs)
- PEO 1:
- To produce
- engineering
- graduate engineers with an ability to comprehend, understand and analyze real life problems for providing sustainable solutions in the light of disruptive technologies.
- PEO 2:
- To inculcate life-long learning skills in graduates preparing them for work in changing environments and multidisciplinary teams in order to enhance their capability being globally employable.
- </a:r><a:br><a:rPr lang="en-US" sz="3000" b="1" i="0" u="none" strike="noStrike" cap="none" dirty="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:rPr></a:br><a:endParaRPr lang="en-US" sz="3000" b="1" i="0" u="none" strike="noStrike" cap="none" dirty="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:endParaRPr></a:p></p:txBody></p:sp><p:sp><p:nvSpPr><p:cNvPr id="7" name="TextBox 6"/><p:cNvSpPr txBox="1"/><p:nvPr/></p:nvSpPr><p:spPr><a:xfrm><a:off x="8709003" y="85987"/><a:ext cx="284052" cy="307777"/></a:xfrm><a:prstGeom prst="rect"><a:avLst/></a:prstGeom><a:noFill/></p:spPr><p:txBody><a:bodyPr wrap="none" rtlCol="0"><a:spAutoFit/></a:bodyPr><a:lstStyle/><a:p><a:r><a:rPr lang="en-IN" dirty="0" smtClean="0"/><a:t>8

### Slide 10
- Program Outcome (POs)
- PO1:
- Engineering knowledge: Apply the knowledge of mathematics, science, engineering fundamentals and an engineering specialization to the solution of complex engineering problems.
- PO2:
- Problem analysis: Identify, formulate, review research literature and analyze complex engineering problems reaching substantiated conclusions using first principles mathematics, natural sciences and engineering sciences.
- PO3:
- Design/development of solutions: Design solutions for complex engineering problems and design system components or processes that meet the specified needs with appropriate consideration for the public health and safety and the cultural, societal, and environmental considerations.
- PO4:
- Conduct investigations of complex problems: Use research-based knowledge and research methods including design of experiments, analysis and interpretation of data and synthesis of the information to provide valid conclusions.
- </a:r><a:br><a:rPr lang="pl-PL" sz="3000" b="1" i="0" u="none" strike="noStrike" cap="none" dirty="0" smtClean="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:rPr></a:br><a:endParaRPr lang="pl-PL" sz="3000" b="1" i="0" u="none" strike="noStrike" cap="none" dirty="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:endParaRPr></a:p></p:txBody></p:sp><p:sp><p:nvSpPr><p:cNvPr id="7" name="TextBox 6"/><p:cNvSpPr txBox="1"/><p:nvPr/></p:nvSpPr><p:spPr><a:xfrm><a:off x="8709003" y="85987"/><a:ext cx="284052" cy="307777"/></a:xfrm><a:prstGeom prst="rect"><a:avLst/></a:prstGeom><a:noFill/></p:spPr><p:txBody><a:bodyPr wrap="none" rtlCol="0"><a:spAutoFit/></a:bodyPr><a:lstStyle/><a:p><a:r><a:rPr lang="en-IN" dirty="0" smtClean="0"/><a:t>9

### Slide 11
- Program Outcome (POs
- ) (cont..)
- PO5:
- Modern tool usage: Create, select, and apply appropriate techniques, resources and modern engineering and IT tools including prediction and modeling to complex engineering activities with an understanding of the limitations.
- PO6:
- The Engineer and Society: Apply reasoning informed by the contextual knowledge to assess societal, health, safety, legal and cultural issues and the consequent responsibilities relevant to the professional engineering practice.
- PO7:
- Environment and sustainability: Understand the impact of the professional engineering solutions in societal and environmental contexts, and demonstrate the knowledge of, and need for sustainable development.
- PO8:
- Ethics: Apply ethical principles and commit to professional ethics and responsibilities and norms of the engineering practice.
- PO9:
- Individual and teamwork: Function effectively as an individual, and as a member or leader in diverse teams, and in multidisciplinary settings.
- </a:r><a:br><a:rPr lang="pl-PL" sz="3000" b="1" i="0" u="none" strike="noStrike" cap="none" dirty="0" smtClean="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:rPr></a:br><a:endParaRPr lang="pl-PL" sz="3000" b="1" i="0" u="none" strike="noStrike" cap="none" dirty="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:endParaRPr></a:p></p:txBody></p:sp><p:sp><p:nvSpPr><p:cNvPr id="7" name="TextBox 6"/><p:cNvSpPr txBox="1"/><p:nvPr/></p:nvSpPr><p:spPr><a:xfrm><a:off x="8709003" y="85987"/><a:ext cx="284052" cy="307777"/></a:xfrm><a:prstGeom prst="rect"><a:avLst/></a:prstGeom><a:noFill/></p:spPr><p:txBody><a:bodyPr wrap="none" rtlCol="0"><a:spAutoFit/></a:bodyPr><a:lstStyle/><a:p><a:r><a:rPr lang="en-IN" dirty="0" smtClean="0"/><a:t>9

### Slide 12
- Program Outcome (POs
- ) (cont..)
- PO10:
- Communication: Communicate effectively on complex computer science engineering activities with the engineering community like CSI society at large, such as, being able to comprehend and write effective reports and design documentation, make effective presentations, and give and receive clear instructions.
- PO11:
- Project management and finance: Demonstrate knowledge and understanding of the computer science engineering and management principles and apply these to one’s own work, as a member and leader in a team, to manage projects and in multidisciplinary environments.
- PO12:
- Life-long learning: Recognize the need for, and have the preparation and ability to engage in independent and life- long learning in the broadest context of computer science engineering changes
- PO13:
- Critical Thinking: Develop the ability to critically
- analyse
- engineering challenges and synthesize innovative solutions.
- </a:r><a:br><a:rPr lang="pl-PL" sz="3000" b="1" i="0" u="none" strike="noStrike" cap="none" dirty="0" smtClean="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:rPr></a:br><a:endParaRPr lang="pl-PL" sz="3000" b="1" i="0" u="none" strike="noStrike" cap="none" dirty="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:endParaRPr></a:p></p:txBody></p:sp><p:sp><p:nvSpPr><p:cNvPr id="7" name="TextBox 6"/><p:cNvSpPr txBox="1"/><p:nvPr/></p:nvSpPr><p:spPr><a:xfrm><a:off x="8709003" y="85987"/><a:ext cx="284052" cy="307777"/></a:xfrm><a:prstGeom prst="rect"><a:avLst/></a:prstGeom><a:noFill/></p:spPr><p:txBody><a:bodyPr wrap="none" rtlCol="0"><a:spAutoFit/></a:bodyPr><a:lstStyle/><a:p><a:r><a:rPr lang="en-IN" dirty="0" smtClean="0"/><a:t>9

### Slide 13
- Program Outcome (POs
- ) (cont..)
- PO14:
- Multidisciplinary Knowledge: Integrate knowledge from various disciplines to design systems or solve problems in interdisciplinary domains.
- PO15:
- Leadership: Exhibit leadership and decision-making capabilities in engineering and societal contexts.
- PO16:
- Global Perspective: Demonstrate awareness of global issues and trends and their implications for professional practice.
- PO17:
- Entrepreneurship: Apply engineering principles to identify business opportunities and create innovative products or services
- </a:r><a:br><a:rPr lang="pl-PL" sz="3000" b="1" i="0" u="none" strike="noStrike" cap="none" dirty="0" smtClean="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:rPr></a:br><a:endParaRPr lang="pl-PL" sz="3000" b="1" i="0" u="none" strike="noStrike" cap="none" dirty="0"><a:solidFill><a:schemeClr val="bg2"/></a:solidFill><a:latin typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:ea typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" panose="020F0502020204030204" pitchFamily="34" charset="0"/><a:sym typeface="Arial"/></a:endParaRPr></a:p></p:txBody></p:sp><p:sp><p:nvSpPr><p:cNvPr id="7" name="TextBox 6"/><p:cNvSpPr txBox="1"/><p:nvPr/></p:nvSpPr><p:spPr><a:xfrm><a:off x="8709003" y="85987"/><a:ext cx="284052" cy="307777"/></a:xfrm><a:prstGeom prst="rect"><a:avLst/></a:prstGeom><a:noFill/></p:spPr><p:txBody><a:bodyPr wrap="none" rtlCol="0"><a:spAutoFit/></a:bodyPr><a:lstStyle/><a:p><a:r><a:rPr lang="en-IN" dirty="0" smtClean="0"/><a:t>9

### Slide 14
- Program Specific Outcome (PSOs)
- PSO 1: Empowering the students for continuous learning and deliver efficient solutions for emerging challenges in the computation domain.
- PSO 2: Ability to apply standard software engineering principles to develop viable solutions for Information Technology Enabled Services (ITES).
- 10

### Slide 15
- CHANDIGARH
- UNIVERSITY
- Academic
- Calendar
- for
- the
- Session
- 2026-
- 27
- Version
- 1.3
- f
- For
- University
- Institute
- of
- Computing]
- ODD
- SEMESTER:
- JUL-
- DEC
- 2026
- Date
- Day
- Activity
- 01-07-
- 2026
- Wed
- Start
- of
- registration
- 2nd
- Year onward
- students
- [All
- Programs
- of
- UIC]
- for
- ODD
- Semester
- [01.07.2026
- to
- 13.07.2026]
- 14-07-
- 2026
- Tue
- Start
- of
- Odd
- Semester-
- Old
- Batches
- [All
- Programs
- of
- UIC]
- 20-07-
- 2026
- Mon
- Orientation
- &
- Induction
- 1st
- Year
- [All
- Programs
- of
- UIC]
- Batch
- I
- [20.07.2026
- to
- 25.07.2026]
- 21-07-
- 2026
- Tue
- Start
- of
- Odd
- Semester-
- 1st
- Year,
- [All
- Programs
- of
- UIC]
- Batch
- I
- 24-08-
- 2026
- Mon
- Orientation
- &
- Induction
- 1st
- Year,
- Batch
- II
- [24.08.2026
- to
- 26.08.2026]
- 25-08-
- 2026
- Tue
- Start
- of
- Odd
- Semester
- 1st
- Year,
- [All
- Programs
- of
- UIC]
- Batch
- II
- 3
- 1
- -
- 08-
- 2026
- Mon
- In
- Semester
- Test
- [IST]
- -
- 01,
- All
- Years
- [All
- programs
- of
- UIC]
- and
- 1st
- year,
- Batch-
- 1
- [31.08.2026
- to
- 05.09.2026]
- 18-09-
- 2026
- Fri
- Fresher's
- Party-
- 2026
- Intake
- [All
- Programs
- of
- UIC]
- 26-09-
- 2026
- Sat
- Orientation
- &
- Induction
- [International
- Students]
- 1st
- Year [All
- Programs
- of
- UIC]
- 28-09-
- 2026
- Mon
- Practical
- In
- Semester
- Test
- [IST]
- [28.09.2026
- to
- 03.10.2026]

### Slide 16
- CHANDIGARH
- UNIVERSITY
- Academic
- Calendar
- for
- the
- Session
- 2026-
- 27
- Version
- 1.3
- f
- For
- University
- Institute
- of
- Computing]
- ODD
- SEMESTER:
- JUL-
- DEC
- 2026
- Date
- Day
- Activity
- 05-10-
- 2026
- Mon
- Value
- Added
- Courses
- (VAC)
- Week
- [05.10.2026
- to
- 09.10.2026]
- *
- 22-10-
- 2026
- Thu
- In
- Semester
- Test
- [IST]
- -
- 02
- All
- Years
- [All
- Programs
- of
- UIC]
- [22.10.2026
- to
- 28.10.2026]
- 09-11-
- 2026
- Mon
- Diwali
- Break
- for
- Students [09.11.2026
- to
- 11.11.2026]
- 13-11-
- 2026
- Fri
- Last
- Teaching
- Day
- All
- Years
- [All
- Programs
- of
- UIC]
- 16-11-
- 2026
- Mon
- End
- Semester
- Practical
- Exam
- Regular
- &
- Reappear-
- [16.11.2026
- to
- 20.11.2026]
- 23-11-
- 2026
- Mon
- End
- Semester
- Theory
- Exams-
- Regular
- &
- Reappear-
- [23.11.2026
- to
- 19.12.2026]
- 15-12-
- 2026
- Tue
- Winter
- Term
- 2026
- {15.12.2026
- to
- 28.12.2026]
- *
- 19-12-
- 2026
- Sat
- End
- of
- Odd
- Semester
- All
- Years
- [All
- Programs
- of
- UIC]
- 21-12-
- 2026
- Mon
- Start
- of
- Registration
- for
- Even
- Semester
- [21.12.2026
- to
- 03.01.2027]
- 02-01-
- 2027
- Sat
- Announcement
- of
- Results
- Note:
- Saturd
- a
- y
- on
- 25
- th
- July
- 2026
- will
- be
- an
- Academic
- day
- f
- or
- Ba
- tch
- 2026
- [All
- Programs
- ]
- The
- regu
- lar
- time
- t
- a
- ble
- of
- Monday
- will
- be
- followed.

### Slide 17
- Course Information
- Prerequisite
- L
- T   P
- S   C  CH
- Mathematics
- 0
- 0
- 0
- 3   1   3
- Objectives
- The objective of this course is to equip students with foundational knowledge and practical skills in data preprocessing, exploratory data analysis, and supervised machine learning, along with an understanding of core Artificial Intelligence, Machine Learning, and Generative AI concepts. The course aims to develop competency in using Azure AI tools and services for NLP, speech, vision, and information extraction, enabling learners to design and implement scalable AI-driven solutions aligned with industry practices and
- AI-901
- fundamentals.
- 16

### Slide 18
- Course Outcomes
- 17

### Slide 19
- This course focuses on Outcome Based Learning (OBE), providing a comprehensive understanding of data pre-processing techniques, Artificial Intelligence and Machine Learning (AIML) algorithms, and their applications in real-time scenarios. It equips students with essential skills to manipulate and analyze data, develop machine learning models, and integrate AI solutions with hardware for real-world engineering problems.
- The AI Application Lab trains students in
- practical, job-relevant skills
- such as data preprocessing, model building, evaluation, and deployment using Python,
- Scikit
- -learn,
- TensorFlow
- , etc. The lab encourages the use of
- real-world datasets and business-relevant problems
- , aligning academic learning with what industry expects in domains like healthcare, finance, retail, and
- cybersecurity
- .
- In the first year of your engineering,
- students
- will learn
- about AI Applications Lab.
- Importance
- of Subject

### Slide 20
- Source:
- https://link.springer.com/chapter/10.1007/978-3-031-06636-8_4
- Disruptive technology is an
- innovation
- that significantly alters the way that consumers, industries, or businesses operate.
- Figure- 1:
- Disruptive Technologies
- Disruptive Technologies

### Slide 21
- Applications
- of the Subject
- Figure-2
- :Application of
- AI
- Source:
- https
- ://
- techvidvan.com/tutorials/artificial-intelligence-applications
- /
- 18

### Slide 22
- Syllabus
- (
- Practical
- )
- 19

### Slide 23
- Syllabus
- (
- Practical
- )
- 19
- CO Mapping

### Slide 24
- Syllabus
- (
- Practical
- )
- 19
- CO Mapping

### Slide 25
- Text and R
- eference Books
- 27

### Slide 26
- E-learning Resources
- 1
- . Google Machine Learning Crash Course
- https://
- developers.google.com/machine-learning/crash-course
- </a:r><a:br><a:rPr lang="en-IN" sz="2000" dirty="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr></a:br><a:r><a:rPr lang="en-IN" sz="2000" b="1" dirty="0" smtClean="0"><a:latin typeface="Calibri" pitchFamily="34" charset="0"/><a:cs typeface="Calibri" pitchFamily="34" charset="0"/></a:rPr><a:t>2
- .
- Kaggle
- Learn – Python, Pandas, and Machine
- Learning
- https://
- www.kaggle.com/learn
- 3. YouTube
- –
- StatQuest
- with Josh
- Starmer
- https
- ://
- www.youtube.com/user/joshstarmer
- 4
- .
- Towards Data Science – Exploratory Data Analysis Guide
- https://towardsdatascience.com/exploratory-graph-analysis-3d4f9c63e92f/
- 27

### Slide 27
- Content Beyond Syllabus
- 28
- S.
- No.
- Title
- Objectives
- 1
- Credit
- card
- Default prediction
- To
- address
- this
- issue,
- we
- can
- predict
- potential
- default
- accounts
- based
- on
- certain
- attributes.
- The
- idea
- is
- that
- the
- earlier
- the
- potential
- default
- accounts
- are detected,
- the lower the losses we will embrace.
- 2
- Stock Market Analysis and Prediction
- Many
- analysts
- and
- scholars
- have
- always
- been
- fascinated
- by
- stock
- market
- forecasting. According
- to
- popular
- belief,
- stock
- markets
- are
- simply
- a
- random
- walk,
- and
- attempting
- to
- predict them. Because of the many variables involved, predicting stock prices is a difficult
- task
- in
- and
- of
- it.
- The
- market
- operates
- like
- a
- voting
- machine
- in
- the
- near term, but it behaves like a weighing machine in the long run, allowing for the prediction
- of
- market
- movements
- over
- a
- longer
- timescale.
- 3
- Toxic
- comment
- classification
- In this project, you want to create a model that predicts to classify comments into different categories. Comments in social media are often abusive and insulting. Organizations often want to ensure that conversations don’t get too negative. This project
- was
- a
- Kaggle
- challenge,
- where
- the
- participants
- had
- to
- suggest
- a
- solution
- for classifying toxic comments in several categories using NLP methods.

### Slide 28
- Assessment Model
- 29

### Slide 29
- 3
- 0
- Internal & External Exam Evaluation Components (Practical)
- S
- No.
- Direct Evaluation Instruments
- Weightage
- of actual
- conduct
- Assessment Tool
- Skills
- Evaluated
- Employ
- ability
- Linkage (Industry Needs)
- Frequency
- of Task
- Final Weightage
- in Internal
- Assessment
- /External Evaluation
- 1
- Unit-1 Practical Evaluation
- 15
- marks
- Conduct, Viva Voce, Written test
- Data cleaning, feature engineering, Data manipulation, Data visualization
- Data Analyst, BI Developer
- 1
- 15
- 2
- Unit-2 Practical Evaluation
- 15
- marks
- Viva Voce, Written test
- Azure AI tools, including Azure ML, NLP services, and AI agent systems.
- Cloud Engineer, Azure Administrator, and AI Support Associate
- 1
- 15
- 3
- Unit–3 Practical Evaluation (Azure
- AI-901
- Practice
- Test)
- 15
- marks
- Azure Portal &
- AI-901
- Practice Test
- Azure AI services for Natural Language Processing, Speech AI, Computer Vision, and information extraction
- AI Engineer, Azure AI Developer, Computer Vision Engineer, and Cloud AI Support Associate
- 1
- 15
- 4
- Lab MST
- 15 Marks
- Conduct, Viva Voce, Written test
- 1
- 15
- 5
- External
- Exam
- 40
- Marks
- Project Implementation
- Output and Project File
- 1
- Per
- Sem
- 40
- 6
- Azure
- AI-901
- Certification
- Non
- Graded but    Mandatory
- 1
- Per
- Sem
- NA

### Slide 30
- Thank You
- 27


---


================================================================================

