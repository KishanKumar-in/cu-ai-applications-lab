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
