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
