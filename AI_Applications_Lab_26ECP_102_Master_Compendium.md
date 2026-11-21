# AI APPLICATIONS LAB (CONT_26ECP-102 / 26ECP-102)
## Master Examination & Lab Practical Compendium — Units 1, 2 and 3

**Course:** AI Applications Lab (`CONT_26ECP-102` / `26ECP-102`)  
**Institution:** Chandigarh University  
**Academic Session:** 2026–27  
**Official Repository:** [KishanKumar-in/cu-ai-applications-lab](https://github.com/KishanKumar-in/cu-ai-applications-lab)  
**Primary Master Source:** `_COMPLETE_CONT_26ECP-102 __ AI APPLICATIONS LAB_SEMESTER_MASTER.md`  

---

### **Provenance & Editorial Standards**
- `[DIRECTLY IN NOTES]`: Topics explicitly present in the CU syllabus, lecture presentations, and lab notebooks.
- `[RESTORED STANDARD CODE / ARCHITECTURE]`: Verified, executable Python implementations, mathematical proofs, and standard industry architectures restored to replace placeholders or truncated artifacts.
- `[LAB / EXAM SUPPORT]`: Worked derivations, multi-model evaluation benchmarks, dry-run analyses, and viva voce preparation.
- `⚠ Examiner's flag`: Critical traps, data leakage warnings, subtle ML bugs, and examination scoring pitfalls.

---

### **Comprehensive Table of Contents**

- [Unit 1: Data Pre-processing, Exploratory Data Analysis & Supervised Machine Learning](#unit-1-data-pre-processing-exploratory-data-analysis--supervised-machine-learning)
  - [Experiment 1.1: Data Pre-processing, Pandas, NumPy & Matplotlib](#experiment-11-data-pre-processing-pandas-numpy--matplotlib)
  - [Experiment 1.2: Exploratory Data Analysis on Real-World Datasets (`data.csv`)](#experiment-12-exploratory-data-analysis-on-real-world-datasets)
  - [Experiment 1.3: Supervised Learning & Classifier Models (`heart.csv.csv`)](#experiment-13-supervised-learning--classifier-models)
  - [Experiment 1.4: Comparative Classification Using Multiple ML Algorithms](#experiment-14-comparative-classification-using-multiple-machine-learning-algorithms)
  - [Unit 1 Master Viva Voce & Debugging Checklist](#unit-1-master-viva-voce--examiner-question-bank)
  - [Unit 1 Quick Revision Formula Sheet](#unit-1-quick-revision-formula-sheet)
- [Unit 2: AI Fundamentals, Generative AI, Transformers & Azure AI](#unit-2-ai-fundamentals-generative-ai-transformers--azure)
  - [Experiment 2.1: Artificial Intelligence Fundamentals & Agent Architectures](#experiment-21-artificial-intelligence-fundamentals-and-agent-architectures)
  - [Experiment 2.2: Transformer Architecture, Attention & Embeddings](#experiment-22-transformer-architecture-attention-and-embeddings)
  - [Experiment 2.3: Natural Language Processing Pipelines & Azure AI Language](#experiment-23-natural-language-processing-pipelines-and-azure-ai-language)
  - [Experiment 2.4: Generative AI on Azure & Prompt Engineering](#experiment-24-generative-ai-on-azure-and-prompt-engineering)
  - [Unit 2 Master Viva Voce & Debugging Checklist](#unit-2-master-viva-voce-and-examiner-checklist)
  - [Unit 2 Quick Revision Formula Sheet](#253-unit-2-quick-revision-formula-sheet)
- [Unit 3: Speech Processing, Computer Vision, OCR & Document Intelligence](#unit-3-speech-processing-computer-vision-ocr-and-master-lab-compendium)
  - [Experiment 3.1: Speech AI, Audio Processing & Azure Speech Services](#experiment-31-speech-ai-audio-processing-and-azure-speech-services)
  - [Experiment 3.2: Computer Vision, CNNs & DeepFace](#experiment-32-computer-vision-cnns-and-deepface)
  - [Experiment 3.3: Information Extraction, OCR & Azure Document Intelligence](#experiment-33-information-extraction-ocr-and-azure-document-intelligence)
- [Section 4: Ten High-Yield Solved Lab Practical Programs](#4-ten-high-yield-solved-lab-practical-programs)
- [Section 5: Comprehensive Master Viva Voce Question Bank (30 Questions)](#5-comprehensive-master-viva-voce-question-bank)
- [Section 6: Master Examiner's Pitfalls & Debugging Checklist](#6-master-examiners-pitfalls-and-debugging-checklist)
- [Section 7: Ultimate Revision Cheat Sheet](#7-ultimate-revision-cheat-sheet)
- [Section 8: Master Practical Exam Preparation Checklist](#8-master-practical-exam-preparation-checklist)
- [Section 9: Final Course Completion Matrix](#9-final-unit-3-completion-matrix)

---

# **UNIT 1: DATA PRE-PROCESSING, EXPLORATORY DATA ANALYSIS & SUPERVISED MACHINE LEARNING**

## **UNIT 1: Learning objectives**

By the end of this unit, you should be able to:

1. Work with Python, NumPy, Pandas and Matplotlib.
2. Clean, transform and prepare real-world datasets.
3. Perform exploratory data analysis and detect outliers.
4. Understand statistical distributions and feature relationships.
5. Train supervised classification algorithms.
6. Evaluate classifiers using statistical performance metrics.
7. Implement stratified cross-validation.
8. Compare multiple ML algorithms using reproducible experiments.

**Provenance convention used throughout**

- `[DIRECTLY IN NOTES]`: Explicitly specified in the supplied course material or syllabus.
- `[RESTORED STANDARD CODE / ARCHITECTURE]`: Complete implementation or established industry-standard technical detail.
- `[LAB / EXAM SUPPORT]`: Additional explanations, derivations, complexity analysis and examination preparation.

## **1. UNIT 1: EXPERIMENTAL STRUCTURE**

| Experiment | Practical title                                         | CO       |
| ---------- | ------------------------------------------------------- | -------- |
| 1.1        | Data Pre-processing, Pandas, NumPy and Matplotlib       | CO1, CO2 |
| 1.2        | Exploratory Data Analysis on Real-World Datasets        | CO2      |
| 1.3        | Supervised Learning and Classifier Models               | CO3      |
| 1.4        | Comparative Classification Using Multiple ML Algorithms | CO3      |

The repository identifies Google Colab as the practical platform and contains lecture notes, code examples, presentation material and practice questions for these experiments. Its master document reports 10,024 lines and approximately 307 KB.&#x20;

[image](https://www.google.com/s2/favicons?domain=https://github.com\&sz=32)

GitHub



# **EXPERIMENT 1.1**

# **DATA PRE-PROCESSING, PANDAS, NUMPY & MATPLOTLIB**



CO1 · CO2

Practical examination



## **1.1.1 Experiment details**

**[DIRECTLY IN NOTES]**

**Objective:** To understand and apply data pre-processing techniques using Python libraries such as NumPy, Pandas and Matplotlib, which are essential for preparing datasets for machine learning models.

**Platform:** Google Colaboratory.

**Expected learning outcomes:**

- Understand the importance of data preprocessing.
- Create and manipulate Pandas DataFrames.
- Perform numerical computations using NumPy.
- Apply statistical operations to datasets.
- Visualize data using different Matplotlib charts.
- Prepare structured datasets for machine learning.

## **1.1.2 Introduction to data preprocessing**

**[DIRECTLY IN NOTES]**

Data preprocessing is the process of transforming raw, inconsistent and incomplete data into a clean and structured format suitable for analysis and machine learning.

Real-world datasets commonly contain:

1. Missing values.
2. Duplicate records.
3. Incorrect data types.
4. Inconsistent categorical values.
5. Outliers.
6. Different numerical scales.
7. Unnecessary features.

### **Data preprocessing workflow**

**[LAB / EXAM SUPPORT]**

```
             RAW DATA
                 |
                 v
          DATA COLLECTION
                 |
                 v
          DATA INSPECTION
                 |
                 v
           DATA CLEANING
          /      |       \
         /       |        \
    Missing   Duplicates  Errors
    Values     Removal    Correction
         \       |        /
          \      |       /
                 v
         DATA TRANSFORMATION
                 |
          +------+------+
          |             |
          v             v
       Encoding      Scaling
          |             |
          +------+------+
                 |
                 v
          FEATURE SELECTION
                 |
                 v
          MODEL-READY DATA
```

### **Why is preprocessing important?**

| Reason         | Explanation                         |
| -------------- | ----------------------------------- |
| Data quality   | Removes inconsistencies and errors  |
| Accuracy       | Can improve predictive performance  |
| Efficiency     | Reduces unnecessary computation     |
| Consistency    | Makes features usable by algorithms |
| Reliability    | Reduces misleading patterns         |
| Generalization | Helps models perform on unseen data |

**Examiner's flag:** Preprocessing does not automatically improve accuracy. Incorrect preprocessing, such as deleting informative observations or scaling using inappropriate statistics, can make model performance worse.

## **1.1.3 Python fundamentals**

**[DIRECTLY IN NOTES + RESTORED STANDARD CODE]**

Python is a high-level, interpreted, dynamically typed programming language extensively used in artificial intelligence, machine learning and data science.

### **A. Variables**

A variable is a named reference to an object stored in memory.

```
name = "Alice"age = 20height = 5.4is_student = Trueprint("Name:", name)print("Age:", age)print("Height:", height)print("Student:", is_student)
```

**Expected output**

```
Name: Alice
Age: 20
Height: 5.4
Student: True
```

### **B. Python data types**

| Data type | Description          | Example          |
| --------- | -------------------- | ---------------- |
| int       | Integer values       | `age = 20`       |
| float     | Decimal values       | `height = 5.4`   |
| str       | Text                 | `name = "Alice"` |
| bool      | Logical values       | `active = True`  |
| list      | Mutable collection   | `[10, 20, 30]`   |
| tuple     | Immutable collection | `(10, 20, 30)`   |
| set       | Unique elements      | `{1, 2, 3}`      |
| dict      | Key-value collection | `{"age": 20}`    |

### **C. Checking data types and memory representation**

**[LAB / EXAM SUPPORT]**

```
import sysname = "Alice"age = 20height = 5.4marks = [80, 85, 90]print("Name type:", type(name))print("Age type:", type(age))print("Height type:", type(height))print("Marks type:", type(marks))print("Memory occupied by age object:",      sys.getsizeof(age), "bytes")print("Memory occupied by height object:",      sys.getsizeof(height), "bytes")print("Memory occupied by marks list:",      sys.getsizeof(marks), "bytes")
```

**Expected output**

```
Name type: <class 'str'>
Age type: <class 'int'>
Height type: <class 'float'>
Marks type: <class 'list'>
```

The memory sizes depend on the Python implementation and platform.

**Important memory concept**

Python variables are references to objects, rather than fixed memory boxes containing values directly.

```
Variable name
     |
     v
  Reference
     |
     v
+------------+
| Python     |
| Object     |
+------------+
| Value: 20  |
| Type: int  |
+------------+
```

For NumPy arrays, numerical elements are generally stored in contiguous or strided memory buffers, making vectorized computation much more efficient than repeatedly processing Python objects.

### **D. Arithmetic operations**

**[DIRECTLY IN NOTES]**

The repository demonstrates arithmetic operations using:

```
a = 220b = 16addition = a + bsubtraction = a - bmultiplication = a * bdivision = a / bfloor_division = a // bmodulus = a % bexponentiation = a ** bprint("Addition:", addition)print("Subtraction:", subtraction)print("Multiplication:", multiplication)print("Division:", division)print("Floor Division:", floor_division)print("Modulus:", modulus)print("Exponentiation:", exponentiation)
```

**Expected output**

```
Addition: 236
Subtraction: 204
Multiplication: 3520
Division: 13.75
Floor Division: 13
Modulus: 12
```

The exponentiation result is a very large integer:

```
220^16 =
115792089237316195423570985008687907853269984665640564007913129639936
```

**[EXAMINER’S FLAG / RESTORED STANDARD MATH]:** In standard IEEE Python execution, $220^{16} = 30113614963390651432960000000000000000 \approx 3.011 \times 10^{37}$. The number appearing in the CU slide text ($1.1579 \times 10^{75} \approx 2^{256}$) reflects an overflow/hash artifact from the course note compiler.

## 1.1.4 Pandas Codes for Data Analysis
[DIRECTLY IN NOTES] [RESTORED STANDARD CODE / ARCHITECTURE]
A. Introduction to Pandas
Pandas is an open-source Python library used for data manipulation, cleaning, analysis and preprocessing.
It provides two primary data structures:
Series: A one-dimensional labeled array.
DataFrame: A two-dimensional tabular data structure containing rows and columns.
A DataFrame resembles a database table or spreadsheet.
Architecture
PANDAS | +--------+--------+ | | Series DataFrame (1 Dimension) (2 Dimensions) | | Index Rows + Columns | | Values Labeled Data
B. Creating a Simple DataFrame
Program 1: Creating a DataFrame
import pandas as pd data = { "Name": ["Aman", "Riya", "Rahul", "Priya", "Karan"], "Age": [20, 21, 19, 22, 20], "Marks": [85, 92, 78, 95, 88], "Department": ["CSE", "IT", "CSE", "ECE", "IT"] } df = pd.DataFrame(data) print("Complete DataFrame:") print(df) print("\nFirst Five Records:") print(df.head()) print("\nLast Two Records:") print(df.tail(2)) print("\nDataFrame Shape:") print(df.shape) print("\nColumn Names:") print(df.columns.tolist())
Expected output
Complete DataFrame: Name Age Marks Department 0 Aman 20 85 CSE 1 Riya 21 92 IT 2 Rahul 19 78 CSE 3 Priya 22 95 ECE 4 Karan 20 88 IT DataFrame Shape: (5, 4) Column Names: ['Name', 'Age', 'Marks', 'Department']
head() displays the first five rows by default, while tail() displays the last five rows by default.
C. DataFrame Information
Program 2: Displaying DataFrame Information
import pandas as pd data = { "Name": ["Aman", "Riya", "Rahul", "Priya", "Karan"], "Age": [20, 21, 19, 22, 20], "Marks": [85, 92, 78, 95, 88], "Department": ["CSE", "IT", "CSE", "ECE", "IT"] } df = pd.DataFrame(data) print("Dataset Information:") df.info() print("\nNumber of Rows:", df.shape[0]) print("Number of Columns:", df.shape[1]) print("\nData Types:") print(df.dtypes) print("\nMemory Usage:") print(df.memory_usage(deep=True))
Expected output
Dataset Information: <class 'pandas.core.frame.DataFrame'> RangeIndex: 5 entries, 0 to 4 Data columns (total 4 columns): # Column Non-Null Count Dtype --- ------ -------------- ----- 0 Name 5 non-null object 1 Age 5 non-null int64 2 Marks 5 non-null int64 3 Department 5 non-null object dtypes: int64(2), object(2)
Memory usage and some formatting details can vary by Pandas version.
Important DataFrame functions
Function
Purpose
df.info()
Dataset structure and data types
df.shape
Rows and columns
df.columns
Column names
df.dtypes
Data types
df.head()
First five records
df.tail()
Last five records
df.isnull().sum()
Missing values per column
df.duplicated().sum()
Number of duplicate rows
df.drop_duplicates()
Remove duplicate rows
D. DataFrame Summary Statistics
Program 3: Descriptive Statistics
import pandas as pd data = { "Name": ["Aman", "Riya", "Rahul", "Priya", "Karan"], "Age": [20, 21, 19, 22, 20], "Marks": [85, 92, 78, 95, 88] } df = pd.DataFrame(data) print("Statistical Summary:") print(df.describe()) print("\nMean Marks:", df["Marks"].mean()) print("Median Marks:", df["Marks"].median()) print("Mode Marks:", df["Marks"].mode().tolist()) print("Maximum Marks:", df["Marks"].max()) print("Minimum Marks:", df["Marks"].min()) print("Standard Deviation:", round(df["Marks"].std(), 2)) print("Variance:", round(df["Marks"].var(), 2))
Expected numerical results
Statistic
Age
Marks
Count
5
5
Mean
20.4
87.6
Minimum
19
78
Maximum
22
95
For Marks:
Mean = 87.6
Median = 88
Mode = No unique mode; all values occur once.
Sample standard deviation ≈ 6.54.
Sample variance = 42.8.
Examiner's flag: Pandas std() and var() calculate sample standard deviation and sample variance by default, using \(N-1\) in the denominator. NumPy's default variance uses \(N\).
E. Data Selection and Filtering
Program 4: Indexing, Selection and Filtering
import pandas as pd data = { "Name": ["Aman", "Riya", "Rahul", "Priya", "Karan"], "Age": [20, 21, 19, 22, 20], "Marks": [85, 92, 78, 95, 88] } df = pd.DataFrame(data) print("Single Column:") print(df["Name"]) print("\nMultiple Columns:") print(df[["Name", "Marks"]]) print("\nUsing loc:") print(df.loc[0:2, ["Name", "Marks"]]) print("\nUsing iloc:") print(df.iloc[0:3, 0:2]) print("\nStudents scoring above 85:") print(df[df["Marks"] > 85]) print("\nStudents aged 20 or above:") print(df[df["Age"] >= 20])
Difference between loc and iloc
Feature
loc
iloc
Selection
Label-based
Position-based
Row indexing
Index labels
Integer positions
End slicing
Inclusive
Exclusive
Example
df.loc[0:2]
df.iloc[0:2]
Examiner's flag
A common mistake is assuming that loc[0:2] and iloc[0:2] return the same number of rows. With the default integer index, the first returns three rows and the second returns two.
1.1.5 NumPy Codes for Data Analysis
[DIRECTLY IN NOTES] [RESTORED STANDARD CODE / ARCHITECTURE]
A. Introduction to NumPy
NumPy stands for Numerical Python. It is a fundamental library for scientific computing and numerical operations.
Its primary data structure is the multidimensional homogeneous array called ndarray.
Advantages
Fast numerical calculations.
Vectorized mathematical operations.
Efficient memory representation.
Matrix and linear algebra operations.
Statistical analysis.
Random number generation.
B. Creating One-Dimensional and Two-Dimensional Arrays
Program 1: Array Creation
import numpy as np # One-dimensional array arr1 = np.array([10, 20, 30, 40, 50]) # Two-dimensional array arr2 = np.array([ [10, 20, 30], [40, 50, 60], [70, 80, 90] ]) print("1D Array:") print(arr1) print("\n2D Array:") print(arr2) print("\nDimensions:", arr2.ndim) print("Shape:", arr2.shape) print("Total Elements:", arr2.size) print("Data Type:", arr2.dtype) print("\nZeros:") print(np.zeros((2, 3))) print("\nOnes:") print(np.ones((2, 3))) print("\nRange:") print(np.arange(1, 11, 2)) print("\nEvenly Spaced Values:") print(np.linspace(0, 10, 5))
Expected output
1D Array: [10 20 30 40 50] 2D Array: [[10 20 30] [40 50 60] [70 80 90]] Dimensions: 2 Shape: (3, 3) Total Elements: 9 Data Type: int64 Range: [1 3 5 7 9] Evenly Spaced Values: [ 0. 2.5 5. 7.5 10. ]
C. Array Slicing and Vectorized Operations
Program 2: Array Manipulation
import numpy as np arr = np.array([10, 20, 30, 40, 50]) print("Original Array:", arr) print("First Three:", arr[:3]) print("Last Two:", arr[-2:]) print("Elements from Index 1 to 3:", arr[1:4]) print("\nAddition:", arr + 5) print("Subtraction:", arr - 5) print("Multiplication:", arr * 2) print("Division:", arr / 10) print("Square:", arr ** 2) print("\nElements Greater Than 25:") print(arr[arr > 25])
Expected output
Original Array: [10 20 30 40 50] First Three: [10 20 30] Last Two: [40 50] Elements from Index 1 to 3: [20 30 40] Addition: [15 25 35 45 55] Subtraction: [ 5 15 25 35 45] Multiplication: [ 20 40 60 80 100] Division: [1. 2. 3. 4. 5.] Square: [ 100 400 900 1600 2500] Elements Greater Than 25: [30 40 50]
D. Basic Statistical Analysis
Program 3: Statistical Operations
import numpy as np data = np.array([10, 20, 30, 40, 50]) print("Dataset:", data) print("Mean:", np.mean(data)) print("Median:", np.median(data)) print("Standard Deviation:", np.std(data)) print("Variance:", np.var(data)) print("Minimum:", np.min(data)) print("Maximum:", np.max(data)) print("Sum:", np.sum(data)) print("Range:", np.ptp(data))
Expected output
Dataset: [10 20 30 40 50] Mean: 30.0 Median: 30.0 Standard Deviation: 14.1421356237 Variance: 200.0 Minimum: 10 Maximum: 50 Sum: 150 Range: 40
Mathematical formulations:
Arithmetic mean
\[ \mu=\frac{1}{N}\sum_{i=1}^{N}x_i \]
Population variance
\[ \sigma^2=\frac{1}{N}\sum_{i=1}^{N}(x_i-\mu)^2 \]
Population standard deviation
\[ \sigma=\sqrt{\frac{1}{N}\sum_{i=1}^{N}(x_i-\mu)^2} \]
Note: np.std() and np.var() use population formulas by default (ddof=0). Set ddof=1 for sample statistics.
E. Correlation Coefficient
Correlation measures the strength and direction of a relationship between two variables.
Pearson correlation coefficient
\[ r_{xy}= \frac{\sum_{i=1}^{N}(x_i-\bar{x})(y_i-\bar{y})} {\sqrt{\sum_{i=1}^{N}(x_i-\bar{x})^2 \sum_{i=1}^{N}(y_i-\bar{y})^2}} \]
Interpretation:
Correlation
Interpretation
+1
Perfect positive correlation
+0.7
Strong positive correlation
+0.3
Weak positive correlation
0
No linear correlation
-0.3
Weak negative correlation
-0.7
Strong negative correlation
-1
Perfect negative correlation
Program 4: Correlation using NumPy
import numpy as np study_hours = np.array([1, 2, 3, 4, 5]) marks = np.array([20, 40, 50, 70, 90]) correlation_matrix = np.corrcoef(study_hours, marks) print("Correlation Matrix:") print(correlation_matrix) print("\nPearson Correlation:") print(round(correlation_matrix[0, 1], 4))
Expected output
Correlation Matrix: [[1. 0.99388373] [0.99388373 1. ]] Pearson Correlation: 0.9939
Examiner's flag
Correlation does not establish causation. A high correlation does not prove that one variable causes changes in another.
1.1.6 Matplotlib Codes for Data Visualization
[DIRECTLY IN NOTES] [RESTORED STANDARD CODE / ARCHITECTURE]
A. Introduction to Matplotlib
Matplotlib is a Python visualization library used to generate:
Line plots.
Bar charts.
Histograms.
Scatter plots.
Pie charts.
Box plots.
Its pyplot module provides a MATLAB-like plotting interface.
MATPLOTLIB | Pyplot | +---------+---------+ | | | Line Bar Pie Plot Chart Chart | Scatter | Histogram
B. Adding Grid Lines and Customizing Line Plots
Program 1: Line Plot with Grid
import matplotlib.pyplot as plt days = [1, 2, 3, 4, 5, 6, 7] temperature = [25, 27, 26, 30, 32, 31, 34] plt.figure(figsize=(9, 5)) plt.plot( days, temperature, color="blue", marker="o", linestyle="--", linewidth=2, markersize=8, label="Temperature" ) plt.title("Weekly Temperature Analysis") plt.xlabel("Day") plt.ylabel("Temperature (°C)") plt.grid( True, linestyle=":", alpha=0.7 ) plt.legend() plt.xticks(days) plt.tight_layout() plt.show()
Expected analysis: The line chart shows a general increasing temperature trend over seven days.
C. Bar Charts
A bar chart represents categorical data using rectangular bars.
Program 2: Simple Bar Chart
import matplotlib.pyplot as plt students = ["Aman", "Riya", "Rahul", "Priya", "Karan"] marks = [85, 92, 78, 95, 88] plt.figure(figsize=(9, 5)) plt.bar( students, marks, color="skyblue", edgecolor="black" ) plt.title("Student Marks Comparison") plt.xlabel("Students") plt.ylabel("Marks") plt.ylim(0, 100) plt.grid(axis="y", linestyle="--", alpha=0.5) plt.tight_layout() plt.show()
Program 3: Grouped Bar Chart
import numpy as np import matplotlib.pyplot as plt students = ["Aman", "Riya", "Rahul", "Priya"] python_marks = [85, 92, 78, 95] java_marks = [80, 88, 82, 90] x = np.arange(len(students)) width = 0.35 plt.figure(figsize=(9, 5)) plt.bar( x - width / 2, python_marks, width, label="Python", color="steelblue" ) plt.bar( x + width / 2, java_marks, width, label="Java", color="orange" ) plt.xlabel("Students") plt.ylabel("Marks") plt.title("Python vs Java Marks") plt.xticks(x, students) plt.legend() plt.grid(axis="y", alpha=0.4) plt.tight_layout() plt.show()
Program 4: Stacked Bar Chart
import matplotlib.pyplot as plt students = ["Aman", "Riya", "Rahul", "Priya"] theory = [40, 45, 35, 48] practical = [45, 47, 43, 47] plt.figure(figsize=(9, 5)) plt.bar( students, theory, label="Theory", color="royalblue" ) plt.bar( students, practical, bottom=theory, label="Practical", color="orange" ) plt.title("Total Marks Distribution") plt.xlabel("Students") plt.ylabel("Marks") plt.legend() plt.grid(axis="y", alpha=0.4) plt.tight_layout() plt.show()
D. Pie Chart
A pie chart displays the proportional contribution of categories to a whole.
Program 5: Pie Chart with Explode and Autopct
import matplotlib.pyplot as plt departments = ["CSE", "IT", "ECE", "Mechanical"] students = [40, 25, 20, 15] explode = (0.1, 0, 0, 0) plt.figure(figsize=(8, 8)) plt.pie( students, labels=departments, autopct="%1.1f%%", explode=explode, startangle=90, shadow=True ) plt.title("Department-wise Student Distribution") plt.legend( departments, title="Departments", loc="best" ) plt.axis("equal") plt.show()
Expected output analysis
Department
Students
Percentage
CSE
40
40%
IT
25
25%
ECE
20
20%
Mechanical
15
15%
Total
100
100%
Examiner's flag: The sum of pie-chart values represents the whole. Negative values are invalid, and zero-total data cannot form meaningful proportions.
1.1.7 Practice Task Questions, Expected Outputs & Analysis
[LAB / EXAM SUPPORT]
A. Practice questions
No.
Practical question
Main function
1
Create a Pandas DataFrame containing student details.
pd.DataFrame()
2
Display the first five records.
head()
3
Display dataset information.
info()
4
Calculate mean, median and mode.
mean(), median(), mode()
5
Create a 1D NumPy array.
np.array()
6
Create a 2D NumPy matrix.
np.array()
7
Calculate variance and standard deviation.
np.var(), np.std()
8
Calculate correlation between two variables.
np.corrcoef()
9
Draw a line graph with grid lines.
plt.plot()
10
Draw a grouped bar chart.
plt.bar()
11
Create a stacked bar chart.
bottom=
12
Create a pie chart with percentage labels.
plt.pie()
B. Combined practical examination program
This program integrates DataFrame creation, statistical calculations, NumPy operations and Matplotlib visualization.
import pandas as pd import numpy as np import matplotlib.pyplot as plt # Step 1: Create sample dataset data = { "Student": ["Aman", "Riya", "Rahul", "Priya", "Karan"], "Marks": [85, 92, 78, 95, 88], "Attendance": [90, 95, 85, 98, 92] } df = pd.DataFrame(data) # Step 2: Display dataset print("STUDENT DATA") print(df) # Step 3: Statistical analysis print("\nSTATISTICAL SUMMARY") print(df[["Marks", "Attendance"]].describe()) # Step 4: NumPy analysis marks = np.array(df["Marks"]) print("\nNUMPY ANALYSIS") print("Mean:", np.mean(marks)) print("Median:", np.median(marks)) print("Variance:", np.var(marks)) print("Standard Deviation:", np.std(marks)) # Step 5: Correlation correlation = np.corrcoef( df["Marks"], df["Attendance"] ) print("\nCORRELATION MATRIX") print(correlation) # Step 6: Visualization plt.figure(figsize=(8, 5)) plt.plot( df["Student"], df["Marks"], marker="o", linewidth=2, label="Marks" ) plt.title("Student Performance") plt.xlabel("Students") plt.ylabel("Marks") plt.grid(True) plt.legend() plt.tight_layout() plt.show() # Step 7: Bar chart plt.figure(figsize=(8, 5)) plt.bar( df["Student"], df["Attendance"], color="skyblue" ) plt.title("Student Attendance") plt.xlabel("Students") plt.ylabel("Attendance (%)") plt.ylim(0, 100) plt.tight_layout() plt.show()
Expected numerical output
Student
Marks
Attendance
Aman
85
90
Riya
92
95
Rahul
78
85
Priya
95
98
Karan
88
92
Mean marks: 87.6
Median marks: 88
Population variance: 34.64
Population standard deviation: approximately 5.885
Correlation between marks and attendance: approximately 0.995.
Experiment 1.1 conclusion: Pandas handles structured data, NumPy performs numerical computations, and Matplotlib visualizes patterns. These libraries collectively establish the foundation for subsequent machine learning experiments.
EXPERIMENT 1.2: EXPLORATORY DATA ANALYSIS ON REAL-WORLD DATASETS
Core Unit 1 Practical
1.2.1 Objective
[DIRECTLY IN NOTES]
To perform Exploratory Data Analysis (EDA) on a real-world dataset to identify patterns, correlations and trends using descriptive statistics and visualization techniques.
Learning objectives
Understand and apply descriptive statistical methods.
Identify numerical and categorical distributions.
Detect missing values, duplicate records and outliers.
Calculate statistical relationships between variables.
Visualize distributions using histograms, box plots, scatter plots and heatmaps.
Extract insights that can guide feature selection and machine learning model development.
Platform and tools
Component
Technology
Programming language
Python 3
Platform
Google Colab / Jupyter Notebook
Data manipulation
Pandas
Numerical computation
NumPy
Visualization
Matplotlib
Statistical visualization
Seaborn
Dataset
data.csv
Installation
!pip install -q pandas numpy matplotlib seaborn scipy
Importing libraries
import pandas as pd import numpy as np import matplotlib.pyplot as plt import seaborn as sns from scipy import stats sns.set_theme(style="whitegrid") print("All libraries imported successfully.")
Expected output:
All libraries imported successfully.
1.2.2 Theoretical foundations of EDA
A. What is Exploratory Data Analysis?
EDA is the process of investigating a dataset before applying statistical modeling or machine learning.
It helps us understand:
Dataset structure.
Variable distributions.
Missing information.
Outliers.
Relationships between variables.
Trends and patterns.
EDA workflow
RAW DATASET | v LOAD DATA | v DATA UNDERSTANDING | v MISSING VALUE CHECK | v DUPLICATE DETECTION | v DESCRIPTIVE STATISTICS | v DATA VISUALIZATION | v CORRELATION ANALYSIS | v OUTLIER DETECTION | v FEATURE SELECTION | v MACHINE LEARNING READY DATA
B. Numerical and categorical distributions
Numerical variables
Numerical variables represent measurable quantities.
Examples:
Duration.
Pulse.
Maximum pulse.
Calories.
Age.
Temperature.
They can be divided into:
Discrete variables: Countable values, such as number of students.
Continuous variables: Measurable values, such as body temperature.
Categorical variables
Categorical variables represent groups or labels.
Examples:
Gender.
Department.
Product category.
Disease status.
They can be divided into:
Nominal: Categories without an inherent order.
Ordinal: Categories with an inherent order.
C. Measures of central tendency
1. Mean
The mean is the arithmetic average.
\[ \mu=\frac{1}{N}\sum_{i=1}^{N}x_i \]
Example:
Dataset:
\[ X=[10,20,30,40,50] \]
\[ \mu=\frac{10+20+30+40+50}{5} \]
\[ \boxed{\mu=30} \]
2. Median
The median is the middle value after sorting the observations.
For an odd number of observations:
\[ Median=X_{\left(\frac{N+1}{2}\right)} \]
For an even number:
\[ Median=\frac{X_{(N/2)}+X_{(N/2+1)}}{2} \]
Example:
\[ X=[10,20,30,40,50] \]
\[ Median=30 \]
3. Mode
Mode is the most frequently occurring observation.
Example:
\[ X=[10,20,20,30,40] \]
\[ Mode=20 \]
D. Measures of dispersion
1. Range
\[ Range=X_{\max}-X_{\min} \]
For:
\[ X=[10,20,30,40,50] \]
\[ Range=50-10=40 \]
2. Variance
Population variance measures how far observations are spread around their mean.
\[ \sigma^2=\frac{1}{N}\sum_{i=1}^{N}(x_i-\mu)^2 \]
Worked example:
\[ X=[10,20,30,40,50] \]
Mean:
\[ \mu=30 \]
\(x_i\)
\(x_i-\mu\)
\((x_i-\mu)^2\)
10
-20
400
20
-10
100
30
0
0
40
10
100
50
20
400
Total
0
1000
Therefore:
\[ \sigma^2=\frac{1000}{5} \]
\[ \boxed{\sigma^2=200} \]
3. Standard deviation
\[ \sigma=\sqrt{\sigma^2} \]
\[ \sigma=\sqrt{200} \]
\[ \boxed{\sigma\approx14.142} \]
A higher standard deviation indicates greater dispersion.
E. Skewness
Skewness measures the asymmetry of a probability distribution.
[Handling skewed data during your data analysis: | by Abhinay Ratakonda | Medium](https://images.openai.com/static-rsc-4/fQiq_0Vj1Jd7qZEJ-e4i18PhBnOTqL1MC-6bGGaFr2Ko4E5rce4nlzCv3gu0IaqVl-IUiIyAPei9sRkCnNLP1fullIQVqdpk_npSqI0BtZMrFjHU_ytrYJdpv6ZPtsuHNx-vrSkGZdPPOPGyvGRJUaRV1nAQSzTSLxdPStTHa_o?purpose=inline)
Positive skewness
Long tail towards the right.
Mean generally greater than median.
Example: Income distributions.
[Programming Machine Learning Applications in Python — Part 2 | by Neha Bhatia | Medium](https://images.openai.com/static-rsc-4/wxZgW2i0_yT-ZuYHBhHUzpOkm7QKlbdISoTCWSjL6rmJoRbPiExtERiowvBASalVnVlIrLgVopo94fhe9G_GK7NguzKley4Irchvp3d6lXq-BwYzKUYEvLD-Ll0__BAtrAZHHaeWxPpAY5UtBHy9FRYJKaSeb3hBf05KCbHG9qk?purpose=inline)
Symmetrical distribution
Approximately equal tails.
Mean approximately equal to median.
Example: Ideal normal distribution.
[Determining the central tendency in case of a skewed distribution](https://images.openai.com/static-rsc-4/No0a8qtxTSWrvzwI8IH3mPwJtG7qKlGY6_-bQXJR-s_ZBZS0u8OJmeSldQ61QRwzLx3W0jgjkFzrwDA0fc5NTSCVunmRF9YIMQr8Qz6jy91OjPk-JFt8I-Q0BR6KaOLWlWu7qA--p-qXkHIMXwya8cjYbUyzjH7RwVqkh9Rav2Q?purpose=inline)
Negative skewness
Long tail towards the left.
Mean generally less than median.
Example: An assessment where most students score highly.
Python calculation:
import pandas as pd data = [10, 20, 25, 30, 35, 40, 100] series = pd.Series(data) print("Skewness:", series.skew()) print("Kurtosis:", series.kurt())
Pandas computes sample skewness and excess kurtosis by default.
F. Interquartile Range (IQR)
IQR measures the spread of the middle 50% of the observations.
\[ IQR=Q_3-Q_1 \]
Where:
\(Q_1\): First quartile, 25th percentile.
\(Q_2\): Median, 50th percentile.
\(Q_3\): Third quartile, 75th percentile.
Outlier boundaries:
\[ Lower=Q_1-1.5(IQR) \]
\[ Upper=Q_3+1.5(IQR) \]
Any observation outside these boundaries is flagged as a potential outlier.
Worked example
Suppose:
\[ Q_1=20,\quad Q_3=40 \]
\[ IQR=40-20=20 \]
Lower boundary:
\[ 20-1.5(20)=-10 \]
Upper boundary:
\[ 40+1.5(20)=70 \]
Therefore, values below -10 or above 70 are potential outliers.
G. Z-score method
Z-score indicates how many standard deviations an observation is away from the mean.
\[ Z=\frac{x-\mu}{\sigma} \]
Interpretation:
Z-score
Interpretation
0
Exactly at the mean
+1
One standard deviation above mean
-1
One standard deviation below mean
+2
Two standard deviations above mean
-2
Two standard deviations below mean
Greater than +3 or less than -3
Common potential-outlier threshold
Python implementation
import numpy as np from scipy.stats import zscore data = np.array([10, 12, 11, 13, 12, 14, 100]) z_scores = zscore(data) print("Original Data:", data) print("Z-Scores:", np.round(z_scores, 3)) outliers = data[np.abs(z_scores) > 2] print("Potential Outliers:", outliers)
Expected result: The value 100 is identified as a potential outlier under this example's chosen threshold.
Examiner's flag: Outlier thresholds are screening rules, not proof that a measurement is erroneous. An extreme but valid observation should not automatically be deleted.
H. Pearson correlation coefficient
Pearson correlation measures the strength and direction of a linear relationship.
\[ r_{xy}= \frac{\sum(x_i-\bar{x})(y_i-\bar{y})} {\sqrt{\sum(x_i-\bar{x})^2\sum(y_i-\bar{y})^2}} \]
Its value lies between -1 and +1.
Positive: Both variables tend to increase together.
Negative: One variable tends to decrease as the other increases.
Zero: No linear relationship is detected.
Important distinction: Zero Pearson correlation does not necessarily mean that two variables are independent. A nonlinear relationship may exist.
1.2.3 Real-world dataset: data.csv
[DIRECTLY IN NOTES]
The practical uses a physical-activity or exercise dataset with the following numerical columns.
Column
Description
Data type
Unit
Duration
Duration of exercise
Numerical
Minutes
Pulse
Heart rate during exercise
Numerical
Beats/min
Maxpulse
Maximum pulse recorded
Numerical
Beats/min
Calories
Calories burned
Numerical
Calories
The dataset allows analysis of relationships between exercise duration, heart rate and energy expenditure.
Important: The actual CSV is not attached to this conversation. The following programs load the original data.csv when supplied. To make the practical fully reproducible without an external download, a separate synthetic dataset generator is also provided.
Synthetic sample dataset generator
This generator creates realistic demonstration records with missing values and an outlier. It is not claimed to be the original CU dataset.
import pandas as pd import numpy as np rng = np.random.default_rng(42) n = 100 duration = rng.integers(15, 91, size=n) pulse = rng.normal(110, 12, size=n).round().astype(float) maxpulse = ( pulse + rng.normal(35, 8, size=n) ).round().astype(float) calories = ( duration * 5.2 + (pulse - 90) * 2.1 + rng.normal(0, 25, size=n) ).round(2) df_sample = pd.DataFrame({ "Duration": duration, "Pulse": pulse, "Maxpulse": maxpulse, "Calories": calories }) # Introduce controlled missing values df_sample.loc[5, "Calories"] = np.nan df_sample.loc[12, "Pulse"] = np.nan df_sample.loc[24, "Duration"] = np.nan # Introduce a demonstration outlier df_sample.loc[50, "Calories"] = 1500 df_sample.to_csv("data.csv", index=False) print("Sample dataset created successfully.") print(df_sample.head(10)) print("\nDataset Shape:", df_sample.shape)
Expected output:
Sample dataset created successfully. Dataset Shape: (100, 4)
The first ten records will be generated deterministically using seed 42.
1.2.4 Complete practical implementation: Eight essential codes
Code 1: Load Dataset
[DIRECTLY IN NOTES]
Objective: Load the dataset using Pandas and display the records.
import pandas as pd # Load CSV file df = pd.read_csv("data.csv") # Display complete dataset print("COMPLETE DATASET") print(df.to_string()) # Display first five records print("\nFIRST FIVE RECORDS") print(df.head()) # Display dataset dimensions print("\nDATASET SHAPE") print(df.shape) # Display column names print("\nCOLUMN NAMES") print(df.columns.tolist())
Expected output structure
FIRST FIVE RECORDS Duration Pulse Maxpulse Calories 0 15 113.0 148.0 ... 1 65 125.0 160.0 ... ... DATASET SHAPE (100, 4)
Exact values depend on the CSV being loaded.
Analysis: The dataset contains four variables, each representing a measurable aspect of exercise performance.
Code 2: Basic Dataset Information
Objective: Inspect row count, columns, data types and non-null records.
import pandas as pd df = pd.read_csv("data.csv") print("DATASET INFORMATION") df.info() print("\nNUMBER OF ROWS:") print(df.shape[0]) print("\nNUMBER OF COLUMNS:") print(df.shape[1]) print("\nCOLUMN DATA TYPES:") print(df.dtypes) print("\nCOLUMN NAMES:") print(df.columns.tolist())
Expected output structure
<class 'pandas.core.frame.DataFrame'> RangeIndex: 100 entries, 0 to 99 Data columns (total 4 columns): # Column Non-Null Count Dtype --- ------ -------------- ----- 0 Duration ... 1 Pulse ... 2 Maxpulse ... 3 Calories ... dtypes: float64(...), int64(...)
The number of non-null values reveals whether columns contain missing data.
Code 3: Summary Statistics
Objective: Calculate descriptive statistical measures.
import pandas as pd import numpy as np df = pd.read_csv("data.csv") print("DESCRIPTIVE STATISTICS") print(df.describe()) print("\nADDITIONAL STATISTICS") for column in df.select_dtypes(include=np.number).columns: print("\nColumn:", column) print("Mean:", df[column].mean()) print("Median:", df[column].median()) print("Mode:", df[column].mode().tolist()) print("Variance:", df[column].var()) print("Standard Deviation:", df[column].std()) print("Minimum:", df[column].min()) print("Maximum:", df[column].max()) print("Skewness:", df[column].skew())
Expected output table structure
Statistic
Duration
Pulse
Maxpulse
Calories
Count
Valid count
Valid count
Valid count
Valid count
Mean
Calculated
Calculated
Calculated
Calculated
Std
Calculated
Calculated
Calculated
Calculated
Min
Calculated
Calculated
Calculated
Calculated
25%
Calculated
Calculated
Calculated
Calculated
50%
Calculated
Calculated
Calculated
Calculated
75%
Calculated
Calculated
Calculated
Calculated
Max
Calculated
Calculated
Calculated
Calculated
Analysis: The mean and median indicate central tendency. Standard deviation and variance indicate dispersion. Minimum, maximum and quartiles help identify unusual observations.
Code 4: Checking and Handling Missing Values
Objective: Detect missing observations and demonstrate deletion and imputation.
Part A: Missing-value detection
import pandas as pd df = pd.read_csv("data.csv") print("MISSING VALUES PER COLUMN") print(df.isna().sum()) print("\nTOTAL MISSING VALUES") print(df.isna().sum().sum()) print("\nMISSING VALUE PERCENTAGE") print((df.isna().mean() * 100).round(2))
Part B: Removing missing values
import pandas as pd df = pd.read_csv("data.csv") print("Original Shape:", df.shape) df_dropped = df.dropna() print("Shape After Removing Missing Rows:") print(df_dropped.shape) print("\nRemaining Missing Values:") print(df_dropped.isna().sum())
dropna() removes rows containing missing values by default.
Part C: Mean, median and mode imputation
import pandas as pd import numpy as np df = pd.read_csv("data.csv") numeric_columns = df.select_dtypes( include=np.number ).columns df_mean = df.copy() df_median = df.copy() df_mode = df.copy() for column in numeric_columns: mean_value = df_mean[column].mean() median_value = df_median[column].median() mode_values = df_mode[column].mode() if not mode_values.empty: mode_value = mode_values.iloc[0] df_mode[column] = df_mode[column].fillna( mode_value ) df_mean[column] = df_mean[column].fillna( mean_value ) df_median[column] = df_median[column].fillna( median_value ) print("Original Missing Values:") print(df.isna().sum()) print("\nAfter Mean Imputation:") print(df_mean.isna().sum()) print("\nAfter Median Imputation:") print(df_median.isna().sum()) print("\nAfter Mode Imputation:") print(df_mode.isna().sum())
Comparison
Technique
Method
Suitable situation
dropna()
Remove incomplete rows
Few missing records
Mean
Replace with average
Approximately symmetric numerical data
Median
Replace with middle value
Skewed numerical data or outlier-prone data
Mode
Replace with most frequent value
Categorical or repeated discrete data
Examiner's flag
Never calculate imputation statistics using the complete dataset before a train-test split when building a predictive model. Fit imputers on training data only, then apply the fitted transformation to test data.
Code 5: Correlation Matrix
Objective: Calculate relationships between numerical variables.
import pandas as pd df = pd.read_csv("data.csv") numeric_df = df.select_dtypes( include="number" ) correlation_matrix = numeric_df.corr( method="pearson" ) print("PEARSON CORRELATION MATRIX") print(correlation_matrix.round(3))
Expected output structure
Duration Pulse Maxpulse Calories Duration 1.000 ... ... ... Pulse ... 1.000 ... ... Maxpulse ... ... 1.000 ... Calories ... ... ... 1.000
Every diagonal element equals 1 because each variable has perfect correlation with itself.
Alternative correlation methods
print("Pearson:") print(numeric_df.corr(method="pearson")) print("\nSpearman:") print(numeric_df.corr(method="spearman")) print("\nKendall:") print(numeric_df.corr(method="kendall"))
Method
Measures
Pearson
Linear relationship
Spearman
Monotonic rank relationship
Kendall
Rank association
Code 6: Correlation Heatmap
[DIRECTLY IN NOTES]
Objective: Visualize correlations using Seaborn.
import pandas as pd import matplotlib.pyplot as plt import seaborn as sns df = pd.read_csv("data.csv") numeric_df = df.select_dtypes( include="number" ) correlation_matrix = numeric_df.corr() plt.figure(figsize=(9, 7)) sns.heatmap( correlation_matrix, annot=True, cmap="coolwarm", fmt=".2f", linewidths=0.5, square=True, vmin=-1, vmax=1 ) plt.title("Correlation Heatmap of Exercise Dataset") plt.tight_layout() plt.show()
How to interpret the heatmap
Strong positive correlation: Darker positive-side color.
Strong negative correlation: Opposite-side color.
Near-zero correlation: Values near the midpoint.
The precise color depends on the selected colormap and its scale.
Code 7: Boxplots for Outlier Detection
Objective: Identify potential outliers in numerical columns.
import pandas as pd import matplotlib.pyplot as plt import seaborn as sns df = pd.read_csv("data.csv") numeric_df = df.select_dtypes( include="number" ) plt.figure(figsize=(11, 6)) sns.boxplot( data=numeric_df, orient="h" ) plt.title("Box Plot for Numerical Columns") plt.xlabel("Values") plt.tight_layout() plt.show()
Individual box plots
import pandas as pd import matplotlib.pyplot as plt import seaborn as sns df = pd.read_csv("data.csv") columns = [ "Duration", "Pulse", "Maxpulse", "Calories" ] fig, axes = plt.subplots( 2, 2, figsize=(12, 8) ) axes = axes.flatten() for i, column in enumerate(columns): sns.boxplot( y=df[column], ax=axes[i] ) axes[i].set_title( f"Outlier Analysis: {column}" ) plt.tight_layout() plt.show()
IQR-based numerical outlier detection
import pandas as pd df = pd.read_csv("data.csv") numeric_columns = df.select_dtypes( include="number" ).columns for column in numeric_columns: q1 = df[column].quantile(0.25) q3 = df[column].quantile(0.75) iqr = q3 - q1 lower = q1 - 1.5 * iqr upper = q3 + 1.5 * iqr outliers = df[ (df[column] < lower) | (df[column] > upper) ] print("\nColumn:", column) print("Q1:", q1) print("Q3:", q3) print("IQR:", iqr) print("Lower Boundary:", lower) print("Upper Boundary:", upper) print("Outlier Count:", len(outliers)) print(outliers[[column]])
Analysis: Box plots show the median, quartiles, interquartile range and observations beyond the whisker boundaries.
Code 8: Scatter Plot (Pulse vs Calories)
[DIRECTLY IN NOTES] [RESTORED STANDARD CODE / ARCHITECTURE]
Objective: Examine the relationship between Pulse and Calories.
import pandas as pd import matplotlib.pyplot as plt import seaborn as sns df = pd.read_csv("data.csv") plot_df = df[ ["Pulse", "Calories"] ].dropna() plt.figure(figsize=(9, 6)) plt.scatter( plot_df["Pulse"], plot_df["Calories"], color="purple", alpha=0.7, edgecolors="black" ) plt.title("Pulse vs Calories") plt.xlabel("Pulse (Beats per Minute)") plt.ylabel("Calories Burned") plt.grid(True, linestyle="--", alpha=0.5) plt.tight_layout() plt.show()
Scatter plot with regression trendline
import pandas as pd import matplotlib.pyplot as plt import seaborn as sns df = pd.read_csv("data.csv") plot_df = df[ ["Pulse", "Calories"] ].dropna() plt.figure(figsize=(9, 6)) sns.regplot( data=plot_df, x="Pulse", y="Calories", scatter_kws={ "color": "purple", "alpha": 0.65 }, line_kws={ "color": "red", "linewidth": 2 } ) plt.title("Pulse vs Calories with Regression Trendline") plt.xlabel("Pulse") plt.ylabel("Calories Burned") plt.grid(True, alpha=0.4) plt.tight_layout() plt.show()
Analysis: Each point represents an exercise observation. The regression line summarizes the fitted linear trend. Its slope does not establish a causal relationship between pulse and calorie expenditure.
1.2.5 EDA practical output and interpretation
Expected analysis report
EDA operation
Expected result
Interpretation
head()
First five records
Initial data inspection
info()
Column types and non-null counts
Data structure
describe()
Mean, standard deviation, quartiles
Statistical distribution
isna().sum()
Missing count per feature
Data quality
dropna()
Reduced dataset
Complete-case dataset
fillna()
Imputed values
Missing-value treatment
corr()
Correlation coefficients
Linear relationships
Heatmap
Color-coded matrix
Visual correlation analysis
Box plot
Median, quartiles and outliers
Spread and unusual values
Scatter plot
Individual observations
Variable relationship
EDA interpretation questions
1. Why is EDA necessary before machine learning?
It identifies data-quality problems, unusual distributions, outliers and relationships that influence model selection and preprocessing.
2. Why use median instead of mean for skewed data?
The median is less sensitive to extreme values and therefore often represents the center of skewed data more reliably.
3. Why use a correlation heatmap?
It visually identifies relationships between numerical variables and helps investigate potential multicollinearity.
4. What is the difference between a box plot and a histogram?
A histogram displays frequency distribution across bins, whereas a box plot summarizes quartiles, median and potential outliers.
5. Does high correlation mean that two features should always be removed?
No. Feature importance, domain knowledge, model type and predictive evaluation must also be considered.
Practice task questions
Load data.csv using Pandas.
Display its first five and last five records.
Display shape, columns and data types.
Calculate mean, median, mode and standard deviation.
Find missing values in every column.
Remove incomplete records using dropna().
Impute missing numerical values using mean and median.
Calculate the Pearson correlation matrix.
Generate a Seaborn correlation heatmap.
Identify outliers using box plots.
Calculate IQR boundaries for each numerical variable.
Draw a scatter plot of Pulse against Calories.
Add a regression trendline.
Compare Pearson and Spearman correlation.
Write an interpretation of the dataset.
Common examiner traps
Important practical mistakes
Using df.corr() on an unsuitable dataset containing non-numerical columns without selecting numerical features.
Confusing dropna() with fillna().
Assuming missing values are always represented by zero.
Treating all outliers as incorrect data.
Confusing correlation with causation.
Calculating statistics on the wrong column.
Forgetting to call plt.show() in scripts.
Using mean imputation for heavily skewed data without justification.
Experiment 1.2 conclusion
EDA provides a systematic understanding of raw data through statistical analysis, missing-value treatment, correlation analysis and visualizations. It prepares the dataset for reliable feature selection and supervised learning.
EXPERIMENT 1.3: SUPERVISED LEARNING & CLASSIFIER MODELS
High-priority ML practical
1.3.1 Objective
[DIRECTLY IN NOTES]
To understand supervised learning and apply classification algorithms to train models on labeled datasets, enabling prediction of categorical outcomes and evaluation using appropriate performance metrics.
Platform: Google Colab / Jupyter Notebook.
Learning objectives
Understand supervised learning and classification.
Identify independent features and dependent labels.
Load and preprocess the Heart Disease dataset.
Split the dataset into training and testing subsets.
Apply feature scaling.
Train a Gaussian Naive Bayes classifier.
Evaluate the model using a confusion matrix and classification report.
Apply stratified cross-validation.
1.3.2 Supervised learning foundations
A. Definition
Supervised learning is a machine learning approach in which an algorithm learns from labeled training data.
Each training observation contains:
Input features \(X\).
Corresponding target label \(y\).
The objective is to learn a mapping function:
\[ f:X\rightarrow y \]
The model uses this learned relationship to predict the output for previously unseen observations.
B. Supervised learning architecture
LABELED DATASET | +--------+--------+ | | FEATURES X TARGET y | | +--------+--------+ | v TRAIN-TEST SPLIT | +--------+--------+ | | TRAINING DATA TEST DATA | v PREPROCESSING | v MODEL TRAINING | v TRAINED MODEL | +--------------------+ | | v v TEST FEATURES ACTUAL LABELS | v PREDICTION | v EVALUATION METRICS | v MODEL PERFORMANCE
C. Types of supervised learning
Type
Description
Example
Classification
Predicts categorical outputs
Disease / No Disease
Regression
Predicts continuous values
House prices
Classification can be divided into:
Binary classification: Two possible output classes.
Multiclass classification: More than two mutually exclusive classes.
Multilabel classification: An observation may belong to multiple labels simultaneously.
The Heart Disease practical uses binary classification.
D. Features and target variables
Suppose a dataset contains:
Age
Cholesterol
Pulse
Target
45
230
150
1
55
180
130
0
60
250
140
1
40
170
160
0
The independent variables are:
\[ X= \begin{bmatrix} 45&230&150\\ 55&180&130\\ 60&250&140\\ 40&170&160 \end{bmatrix} \]
The target vector is:
\[ y= \begin{bmatrix} 1\\0\\1\\0 \end{bmatrix} \]
Here:
\(X\) represents the input feature matrix.
\(y\) represents the output labels.
E. Training and testing
The dataset is generally divided into two parts:
Training dataset: Used to learn model parameters.
Testing dataset: Used to evaluate generalization on unseen observations.
The CU notes describe a typical split of 70–80% training and 20–30% testing.
For this experiment, we use:
\[ Training=80\% \]
\[ Testing=20\% \]
For \(N\) total observations:
\[ N_{train}\approx0.8N \]
\[ N_{test}\approx0.2N \]
Why stratify=y?
Stratification preserves approximately the same class proportions in training and testing subsets.
For example, if the complete dataset has:
Class
Percentage
Class 0
55%
Class 1
45%
The training and test sets should retain approximately these proportions.
F. Feature scaling
Feature scaling brings numerical variables onto comparable scales.
Two important methods are:
1. Min-Max normalization
\[ x'=\frac{x-x_{\min}}{x_{\max}-x_{\min}} \]
This generally transforms values into the interval:
\[ 0\leq x'\leq1 \]
2. Standardization (Z-score)
\[ z=\frac{x-\mu}{\sigma} \]
After standardization, the transformed training features have approximately:
\[ \mu=0,\qquad \sigma=1 \]
Comparison
Min-Max Scaling
Standard Scaling
Uses minimum and maximum
Uses mean and standard deviation
Usually produces 0–1
Usually centers around 0
Sensitive to extreme values
Also affected by outliers
Useful for bounded feature ranges
Common for SVM, KNN and linear models
Critical examiner warning
Never fit a scaler on the complete dataset before splitting into training and testing data. This leaks information from the test set into the training process.
Use:
scaler.fit(X_train) X_train_scaled = scaler.transform(X_train) X_test_scaled = scaler.transform(X_test)
An even safer approach is a Scikit-Learn Pipeline, particularly when performing cross-validation.
1.3.3 Bayes' Theorem and Gaussian Naive Bayes
[RESTORED STANDARD CODE / ARCHITECTURE] [LAB / EXAM SUPPORT]
A. Bayes' Theorem
Bayes' theorem calculates the probability of an event using prior knowledge and observed evidence.
\[ P(A|B)=\frac{P(B|A)P(A)}{P(B)} \]
Where:
Symbol
Meaning
\(P(A|B)\)
Posterior probability
\(P(B|A)\)
Likelihood
\(P(A)\)
Prior probability
\(P(B)\)
Evidence
B. Derivation
From the definition of conditional probability:
\[ P(A|B)=\frac{P(A\cap B)}{P(B)} \]
Similarly:
\[ P(B|A)=\frac{P(A\cap B)}{P(A)} \]
Rearranging:
\[ P(A\cap B)=P(B|A)P(A) \]
Substitute:
\[ P(A|B)=\frac{P(B|A)P(A)}{P(B)} \]
Therefore:
\[ \boxed{P(A|B)=\frac{P(B|A)P(A)}{P(B)}} \]
C. Numerical example
Suppose:
10% of patients have a hypothetical disease.
A test correctly returns positive for 90% of diseased patients.
5% of healthy patients also return positive.
Given:
\[ P(D)=0.10 \]
\[ P(+|D)=0.90 \]
\[ P(+|\neg D)=0.05 \]
We need to calculate:
\[ P(D|+) \]
Using total probability:
\[ P(+)=P(+|D)P(D)+P(+|\neg D)P(\neg D) \]
\[ P(+)=0.90(0.10)+0.05(0.90) \]
\[ P(+)=0.135 \]
Therefore:
\[ P(D|+)=\frac{0.90(0.10)}{0.135} \]
\[ \boxed{P(D|+)=0.6667} \]
The probability of disease given a positive result is approximately 66.67%.
This demonstrates why the probability of a positive test is not automatically the probability of having the disease.
D. Naive Bayes classifier
Naive Bayes applies Bayes' theorem with a conditional independence assumption between features given the class.
For features \(X_1,X_2,\ldots,X_n\):
\[ P(C|X_1,\ldots,X_n) \propto P(C)\prod_{i=1}^{n}P(X_i|C) \]
The predicted class is:
\[ \hat{C}=\arg\max_C \left[ P(C)\prod_{i=1}^{n}P(X_i|C) \right] \]
The conditional independence assumption simplifies probability estimation.
E. Gaussian Naive Bayes
Gaussian Naive Bayes is used when numerical feature values are modeled using Gaussian distributions within each class.
Its probability density function is:
\[ P(x_i|C)= \frac{1}{\sqrt{2\pi\sigma_C^2}} \exp\left( -\frac{(x_i-\mu_C)^2}{2\sigma_C^2} \right) \]
Where:
\(x_i\): Observed feature value.
\(\mu_C\): Feature mean for class \(C\).
\(\sigma_C^2\): Feature variance for class \(C\).
For multiple features:
\[ P(X|C)=\prod_{i=1}^{n}P(x_i|C) \]
Prediction:
\[ \hat{C}=\arg\max_C P(C)\prod_{i=1}^{n}P(x_i|C) \]
In practice, implementations use logarithms to avoid numerical underflow:
\[ \log P(C|X) \propto \log P(C)+\sum_i\log P(x_i|C) \]
Advantages
Simple to implement.
Computationally efficient.
Works with numerical features.
Can perform well on relatively small datasets.
Limitations
Assumes conditional independence.
Gaussian distribution may not describe every feature correctly.
Correlated features can violate its assumptions.
1.3.4 Heart Disease dataset architecture
[DIRECTLY IN NOTES] [RESTORED STANDARD CODE / ARCHITECTURE]
The practical uses a CSV dataset called heart.csv, with a 14-column architecture.
The filename heart.csv.csv mentioned in the requested specification may be the literal filename in some environments. The code below supports both filenames.
A. Feature descriptions
Feature
Description
Type
age
Patient age
Numerical
sex
Sex indicator
Categorical/binary
cp
Chest pain type
Categorical
trestbps
Resting blood pressure
Numerical
chol
Serum cholesterol
Numerical
fbs
Fasting blood sugar indicator
Binary
restecg
Resting ECG result
Categorical
thalach
Maximum heart rate achieved
Numerical
exang
Exercise-induced angina
Binary
oldpeak
ST depression
Numerical
slope
Slope of peak exercise ST segment
Categorical
ca
Number of major vessels
Discrete
thal
Thalassemia-related category
Categorical
target
Target disease classification
Binary
Target interpretation in the commonly used UCI-derived processed dataset:
target = 0: No disease.
target = 1: Disease present.
The exact encoding must be verified against the dataset documentation because Heart Disease datasets can use different target conventions.
B. Feature architecture
HEART.CSV | +-------+-------+ | | 13 FEATURES TARGET | | +------+-------+ | | | | NUMERICAL CATEGORICAL | | | | age sex | trestbps cp | chol fbs | thalach restecg | oldpeak exang | slope | ca | thal | | | | +------+-------+ | | | FEATURE MATRIX X y | | +-------+-------+ | CLASSIFIER | PREDICT TARGET
C. Dataset preparation and validation
Important: The commonly distributed processed Heart Disease dataset has 303 observations and 14 columns, but this must not be assumed for every CSV variant.
1.3.5 Complete Scikit-Learn practical: 15 codes
[DIRECTLY IN NOTES] [RESTORED STANDARD CODE / ARCHITECTURE]
The following sequence follows the lab workflow, with leakage-safe improvements where necessary.
Code 1: Install required libraries
!pip install -q pandas numpy matplotlib seaborn scikit-learn
Code 2: Import required libraries
import pandas as pd import numpy as np import matplotlib.pyplot as plt import seaborn as sns from sklearn.model_selection import ( train_test_split, StratifiedKFold, cross_val_score ) from sklearn.preprocessing import StandardScaler from sklearn.naive_bayes import GaussianNB from sklearn.pipeline import Pipeline from sklearn.metrics import ( accuracy_score, confusion_matrix, classification_report, precision_score, recall_score, f1_score, roc_auc_score, roc_curve, matthews_corrcoef, cohen_kappa_score ) import warnings warnings.filterwarnings("ignore") print("Libraries imported successfully.")
Expected output:
Libraries imported successfully.
Code 3: Load the Heart Disease dataset
import pandas as pd from pathlib import Path possible_files = [ "heart.csv", "heart.csv.csv" ] file_path = next( ( name for name in possible_files if Path(name).exists() ), None ) if file_path is None: raise FileNotFoundError( "Place heart.csv or heart.csv.csv in the working directory." ) df = pd.read_csv(file_path) print("Dataset Loaded Successfully") print("\nFirst Five Records:") print(df.head()) print("\nDataset Shape:") print(df.shape)
Expected output for the common 303-row version:
Dataset Loaded Successfully Dataset Shape: (303, 14)
If the supplied dataset differs, its actual shape will be displayed.
Code 4: Inspect dataset information
print("DATASET INFORMATION") df.info() print("\nDESCRIPTIVE STATISTICS") print(df.describe()) print("\nMISSING VALUES") print(df.isnull().sum()) print("\nDUPLICATE RECORDS") print(df.duplicated().sum()) print("\nTARGET DISTRIBUTION") print(df["target"].value_counts())
Expected analysis
info() reveals data types and non-null counts.
describe() summarizes numerical columns.
isnull().sum() reveals missing observations.
duplicated().sum() reveals repeated rows.
value_counts() reveals class balance.
Code 5: Clean the dataset
import pandas as pd import numpy as np df = df.copy() # Remove duplicate records df = df.drop_duplicates() # Convert possible question-mark missing values df = df.replace( ["?", "NA", "N/A", ""], np.nan ) # Validate target column if "target" not in df.columns: raise ValueError("Target column is missing.") # Convert all columns to numeric for column in df.columns: df[column] = pd.to_numeric( df[column], errors="coerce" ) # Remove observations without target labels df = df.dropna(subset=["target"]) # Validate binary target df = df[df["target"].isin([0, 1])] # Impute missing features with median feature_columns = [ column for column in df.columns if column != "target" ] for column in feature_columns: median_value = df[column].median() df[column] = df[column].fillna( median_value ) print("Cleaned Dataset Shape:", df.shape) print("\nMissing Values After Cleaning:") print(df.isnull().sum()) print("\nTarget Distribution:") print(df["target"].value_counts())
Why median imputation?
Median is less sensitive to extreme numerical observations than mean imputation.
Examiner's flag: This is a demonstration preprocessing procedure. For a rigorous evaluation pipeline, imputation must be fitted using training folds only, rather than being calculated before cross-validation.
Code 6: Separate features and target
X = df.drop( columns=["target"] ) y = df["target"] print("FEATURE MATRIX") print(X.head()) print("\nTARGET VECTOR") print(y.head()) print("\nFeature Matrix Shape:", X.shape) print("Target Vector Shape:", y.shape)
Expected shape for the common dataset:
Feature Matrix Shape: (303, 13) Target Vector Shape: (303,)
Code 7: Stratified train-test split
from sklearn.model_selection import train_test_split X_train, X_test, y_train, y_test = train_test_split( X, y, test_size=0.20, random_state=42, stratify=y ) print("Original Dataset Shape:", X.shape) print("Training Feature Shape:", X_train.shape) print("Testing Feature Shape:", X_test.shape) print("\nOriginal Target Shape:", y.shape) print("Training Target Shape:", y_train.shape) print("Testing Target Shape:", y_test.shape) print("\nTraining Class Distribution:") print(y_train.value_counts(normalize=True)) print("\nTesting Class Distribution:") print(y_test.value_counts(normalize=True))
Expected shape for 303 observations:
Original Dataset Shape: (303, 13) Training Feature Shape: (242, 13) Testing Feature Shape: (61, 13) Original Target Shape: (303,) Training Target Shape: (242,) Testing Target Shape: (61,)
The precise class counts depend on the dataset and stratified allocation.
Code 8: Feature scaling with StandardScaler
The original lab workflow introduces StandardScaler. For correct experimental practice, use a pipeline so that scaling is fitted only on the training observations.
from sklearn.preprocessing import StandardScaler scaler = StandardScaler() X_train_scaled = scaler.fit_transform( X_train ) X_test_scaled = scaler.transform( X_test ) print("Training Data After Scaling:") print(X_train_scaled[:5]) print("\nTesting Data After Scaling:") print(X_test_scaled[:5]) print("\nTraining Feature Mean:") print(np.round(X_train_scaled.mean(axis=0), 4)) print("\nTraining Feature Standard Deviation:") print(np.round(X_train_scaled.std(axis=0), 4))
Expected analysis:
Training feature means should be approximately zero.
Training population standard deviations should be approximately one.
Test data is transformed using the training set's mean and standard deviation.
Code 9: Initialize Gaussian Naive Bayes
from sklearn.naive_bayes import GaussianNB model = GaussianNB() print("Gaussian Naive Bayes Model:") print(model)
Expected output:
Gaussian Naive Bayes Model: GaussianNB()
Code 10: Create stratified K-fold cross-validation
from sklearn.model_selection import StratifiedKFold cv = StratifiedKFold( n_splits=5, shuffle=True, random_state=42 ) print("Cross-validation configuration:") print(cv) print("\nNumber of Folds:", cv.get_n_splits())
Expected output:
Cross-validation configuration: StratifiedKFold(n_splits=5, random_state=42, shuffle=True) Number of Folds: 5
Why five folds?
The data is divided into five subsets. Each subset serves as validation data once, while the remaining four subsets are used for training.
Code 11: Evaluate Gaussian Naive Bayes using cross-validation
A pipeline is used here to prevent scaling leakage across folds.
from sklearn.pipeline import Pipeline from sklearn.model_selection import cross_val_score pipeline = Pipeline([ ("scaler", StandardScaler()), ("classifier", GaussianNB()) ]) scores = cross_val_score( pipeline, X_train, y_train, cv=cv, scoring="accuracy" ) print("Cross Validation Accuracy Scores:") print(np.round(scores, 4)) print("\nMean Accuracy:") print(round(scores.mean(), 4)) print("\nStandard Deviation:") print(round(scores.std(), 4))
Expected output format
Cross Validation Accuracy Scores: [0.xxx 0.xxx 0.xxx 0.xxx 0.xxx] Mean Accuracy: 0.xxx Standard Deviation: 0.xxx
Exact scores depend on the input CSV and software version.
Code 12: Train the final model
pipeline.fit( X_train, y_train ) print("Gaussian Naive Bayes Model Trained Successfully.")
Expected output:
Gaussian Naive Bayes Model Trained Successfully.
Code 13: Generate predictions
y_pred = pipeline.predict( X_test ) y_probability = pipeline.predict_proba( X_test )[:, 1] comparison = pd.DataFrame({ "Actual": y_test.to_numpy(), "Predicted": y_pred }) print("ACTUAL VS PREDICTED VALUES") print(comparison.to_string(index=False)) print("\nFirst Five Positive-Class Probabilities:") print(np.round(y_probability[:5], 4))
Expected structure:
ACTUAL VS PREDICTED VALUES Actual Predicted 1 1 0 0 1 1 0 1 1 1 ...
The values above illustrate output structure, not guaranteed predictions for every dataset.
Code 14: Evaluate the model using classification metrics
A. Confusion matrix
cm = confusion_matrix( y_test, y_pred, labels=[0, 1] ) print("CONFUSION MATRIX") print(cm) tn, fp, fn, tp = cm.ravel() print("\nTrue Negative:", tn) print("False Positive:", fp) print("False Negative:", fn) print("True Positive:", tp)
Confusion matrix layout:
PREDICTED 0 1 ACTUAL 0 TN FP 1 FN TP
B. Classification report
print("CLASSIFICATION REPORT") print( classification_report( y_test, y_pred, labels=[0, 1], target_names=[ "No Disease", "Disease" ], zero_division=0 ) )
Expected report structure
precision recall f1-score support No Disease ... ... ... ... Disease ... ... ... ... accuracy ... ... macro avg ... ... ... ... weighted avg ... ... ... ...
C. Individual evaluation metrics
accuracy = accuracy_score( y_test, y_pred ) precision = precision_score( y_test, y_pred, zero_division=0 ) recall = recall_score( y_test, y_pred, zero_division=0 ) f1 = f1_score( y_test, y_pred, zero_division=0 ) specificity = tn / (tn + fp) if (tn + fp) else 0 mcc = matthews_corrcoef( y_test, y_pred ) kappa = cohen_kappa_score( y_test, y_pred ) auc = roc_auc_score( y_test, y_probability ) print("MODEL EVALUATION") print("Accuracy:", round(accuracy, 4)) print("Precision:", round(precision, 4)) print("Recall:", round(recall, 4)) print("Specificity:", round(specificity, 4)) print("F1 Score:", round(f1, 4)) print("ROC-AUC:", round(auc, 4)) print("MCC:", round(mcc, 4)) print("Cohen Kappa:", round(kappa, 4))
Code 15: ROC curve visualization
import matplotlib.pyplot as plt fpr, tpr, thresholds = roc_curve( y_test, y_probability ) auc_value = roc_auc_score( y_test, y_probability ) plt.figure(figsize=(8, 6)) plt.plot( fpr, tpr, color="blue", linewidth=2, label=f"GaussianNB AUC = {auc_value:.3f}" ) plt.plot( [0, 1], [0, 1], linestyle="--", color="red", label="Random Classifier" ) plt.xlabel("False Positive Rate") plt.ylabel("True Positive Rate") plt.title("ROC Curve - Heart Disease Classification") plt.legend() plt.grid(alpha=0.4) plt.tight_layout() plt.show()
1.3.6 Mathematical foundations of classification evaluation
[DIRECTLY IN NOTES] [LAB / EXAM SUPPORT]
A. Confusion matrix
A confusion matrix evaluates predicted labels against actual labels.
Predicted positive
Predicted negative
Actual positive
TP
FN
Actual negative
FP
TN
Definitions:
TP: True Positive.
TN: True Negative.
FP: False Positive.
FN: False Negative.
B. Accuracy
Measures the proportion of correctly classified observations.
\[ Accuracy=\frac{TP+TN}{TP+TN+FP+FN} \]
C. Precision
Measures how many predicted positive observations are actually positive.
\[ Precision=\frac{TP}{TP+FP} \]
D. Recall / Sensitivity
Measures how many actual positive observations are correctly identified.
\[ Recall=\frac{TP}{TP+FN} \]
E. Specificity
Measures the proportion of actual negative observations correctly identified.
\[ Specificity=\frac{TN}{TN+FP} \]
F. F1-score
The harmonic mean of precision and recall.
\[ F1=2\cdot\frac{Precision\cdot Recall} {Precision+Recall} \]
G. ROC curve and AUC
ROC stands for Receiver Operating Characteristic.
It plots:
\[ TPR=\frac{TP}{TP+FN} \]
Against:
\[ FPR=\frac{FP}{FP+TN} \]
AUC is the Area Under the ROC Curve.
AUC
General interpretation
1.0
Perfect ranking
0.9–1.0
Excellent discrimination
0.8–0.9
Good discrimination
0.7–0.8
Fair discrimination
0.5–0.6
Weak discrimination
0.5
Random ranking
These ranges are informal conventions, not universal guarantees of model quality.
H. Worked confusion matrix
Suppose:
\[ TP=40,\quad TN=45,\quad FP=5,\quad FN=10 \]
Total:
\[ N=40+45+5+10=100 \]
Accuracy:
\[ Accuracy=\frac{40+45}{100}=0.85 \]
\[ \boxed{Accuracy=85\%} \]
Precision:
\[ Precision=\frac{40}{40+5}=0.8889 \]
Recall:
\[ Recall=\frac{40}{40+10}=0.8 \]
Specificity:
\[ Specificity=\frac{45}{45+5}=0.9 \]
F1-score:
\[ F1=2\cdot\frac{0.8889\times0.8}{0.8889+0.8} \]
\[ \boxed{F1\approx0.8421} \]
Examiner's question: Why is accuracy sometimes misleading?
If 95% of observations belong to one class, a model that always predicts that class achieves 95% accuracy while completely failing to detect the minority class. Precision, recall, F1-score and class-specific confusion matrix values provide additional information.
1.3.7 Practical conclusion
The Heart Disease classification experiment demonstrates the complete supervised learning workflow:
Loading and inspecting labeled data.
Cleaning duplicate and missing observations.
Separating features and labels.
Performing a stratified 80:20 split.
Scaling numerical features without leakage.
Training Gaussian Naive Bayes.
Evaluating with stratified cross-validation.
Measuring classification performance using multiple metrics.
Visualizing ROC-AUC.
Important academic distinction: This is a machine learning educational experiment, not a clinically validated diagnostic system. A high test score does not establish medical reliability.
EXPERIMENT 1.4: COMPARATIVE CLASSIFICATION USING MULTIPLE MACHINE LEARNING ALGORITHMS
Final Experiment of Unit 1
1.4.1 Objective
[DIRECTLY IN NOTES]
To build and compare classification models using different machine learning algorithms, analyze their performance on a given dataset and identify the most suitable algorithm for accurate prediction.
Learning objectives
Understand different classification algorithms.
Implement six machine learning classifiers.
Apply stratified K-fold cross-validation.
Compare model performance using accuracy, precision, recall, F1-score and ROC-AUC.
Visualize classification results.
Identify an appropriate classifier for a given dataset.
Platform: Google Colab / Jupyter Notebook.
1.4.2 Theoretical comparison of six classifiers
A. Logistic Regression
[DIRECTLY IN NOTES] [RESTORED STANDARD CODE / ARCHITECTURE]
Logistic Regression is a supervised classification algorithm that predicts the probability of a categorical outcome.
It uses the logistic or sigmoid function:
\[ \sigma(z)=\frac{1}{1+e^{-z}} \]
Where:
\[ z=w_0+w_1x_1+w_2x_2+\cdots+w_nx_n \]
The predicted probability is:
\[ P(y=1|X)=\frac{1}{1+e^{-z}} \]
Classification rule:
\[ \hat y= \begin{cases} 1 & P(y=1|X)\geq0.5\\ 0 & P(y=1|X)<0.5 \end{cases} \]
Advantages
Simple and interpretable.
Produces class probabilities.
Computationally efficient.
Useful as a baseline classifier.
Limitations
Linear decision boundary unless features are transformed.
Sensitive to feature scaling.
May underperform on complex nonlinear relationships.
B. Support Vector Classifier (SVC)
SVC is based on Support Vector Machines.
Its objective is to find a decision boundary that maximizes the margin between different classes.
The hyperplane equation is:
\[ w^Tx+b=0 \]
For a linearly separable classification problem, the margin constraints are:
\[ y_i(w^Tx_i+b)\geq1 \]
The optimization objective is:
\[ \min_{w,b}\frac{1}{2}\|w\|^2 \]
For non-perfectly separable data, soft-margin SVM introduces slack variables and a regularization parameter.
Two important kernels
1. Linear kernel
\[ K(x_i,x_j)=x_i^Tx_j \]
2. Radial Basis Function (RBF) kernel
\[ K(x_i,x_j)= \exp(-\gamma\|x_i-x_j\|^2) \]
The RBF kernel can represent nonlinear decision boundaries.
Advantages
Effective in high-dimensional spaces.
Supports nonlinear classification using kernels.
Maximizes classification margin.
Limitations
Sensitive to parameter selection.
Scaling is generally important.
Training can become expensive on large datasets.
C. Decision Tree Classifier
A Decision Tree classifies data by repeatedly splitting observations according to feature conditions.
Architecture
ROOT NODE | Feature Condition / \ Yes No | | NODE A NODE B / \ / \ 0 1 0 1
Gini impurity
\[ Gini=1-\sum_{i=1}^{C}p_i^2 \]
For binary classification:
\[ Gini=1-(p_0^2+p_1^2) \]
Entropy
\[ H(S)=-\sum_{i=1}^{C}p_i\log_2(p_i) \]
Information Gain
\[ IG=H(parent)-\sum_j \frac{|S_j|}{|S|}H(S_j) \]
A decision tree selects splits that reduce impurity.
Advantages
Easy to interpret.
Handles nonlinear relationships.
Does not require feature scaling.
Can handle numerical and encoded categorical features.
Limitations
Can overfit.
Sensitive to changes in training data.
Deep trees may have poor generalization.
D. Random Forest Classifier
Random Forest is an ensemble learning algorithm that combines multiple decision trees.
It uses:
Bootstrap sampling of training observations.
Random feature selection at each split.
Multiple decision trees.
Aggregation of tree predictions.
Architecture
TRAINING DATA | +----------+----------+ | | | v v v TREE 1 TREE 2 TREE 3 | | | v v v CLASS 1 CLASS 1 CLASS 0 | | | +----------+----------+ | MAJORITY VOTE | v FINAL CLASS 1
Mathematical majority voting:
\[ \hat y=\operatorname{mode} \{T_1(X),T_2(X),\ldots,T_n(X)\} \]
Advantages
Reduces variance compared with an individual tree.
Handles complex nonlinear relationships.
Provides feature importance estimates.
Generally robust to overfitting compared with an unrestricted single tree.
Limitations
Less interpretable than one decision tree.
Can consume considerable memory.
Inference may be slower than simpler models.
E. K-Nearest Neighbors (KNN)
KNN is a distance-based classification algorithm.
It classifies a new observation using the majority class among its \(K\) nearest training observations.
Euclidean distance
\[ d(x,y)=\sqrt{\sum_{i=1}^{n}(x_i-y_i)^2} \]
Algorithm
NEW OBSERVATION | v CALCULATE DISTANCES | v SORT NEIGHBOURS | v SELECT K NEAREST | v MAJORITY VOTE | v PREDICT CLASS
Advantages
Simple and intuitive.
No explicit model-fitting stage.
Can represent nonlinear decision boundaries.
Limitations
Prediction can be computationally expensive.
Sensitive to feature scaling.
Sensitive to the choice of K.
Performance can decline in high-dimensional spaces.
F. Gaussian Naive Bayes
Gaussian Naive Bayes applies Bayes' theorem with a Gaussian distribution assumption for numerical features.
\[ P(C|X)\propto P(C)\prod_{i=1}^{n}P(x_i|C) \]
Its Gaussian likelihood is:
\[ P(x_i|C)= \frac{1}{\sqrt{2\pi\sigma_C^2}} \exp\left( -\frac{(x_i-\mu_C)^2}{2\sigma_C^2} \right) \]
Advantages
Fast training.
Low computational requirements.
Works well as a baseline classifier.
Limitations
Assumes conditional independence.
Assumes Gaussian feature distributions.
May be less accurate when these assumptions are violated.
1.4.3 Comparison of all six classifiers
Algorithm
Main principle
Feature scaling
Nonlinear capability
Logistic Regression
Sigmoid probability
Recommended
Limited without feature transformations
SVC
Maximum-margin hyperplane
Essential in most cases
Yes, with nonlinear kernels
Decision Tree
Recursive splitting
Not required
Yes
Random Forest
Ensemble of trees
Not required
Yes
KNN
Distance and majority voting
Essential in most cases
Yes
Gaussian NB
Bayes' theorem
Usually not required
Can model nonlinear boundaries
Important hyperparameters
Model
Hyperparameter
Purpose
Logistic Regression
C
Inverse regularization strength
SVC
C
Regularization
SVC
kernel
Linear or RBF transformation
SVC
gamma
RBF influence
Decision Tree
max_depth
Maximum tree depth
Random Forest
n_estimators
Number of trees
Random Forest
max_features
Features considered per split
KNN
n_neighbors
Number of nearest neighbours
Gaussian NB
var_smoothing
Numerical stability
1.4.4 Stratified K-Fold Cross-Validation
[DIRECTLY IN NOTES] [LAB / EXAM SUPPORT]
A. What is cross-validation?
Cross-validation is a model evaluation technique in which the available training dataset is divided into multiple subsets called folds.
For \(K\)-fold cross-validation:
Divide the dataset into \(K\) folds.
Train the model on \(K-1\) folds.
Validate it using the remaining fold.
Repeat until every fold has been used for validation.
Calculate the average performance.
Five-fold cross-validation architecture
TRAINING DATA | +---------+---------+ | | | v v v FOLD 1 FOLD 2 FOLD 3 | | | +---------+---------+ | FIVE FOLDS | +---------------+---------------+ | | | v v v ROUND 1 ROUND 2 ROUND 3 Validate 1 Validate 2 Validate 3 Train 2-5 Train 1,3-5 Train 1-2,4-5 | | | +---------------+---------------+ | REMAINING ROUNDS | v COLLECT ALL SCORES | v MEAN AND STD DEV
B. Why stratification?
Stratified K-Fold maintains approximately the same class proportions in every fold.
Consider a dataset with 100 observations:
Class
Observations
Percentage
Class 0
70
70%
Class 1
30
30%
Total
100
100%
For five-fold stratified cross-validation, each fold approximately contains:
Class
Observations per fold
Class 0
14
Class 1
6
Total
20
This prevents folds from having severely distorted class distributions.
C. Cross-validation mathematical formulation
Mean score:
\[ \bar{x}=\frac{1}{K}\sum_{i=1}^{K}x_i \]
Population standard deviation of fold scores:
\[ \sigma= \sqrt{ \frac{1}{K} \sum_{i=1}^{K}(x_i-\bar{x})^2 } \]
Scikit-Learn's cross_validate returns individual fold scores, allowing us to calculate their mean and standard deviation.
A smaller standard deviation generally indicates more consistent fold performance, although it does not guarantee better generalization.
1.4.5 Complete comparative classification implementation
[RESTORED STANDARD CODE / ARCHITECTURE]
The following implementation trains all six algorithms, performs five-fold stratified cross-validation and generates a comparison table.
Code 1: Install libraries
!pip install -q pandas numpy matplotlib seaborn scikit-learn
Code 2: Import libraries
import pandas as pd import numpy as np import matplotlib.pyplot as plt import seaborn as sns import time from pathlib import Path from sklearn.model_selection import ( train_test_split, StratifiedKFold, cross_validate ) from sklearn.preprocessing import StandardScaler from sklearn.pipeline import Pipeline from sklearn.impute import SimpleImputer from sklearn.linear_model import LogisticRegression from sklearn.svm import SVC from sklearn.tree import DecisionTreeClassifier from sklearn.ensemble import RandomForestClassifier from sklearn.neighbors import KNeighborsClassifier from sklearn.naive_bayes import GaussianNB from sklearn.metrics import ( accuracy_score, precision_score, recall_score, f1_score, roc_auc_score, confusion_matrix, classification_report, roc_curve, ConfusionMatrixDisplay ) import warnings warnings.filterwarnings("ignore") sns.set_theme(style="whitegrid") print("All libraries imported successfully.")
Code 3: Load the Heart Disease dataset
possible_files = [ "heart.csv", "heart.csv.csv" ] file_path = next( ( name for name in possible_files if Path(name).exists() ), None ) if file_path is None: raise FileNotFoundError( "Upload heart.csv or heart.csv.csv first." ) df = pd.read_csv(file_path) print("FIRST FIVE RECORDS") print(df.head()) print("\nDATASET SHAPE") print(df.shape) print("\nDATASET INFORMATION") df.info() print("\nMISSING VALUES") print(df.isna().sum()) print("\nTARGET DISTRIBUTION") print(df["target"].value_counts())
Code 4: Preprocess and validate data
df = df.copy() df = df.replace( ["?", "NA", "N/A", ""], np.nan ) for column in df.columns: df[column] = pd.to_numeric( df[column], errors="coerce" ) df = df.drop_duplicates() df = df.dropna( subset=["target"] ) df = df[ df["target"].isin([0, 1]) ] X = df.drop( columns=["target"] ) y = df["target"].astype(int) print("Cleaned Dataset Shape:", df.shape) print("\nFeature Shape:", X.shape) print("\nTarget Shape:", y.shape) print("\nClass Distribution:") print(y.value_counts())
Code 5: Split the dataset
X_train, X_test, y_train, y_test = train_test_split( X, y, test_size=0.20, random_state=42, stratify=y ) print("Training Shape:", X_train.shape) print("Testing Shape:", X_test.shape) print("\nTraining Target Distribution:") print(y_train.value_counts(normalize=True).round(3)) print("\nTesting Target Distribution:") print(y_test.value_counts(normalize=True).round(3))
Code 6: Create the six classification models
We use pipelines to ensure that missing-value imputation and scaling are fitted separately within each cross-validation training fold.
models = { "Logistic Regression": Pipeline([ ("imputer", SimpleImputer(strategy="median")), ("scaler", StandardScaler()), ("classifier", LogisticRegression( max_iter=2000, random_state=42 )) ]), "SVC Linear": Pipeline([ ("imputer", SimpleImputer(strategy="median")), ("scaler", StandardScaler()), ("classifier", SVC( kernel="linear", probability=True, random_state=42 )) ]), "SVC RBF": Pipeline([ ("imputer", SimpleImputer(strategy="median")), ("scaler", StandardScaler()), ("classifier", SVC( kernel="rbf", probability=True, random_state=42 )) ]), "Decision Tree": Pipeline([ ("imputer", SimpleImputer(strategy="median")), ("classifier", DecisionTreeClassifier( max_depth=5, random_state=42 )) ]), "Random Forest": Pipeline([ ("imputer", SimpleImputer(strategy="median")), ("classifier", RandomForestClassifier( n_estimators=200, random_state=42, n_jobs=-1 )) ]), "KNN": Pipeline([ ("imputer", SimpleImputer(strategy="median")), ("scaler", StandardScaler()), ("classifier", KNeighborsClassifier( n_neighbors=5 )) ]), "Gaussian NB": Pipeline([ ("imputer", SimpleImputer(strategy="median")), ("classifier", GaussianNB()) ]) } print("CLASSIFICATION MODELS CREATED") for name in models: print(name)
The two SVC kernels are evaluated separately. Thus, this implementation evaluates seven model configurations representing six algorithm families.
Code 7: Create stratified K-fold validation
cv = StratifiedKFold( n_splits=5, shuffle=True, random_state=42 ) print("Cross Validation:") print(cv) print("\nNumber of Folds:") print(cv.get_n_splits())
Code 8: Define evaluation metrics
scoring = { "Accuracy": "accuracy", "Precision": "precision", "Recall": "recall", "F1": "f1", "ROC_AUC": "roc_auc" } print("Evaluation Metrics:") print(list(scoring.keys()))
For binary classification, the default positive label is 1.
Code 9: Run cross-validation for all models
results = [] fold_results = {} for name, model in models.items(): print("\nEvaluating:", name) start_time = time.time() scores = cross_validate( model, X_train, y_train, cv=cv, scoring=scoring, return_train_score=False, n_jobs=-1, error_score="raise" ) execution_time = time.time() - start_time fold_results[name] = scores results.append({ "Model": name, "Accuracy": scores["test_Accuracy"].mean(), "Precision": scores["test_Precision"].mean(), "Recall": scores["test_Recall"].mean(), "F1": scores["test_F1"].mean(), "ROC-AUC": scores["test_ROC_AUC"].mean(), "Accuracy Std": scores["test_Accuracy"].std(), "Execution Time": execution_time }) print( "Mean Accuracy:", round(scores["test_Accuracy"].mean(), 4) )
Code 10: Generate the comparison table
comparison = pd.DataFrame(results) comparison = comparison.sort_values( by="F1", ascending=False ) comparison = comparison.reset_index( drop=True ) print("\nCOMPLETE MODEL COMPARISON") print( comparison.round(4).to_string( index=False ) ) print("\nBEST MODEL BASED ON F1 SCORE") print( comparison.iloc[0]["Model"] )
Expected output structure
Illustrative table format only. Actual scores must be obtained by running the dataset.
Model
Accuracy
Precision
Recall
F1
ROC-AUC
Logistic Regression
0.xxx
0.xxx
0.xxx
0.xxx
0.xxx
SVC Linear
0.xxx
0.xxx
0.xxx
0.xxx
0.xxx
SVC RBF
0.xxx
0.xxx
0.xxx
0.xxx
0.xxx
Decision Tree
0.xxx
0.xxx
0.xxx
0.xxx
0.xxx
Random Forest
0.xxx
0.xxx
0.xxx
0.xxx
0.xxx
KNN
0.xxx
0.xxx
0.xxx
0.xxx
0.xxx
Gaussian NB
0.xxx
0.xxx
0.xxx
0.xxx
0.xxx
Code 11: Grouped bar chart comparison
metrics = [ "Accuracy", "Precision", "Recall", "F1", "ROC-AUC" ] plot_df = comparison.set_index( "Model" )[metrics] ax = plot_df.plot( kind="bar", figsize=(13, 7), width=0.8 ) plt.title( "Performance Comparison of Classification Algorithms" ) plt.xlabel("Classification Models") plt.ylabel("Performance Score") plt.ylim(0, 1.05) plt.xticks(rotation=35, ha="right") plt.legend( title="Evaluation Metrics" ) plt.grid( axis="y", alpha=0.4 ) plt.tight_layout() plt.show()
Analysis: The grouped bar chart makes it possible to compare different metrics for every model.
Code 12: Train all models and create confusion matrices
trained_models = {} predictions = {} confusion_matrices = {} for name, model in models.items(): model.fit( X_train, y_train ) y_pred = model.predict( X_test ) trained_models[name] = model predictions[name] = y_pred confusion_matrices[name] = confusion_matrix( y_test, y_pred, labels=[0, 1] ) print( name, "Accuracy:", round( accuracy_score(y_test, y_pred), 4 ) )
Code 13: Confusion matrix visualization grid
model_names = list( trained_models.keys() ) fig, axes = plt.subplots( 3, 3, figsize=(15, 13) ) axes = axes.flatten() for i, name in enumerate(model_names): ConfusionMatrixDisplay( confusion_matrix=confusion_matrices[name], display_labels=["No Disease", "Disease"] ).plot( ax=axes[i], cmap="Blues", colorbar=False ) axes[i].set_title(name) for j in range( len(model_names), len(axes) ): axes[j].axis("off") plt.suptitle( "Confusion Matrix Comparison", fontsize=16 ) plt.tight_layout() plt.show()
Analysis: Each confusion matrix shows the correctly and incorrectly classified observations for a particular classifier.
Code 14: Multi-model ROC curve comparison
plt.figure(figsize=(10, 8)) for name, model in trained_models.items(): classifier = model[-1] if not hasattr( classifier, "predict_proba" ): continue probabilities = model.predict_proba( X_test )[:, 1] fpr, tpr, thresholds = roc_curve( y_test, probabilities ) auc_value = roc_auc_score( y_test, probabilities ) plt.plot( fpr, tpr, linewidth=2, label=f"{name} (AUC={auc_value:.3f})" ) plt.plot( [0, 1], [0, 1], linestyle="--", color="black", label="Random Classifier" ) plt.xlabel("False Positive Rate") plt.ylabel("True Positive Rate") plt.title("ROC Curve Comparison of Classification Models") plt.legend(loc="lower right") plt.grid(alpha=0.4) plt.tight_layout() plt.show()
Note: All classifiers in this implementation expose predict_proba() because SVC is configured with probability=True.
Code 15: Cross-validation accuracy boxplots
boxplot_data = [] for name, scores in fold_results.items(): for value in scores["test_Accuracy"]: boxplot_data.append({ "Model": name, "Accuracy": value }) boxplot_df = pd.DataFrame( boxplot_data ) plt.figure(figsize=(13, 7)) sns.boxplot( data=boxplot_df, x="Model", y="Accuracy" ) plt.title( "Cross-Validation Accuracy Distribution" ) plt.xlabel("Classification Models") plt.ylabel("Accuracy") plt.xticks( rotation=35, ha="right" ) plt.tight_layout() plt.show()
Analysis: Box plots reveal the distribution and variability of model accuracy across the validation folds.
Code 16: Final holdout evaluation table
The cross-validation table evaluates the training dataset. This final step evaluates each model independently on the untouched test dataset.
final_results = [] for name, model in trained_models.items(): y_pred = predictions[name] probabilities = model.predict_proba( X_test )[:, 1] final_results.append({ "Model": name, "Accuracy": accuracy_score( y_test, y_pred ), "Precision": precision_score( y_test, y_pred, zero_division=0 ), "Recall": recall_score( y_test, y_pred, zero_division=0 ), "F1": f1_score( y_test, y_pred, zero_division=0 ), "ROC-AUC": roc_auc_score( y_test, probabilities ) }) final_comparison = pd.DataFrame( final_results ) final_comparison = final_comparison.sort_values( by="F1", ascending=False ) print("FINAL TEST SET MODEL COMPARISON") print( final_comparison.round(4).to_string( index=False ) )
1.4.6 Interpreting the comparative results
[LAB / EXAM SUPPORT]
A. Which model is the best?
There is no universally best classification algorithm.
The best model depends on:
Dataset size.
Feature distribution.
Class imbalance.
Feature relationships.
Training time.
Interpretability.
Evaluation metric.
For example:
Requirement
Potentially suitable algorithm
Interpretable classification
Logistic Regression
Nonlinear classification
RBF SVC
Rule-based explanations
Decision Tree
Ensemble classification
Random Forest
Distance-based prediction
KNN
Fast probabilistic baseline
Gaussian Naive Bayes
B. Accuracy versus F1-score
A model with higher accuracy is not necessarily the best model when class distributions are imbalanced.
Consider:
Model
Accuracy
Precision
Recall
F1
A
0.95
0.60
0.40
0.48
B
0.90
0.85
0.82
0.83
Model A has greater accuracy, but Model B has a considerably better F1-score.
C. Cross-validation versus holdout evaluation
Cross-validation
Holdout testing
Uses multiple training/validation splits
Uses one fixed test set
Measures stability across folds
Measures final unseen-data performance
Useful for model comparison
Useful for final evaluation
Produces multiple scores
Produces one test score
Critical examiner warning: Do not use the final test set to repeatedly select hyperparameters or models. Doing so turns the test set into part of the model-selection process and compromises its independence.
For more advanced tuning, use GridSearchCV or RandomizedSearchCV within a properly designed validation procedure.
D. Computational complexity overview
Let:
\(N\): Number of training observations.
\(D\): Number of features.
\(T\): Number of trees.
\(K\): Number of nearest neighbours.
Algorithm
Approximate computational considerations
Logistic Regression
Depends on optimization iterations and matrix operations
Linear SVC
Depends on solver, data size and feature dimension
RBF SVC
Kernel methods can require substantial memory and computation
Decision Tree
Commonly around \(O(ND\log N)\) for balanced tree-building conditions
Random Forest
Approximately tree-building cost multiplied by \(T\)
KNN
Naive prediction approximately \(O(ND)\) per observation
Gaussian NB
Training approximately \(O(ND)\)
These are simplified estimates. Actual performance depends on implementation, data structure, kernel, sparsity and hardware.
Experiment 1.4 conclusion
This experiment demonstrates how different classification algorithms can be trained and evaluated on the same dataset.
Stratified K-fold cross-validation provides a more stable model comparison, while ROC curves, confusion matrices and grouped performance charts help assess classification quality.
UNIT 1: MASTER VIVA VOCE & EXAMINER QUESTION BANK
10 High-yield viva questions
[LAB / EXAM SUPPORT]
Experiment 1.1: Python, Pandas, NumPy and Matplotlib
Q1. What is the difference between NumPy and Pandas?
Answer: NumPy is primarily used for numerical computations using multidimensional arrays, whereas Pandas provides Series and DataFrame structures for labeled, tabular data manipulation and analysis.
Examiner follow-up: Which library is generally more convenient for handling missing values in tabular datasets?
Answer: Pandas.
Q2. What is the difference between a Series and a DataFrame?
Answer: A Series is a one-dimensional labeled array, while a DataFrame is a two-dimensional labeled structure containing rows and columns.
Examiner follow-up: Can a DataFrame contain different data types?
Answer: Yes. Different columns can contain different data types.
Q3. What is the difference between loc and iloc?
Answer: loc performs label-based indexing, whereas iloc performs integer-position-based indexing.
Examiner follow-up: Is the ending index included?
Answer: loc includes the ending label in a slice; iloc excludes the ending position.
Q4. What is vectorization in NumPy?
Answer: Vectorization means performing operations on entire arrays without explicitly writing Python loops for every element. It improves computational efficiency.
Examiner follow-up: What happens when we execute arr * 2?
Answer: Every element of the array is multiplied by two.
Experiment 1.2: Exploratory Data Analysis
Q5. What is EDA, and why is it performed?
Answer: Exploratory Data Analysis is the systematic examination of data using statistics and visualizations to understand distributions, detect missing values and outliers, and identify relationships before modeling.
Examiner follow-up: Name four important EDA visualizations.
Answer: Histogram, box plot, scatter plot and correlation heatmap.
Q6. What is the difference between mean and median?
Answer: Mean is the arithmetic average, while median is the middle observation after sorting the data. Median is generally less sensitive to extreme observations.
Examiner follow-up: Which measure is preferable for highly skewed data?
Answer: Median, in many practical situations.
Q7. What is IQR? How is it used to detect outliers?
Answer: Interquartile Range is the difference between the third and first quartiles.
\[ IQR=Q_3-Q_1 \]
Potential outlier boundaries are:
\[ Q_1-1.5(IQR) \]
and
\[ Q_3+1.5(IQR) \]
Examiner follow-up: Does every observation outside these boundaries have to be deleted?
Answer: No. It must first be investigated.
Q8. What is Pearson correlation?
Answer: Pearson correlation measures the strength and direction of a linear relationship between two numerical variables. Its value ranges from -1 to +1.
Examiner follow-up: Does correlation establish causation?
Answer: No.
Experiment 1.3 and 1.4: Machine Learning
Q9. What is supervised learning? Explain the difference between classification and regression.
Answer: Supervised learning trains a model using labeled data. Classification predicts categorical outputs, whereas regression predicts continuous numerical outputs.
Examiner follow-up: Which type of problem is Heart Disease prediction?
Answer: Binary classification, when the target contains two classes.
Q10. Why is stratified K-fold cross-validation important, and how do we evaluate classification models?
Answer: Stratified K-fold maintains approximately the same class distribution in each fold, making it useful for imbalanced classification datasets.
Common evaluation metrics include:
Accuracy.
Precision.
Recall.
F1-score.
ROC-AUC.
Confusion matrix.
Examiner follow-up: Which metric is particularly useful when balancing precision and recall?
Answer: F1-score.
UNIT 1: COMPLETE EXAMINER'S DEBUGGING CHECKLIST
[LAB / EXAM SUPPORT]
Before submitting a practical examination, verify the following.
Problem
Common cause
Solution
FileNotFoundError
CSV not uploaded
Verify filename and working directory
KeyError: 'target'
Incorrect column name
Check df.columns
ValueError: could not convert string to float
Text in numerical columns
Encode or clean data
Input contains NaN
Missing observations
Use imputation
Found input variables with inconsistent numbers of samples
Incorrect splitting
Check X and y shapes
UndefinedMetricWarning
No predicted positive samples
Inspect class predictions and use zero_division appropriately
Only one class present in y_true
Invalid fold or test split
Ensure sufficient class observations and stratification
could not convert string to float
Unencoded categorical values
Use an encoder
Poor KNN performance
Unscaled features
Apply StandardScaler
SVC takes too long
Large dataset or expensive kernel
Tune kernel and computational settings
Unrealistically high accuracy
Data leakage
Check preprocessing and splitting
Overfitting
Excessive model complexity
Regularize or control model depth
High-priority examiner flags
Critical mistakes that can cost practical marks
1. Data leakage
Fitting StandardScaler, an imputer or a feature selector on the complete dataset before splitting introduces information from test observations into training.
2. Incorrect target separation
Accidentally including target inside X creates target leakage and invalidates the experiment.
3. Confusing standard deviation formulas
Pandas uses sample standard deviation by default; NumPy uses population standard deviation by default.
4. Ignoring class imbalance
Accuracy alone may conceal poor minority-class performance.
5. Using the test set for hyperparameter tuning
The test set should remain untouched until final evaluation.
6. Incorrect positive-class interpretation
Precision and recall depend on which class is designated positive. Verify that class 1 represents the intended outcome.
7. Assuming scaling is mandatory for every algorithm
Scaling is especially important for KNN and SVC, but generally unnecessary for decision trees and random forests.
UNIT 1: QUICK REVISION FORMULA SHEET
A. Descriptive statistics
Concept
Formula
Mean
\(\mu=\frac{1}{N}\sum x_i\)
Population variance
\(\sigma^2=\frac{1}{N}\sum(x_i-\mu)^2\)
Population standard deviation
\(\sigma=\sqrt{\sigma^2}\)
Range
\(X_{\max}-X_{\min}\)
IQR
\(Q_3-Q_1\)
Z-score
\(z=\frac{x-\mu}{\sigma}\)
Pearson correlation
\(\frac{\operatorname{Cov}(X,Y)}{\sigma_X\sigma_Y}\)
B. Data preprocessing
Technique
Formula / Function
Min-Max normalization
\(x'=\frac{x-x_{\min}}{x_{\max}-x_{\min}}\)
Standardization
\(z=\frac{x-\mu}{\sigma}\)
Missing-value detection
df.isna().sum()
Missing-value removal
df.dropna()
Mean imputation
df.fillna(df.mean())
Duplicate detection
df.duplicated()
Duplicate removal
df.drop_duplicates()
C. Classification metrics
Metric
Formula
Accuracy
\(\frac{TP+TN}{TP+TN+FP+FN}\)
Precision
\(\frac{TP}{TP+FP}\)
Recall
\(\frac{TP}{TP+FN}\)
Specificity
\(\frac{TN}{TN+FP}\)
F1-score
\(2\frac{Precision\cdot Recall}{Precision+Recall}\)
TPR
\(\frac{TP}{TP+FN}\)
FPR
\(\frac{FP}{FP+TN}\)
D. Machine learning algorithms
Algorithm
Remember
Logistic Regression
Sigmoid function
SVC
Maximum-margin hyperplane
Decision Tree
Gini / Entropy
Random Forest
Bootstrap + ensemble voting
KNN
Distance-based classification
Gaussian NB
Bayes' theorem + Gaussian likelihood
E. Essential Python commands
Operation
Command
DataFrame creation
pd.DataFrame()
Read CSV
pd.read_csv()
First records
df.head()
Dataset information
df.info()
Statistics
df.describe()
NumPy mean
np.mean()
NumPy correlation
np.corrcoef()
Heatmap
sns.heatmap()
Scatter plot
plt.scatter()
Train-test split
train_test_split()
Scaling
StandardScaler()
Model training
model.fit()
Prediction
model.predict()
Cross-validation
cross_validate()
Confusion matrix
confusion_matrix()
Classification report
classification_report()
ROC-AUC
roc_auc_score()
UNIT 1: FINAL EXPERIMENT COMPLETION MATRIX
Experiment
Topic
Coverage
1.1
Python, Pandas, NumPy and Matplotlib
Completed
1.2
Exploratory Data Analysis
Completed
1.3
Supervised Learning and Gaussian NB
Completed
1.4
Comparative Classification
Completed
Viva
10 technical questions
Completed
Debugging
Common runtime and ML errors
Completed
Formula sheet
Statistical and ML formulas
Completed
Academic preparation recommendation: Practise Experiments 1.2, 1.3 and 1.4 by running the complete scripts in Google Colab. Pay particular attention to the distinction between cross-validation results and final test-set results, as this is a common area for examiner follow-up questions.

# UNIT 2: AI FUNDAMENTALS, GENERATIVE AI, TRANSFORMERS & AZURE

EXPERIMENT 2.1: ARTIFICIAL INTELLIGENCE FUNDAMENTALS AND AGENT ARCHITECTURES
2.1.1 Aim and objectives
[DIRECTLY IN NOTES]
Aim: To study the foundations of Artificial Intelligence, Generative AI, Large Language Models, Small Language Models and AI agent systems, and understand their applications through the Microsoft Azure ecosystem.
After completing this experiment, students should be able to:
Explain the major categories and capabilities of AI.
Differentiate AI, Machine Learning, Deep Learning and Generative AI.
Distinguish generative and discriminative probabilistic models.
Compare LLMs and SLMs in terms of model size and computational requirements.
Explain the components of an autonomous AI agent.
Describe the basic architecture of Azure Machine Learning and Azure OpenAI.
2.1.2 Artificial Intelligence taxonomy
[DIRECTLY IN NOTES + RESTORED STANDARD THEORY]
Artificial Intelligence is a field of computer science concerned with creating systems capable of performing tasks that normally require human intelligence.
Examples include:
Understanding natural language.
Recognizing objects in images.
Making predictions.
Planning actions.
Solving problems.
Generating text, images, audio and code.
AI can be classified by capability into three commonly discussed categories.
A. Artificial Narrow Intelligence (ANI)
ANI, also called Weak AI, is designed to perform a specific task or a limited group of tasks.
Examples:
Spam detection.
Face recognition.
Recommendation systems.
Voice assistants.
Medical image classification.
Machine translation.
Characteristics:
Operates within a defined task domain.
Does not possess general human-like intelligence.
Can outperform humans in specific narrow tasks.
Depends on its training, configuration and operating environment.
B. Artificial General Intelligence (AGI)
AGI is a hypothetical form of AI that would be able to learn, reason and perform a broad range of intellectual tasks at a level comparable to humans.
Expected capabilities would include:
General problem-solving.
Transfer of knowledge between unrelated domains.
Adaptation to unfamiliar tasks.
Flexible reasoning.
Learning with limited task-specific training.
Hypothetical capability
AGI should not be treated as an already established, universally agreed technical category of deployed AI.
C. Artificial Superintelligence (ASI)
ASI is a hypothetical intelligence that would significantly exceed human intellectual capabilities across most or all relevant domains.
Possible theoretical capabilities:
Advanced scientific discovery.
Complex strategic planning.
High-level autonomous problem-solving.
Superior performance across multiple intellectual disciplines.
Comparison table
Feature
ANI
AGI
ASI
Full form
Artificial Narrow Intelligence
Artificial General Intelligence
Artificial Superintelligence
Scope
Specific tasks
General intellectual tasks
Beyond human-level capability
Adaptability
Limited
Broad
Extremely broad
Current status
Widely deployed
Not established
Hypothetical
Example
Spam classifier
Theoretical human-level general AI
Theoretical superhuman AI
⚠ Examiner's flag: ChatGPT, image generators and other advanced generative systems are not automatically AGI. High performance across multiple tasks does not, by itself, prove general intelligence.
2.1.3 AI, Machine Learning, Deep Learning and Generative AI
[DIRECTLY IN NOTES + RESTORED STANDARD THEORY]
These concepts are related, but they are not interchangeable.
Conceptual hierarchy
Artificial Intelligence (AI)
The broad field of intelligent computer systems
Machine Learning (ML)
Learning patterns from data
Deep Learning (DL)
Multi-layer neural networks
Generative AI
Models that generate new content
Conceptual nesting for introductory study. Generative AI is not exclusively deep learning in every possible formulation, but modern foundation-model systems are predominantly deep-learning based.
Artificial Intelligence
AI is the broad discipline of building systems that perform tasks associated with intelligent behavior.
Machine Learning
ML is a subset of AI in which algorithms learn patterns from examples instead of relying entirely on manually written rules.
A basic supervised learning problem can be expressed as:
\[ \hat{f}=\arg\min_{f\in\mathcal{F}} \frac{1}{N}\sum_{i=1}^{N}L(f(x_i),y_i) \]
Where:
\(x_i\): Input sample.
\(y_i\): Actual output.
\(f(x_i)\): Model prediction.
\(L\): Loss function.
\(N\): Number of training samples.
\(\mathcal{F}\): Set of candidate models.
The objective is to find a model that minimizes prediction error.
Deep Learning
Deep Learning uses neural networks containing multiple computational layers.
A basic neural network layer is:
\[ a^{(l)}=\sigma(W^{(l)}a^{(l-1)}+b^{(l)}) \]
Where:
\(W^{(l)}\): Weight matrix.
\(b^{(l)}\): Bias vector.
\(\sigma\): Activation function.
\(a^{(l-1)}\): Previous layer's activation.
Deep Learning is widely used in:
Speech recognition.
Computer vision.
Natural language processing.
Autonomous systems.
Generative AI.
Generative AI
Generative AI learns patterns in training data and generates new content.
Examples:
Text generation.
Image generation.
Code generation.
Audio synthesis.
Video generation.
Key difference: A traditional classifier may predict whether an image contains a cat. A generative model may create a new image of a cat.
2.1.4 Generative AI versus Discriminative AI
[RESTORED STANDARD THEORY / CODE]
This distinction is especially important for mathematical and viva questions.
A. Discriminative models
A discriminative model learns the conditional probability:
\[ P(Y\mid X) \]
It estimates the probability of a class or output given an input.
Example:
Given a medical patient's features \(X\), predict whether the patient belongs to class \(Y=1\) or \(Y=0\).
For binary classification:
\[ P(Y=1\mid X)= \frac{1}{1+e^{-(w^TX+b)}} \]
This is the logistic sigmoid model.
The predicted class can be:
\[ \hat{Y}= \begin{cases} 1 & P(Y=1\mid X)\geq 0.5\\ 0 & P(Y=1\mid X)<0.5 \end{cases} \]
B. Generative models
A generative model learns the joint distribution:
\[ P(X,Y) \]
Using the probability chain rule:
\[ P(X,Y)=P(X\mid Y)P(Y) \]
Bayes' theorem gives:
\[ P(Y\mid X)= \frac{P(X\mid Y)P(Y)}{P(X)} \]
A generative classifier models how the input data is distributed for each class.
For example, Gaussian Naive Bayes assumes:
\[ P(X\mid Y=c)= \prod_{j=1}^{d}P(X_j\mid Y=c) \]
A text-generating language model instead learns a distribution over token sequences and generates tokens according to a conditional distribution such as:
\[ P(x_1,x_2,\ldots,x_T) = \prod_{t=1}^{T}P(x_t\mid x_1,\ldots,x_{t-1}) \]
The model predicts the next token based on preceding tokens.
Mathematical comparison
Property
Discriminative
Generative
Main probability
\(P(Y\mid X)\)
\(P(X,Y)\)
Learns
Decision boundary / conditional distribution
Data distribution and class relationship
Typical task
Classification
Data generation or generative classification
Example
Logistic Regression
Naive Bayes, Gaussian mixture models
Output
Class or probability
Samples or probability estimates
Important distinction: Generative AI is broader than generative classification. A text-generating LLM generally models token-sequence probabilities, not simply a joint distribution between a feature vector and a class label.
Worked probability example
Suppose:
\[ P(D)=0.01 \]
\[ P(+\mid D)=0.95 \]
\[ P(+\mid \neg D)=0.05 \]
We want to calculate the probability that a person has the disease after receiving a positive test.
By Bayes' theorem:
\[ P(D\mid +)= \frac{P(+\mid D)P(D)} {P(+)} \]
First:
\[ P(+)=P(+\mid D)P(D)+P(+\mid\neg D)P(\neg D) \]
\[ P(+)=0.95(0.01)+0.05(0.99) \]
\[ P(+)=0.0095+0.0495=0.059 \]
Therefore:
\[ P(D\mid +)=\frac{0.0095}{0.059} \]
\[ \boxed{P(D\mid +)\approx0.1610=16.10\%} \]
Interpretation: Even though the test has 95% sensitivity, the probability of disease after a positive result is approximately 16.10% because the disease is rare and false positives occur.
2.1.5 Large Language Models versus Small Language Models
[DIRECTLY IN NOTES + RESTORED STANDARD THEORY]
An LLM is a large neural language model trained on substantial text and other data. An SLM is a comparatively compact model intended to operate with fewer computational resources or within narrower application requirements.
Examples of model families include GPT-class models, Llama models, Phi models and other transformer-based language models. The exact size and capabilities depend on the particular model version.
Comparison
Feature
LLM
SLM
Parameter count
Often billions to hundreds of billions
Often hundreds of millions to several billions
Memory requirement
Higher
Lower
Hardware
Often GPU or accelerator infrastructure
Can run on smaller GPUs, CPUs or edge devices
Latency
Depends on model and deployment
Often lower for comparable hardware
Cost
Often higher
Often lower
Capability
Broad general-purpose tasks
Often optimized for narrower tasks
Deployment
Cloud, server or distributed infrastructure
Cloud, local server or edge
Model memory calculation
A model's parameter memory can be estimated as:
\[ M=P\times B \]
Where:
\(M\): Memory in bytes.
\(P\): Number of parameters.
\(B\): Bytes per parameter.
Common approximate storage sizes:
Precision
Bits per parameter
Bytes per parameter
FP32
32
4
FP16 / BF16
16
2
INT8
8
1
INT4
4
0.5
Example: 7-billion-parameter model
For a model with:
\[ P=7\times10^9 \]
FP16:
\[ M=7\times10^9\times2 =14\times10^9\text{ bytes} \]
Approximately 14 GB in decimal units.
INT8:
\[ M=7\times10^9\times1 =7\times10^9\text{ bytes} \]
Approximately 7 GB.
INT4:
\[ M=7\times10^9\times0.5 =3.5\times10^9\text{ bytes} \]
Approximately 3.5 GB.
Parameter storage only
These values do not include all runtime memory requirements.
Additional memory is required for:
KV cache.
Activations.
Temporary computation buffers.
Runtime overhead.
Quantization scales and metadata.
Framework and operating-system memory.
Quantization
Quantization represents model weights using lower-precision numerical formats.
Benefits:
Lower model memory.
Potentially higher inference throughput.
Reduced memory bandwidth.
Ability to run models on smaller devices.
Trade-offs:
Some quantization methods reduce model accuracy.
Hardware support affects speed.
INT4 implementations vary significantly.
Quantization does not guarantee faster execution on every device.
⚠ Examiner's flag: Do not claim that an INT4 model always uses exactly one-quarter of the total GPU memory of an FP16 model. The one-quarter estimate applies only to the raw parameter representation under the simplified calculation.
2.1.6 Autonomous AI Agent Systems
[DIRECTLY IN NOTES + RESTORED STANDARD THEORY]
An AI agent is a software system that receives information, interprets its environment, plans actions and uses tools to achieve a goal.
A basic AI agent contains:
Perception.
Planning.
Memory.
Action.
Four-pillar architecture
USER / ENVIRONMENT | v +------------------+ | PERCEPTION | | Text, image, | | audio, sensors | +------------------+ | v +------------------+ | PLANNING | | Reasoning, task | | decomposition | +------------------+ | +----------+----------+ | | v v +----------------+ +----------------+ | MEMORY | | ACTION | | Working memory | | APIs / Tools | | Vector memory | | Code execution | | Episodic data | | Search / DB | +----------------+ +----------------+ | | +----------+----------+ | v ENVIRONMENT FEEDBACK | +-------> PERCEPTION
Pillar 1: Perception
Perception is the process of collecting and interpreting information from the environment.
Input types:
Text.
Images.
Audio.
Video.
Sensor readings.
Documents.
Structured database records.
Example:
A customer-support agent receives a message:
My order has not arrived. Please check its status.
The perception component identifies the user's intent as an order-status request.
Pillar 2: Planning
Planning determines what steps are required to achieve the goal.
Common planning approaches:
ReAct: Reasoning + Acting
ReAct alternates between reasoning and actions.
Thought: I need to identify the order. Action: Search the order database. Observation: Order #105 is in transit. Thought: I should retrieve the estimated delivery. Action: Call delivery tracking API. Observation: Expected delivery is tomorrow. Final: Your order is expected tomorrow.
Chain-of-Thought (CoT)
CoT refers to prompting or model behavior that encourages multi-step reasoning rather than an immediate short answer.
For deployed systems, internal reasoning should not be treated as a guaranteed source of correctness. The application should validate outputs and use tools or evidence where needed.
Tree-of-Thoughts (ToT)
ToT explores multiple candidate reasoning paths before selecting a promising path.
Initial problem | +---------+---------+ | | | Path A Path B Path C | | | Evaluate Evaluate Evaluate | | | +---------+---------+ | Select best path
Pillar 3: Memory
Memory allows an agent to retain information across steps or interactions.
Memory type
Purpose
Example
Working memory
Information required for the current task
Current user request
Long-term vector memory
Semantic retrieval of stored information
Search similar past support cases
Episodic memory
Records of previous events or interactions
Previous order complaint
A vector database stores numerical embeddings that can be compared using similarity metrics.
Cosine similarity:
\[ \operatorname{cos}(A,B)= \frac{A\cdot B}{\|A\|\|B\|} \]
Pillar 4: Action
Action is the ability to interact with external systems.
Examples:
Call an API.
Search a database.
Execute Python code.
Send a notification.
Retrieve a document.
Update an order record.
An agent should use permissions and validation before executing operations that affect real systems.
Agent feedback loop
A simplified agent can be represented as:
\[ s_t \rightarrow a_t \rightarrow r_{t+1} \]
Where:
\(s_t\): Current state.
\(a_t\): Selected action.
\(r_{t+1}\): Feedback or result.
The next state is:
\[ s_{t+1}=T(s_t,a_t) \]
Here \(T\) represents the environment's transition function.
2.1.7 Azure Machine Learning platform architecture
[RESTORED STANDARD THEORY / AZURE ARCHITECTURE]
Azure Machine Learning is a cloud platform used to develop, train, evaluate, deploy and manage machine-learning models.
Major components
Component
Purpose
Workspace
Central resource for an ML project
Compute instance
Managed development environment
Compute cluster
Scalable compute for training jobs
Datastore
Connection to storage
Data asset
Versioned reference to data
Environment
Software dependencies for jobs
Pipeline
Connected sequence of ML tasks
Model registry
Stores and versions models
Online endpoint
Real-time model inference
Batch endpoint
Large-scale asynchronous inference
Architecture diagram
AZURE SUBSCRIPTION | v RESOURCE GROUP | v AZURE MACHINE LEARNING WORKSPACE | +-----------------+------------------+ | | | v v v DATASTORES COMPUTE REGISTRY | | | v v | Data Assets Training Jobs | | | | +-----------------+------------------+ | v ML PIPELINE | +-----------+-----------+ | | v v MODEL EVALUATION MODEL REGISTER | v DEPLOYMENT | +---------+---------+ | | v v ONLINE ENDPOINT BATCH ENDPOINT
Azure OpenAI Service architecture
Azure OpenAI provides access to supported OpenAI models through Azure-managed resources and deployment configurations.
CLIENT APPLICATION | v APPLICATION BACKEND | Authentication | v AZURE OPENAI RESOURCE | Model Deployment | v FOUNDATION MODEL | +-----------+-----------+ | | v v Input Processing Output Generation | | +-----------+-----------+ | v CLIENT RESPONSE
Important distinction: Azure Machine Learning and Azure OpenAI are related parts of the Azure AI ecosystem, but they are different services. Azure Machine Learning supports the broader ML lifecycle. Azure OpenAI provides access to deployed foundation models through its service interfaces.
Practical example
A university wants to build a student-support assistant.
Azure OpenAI: Generate natural-language responses.
Azure AI Search: Retrieve relevant university documents.
Azure Machine Learning: Train and manage a separate student-risk prediction model.
Azure Storage: Store source documents and datasets.
Application backend: Connect the services and enforce permissions.
2.1.8 Python practical: Generative versus discriminative classification
[RESTORED STANDARD CODE]
This experiment demonstrates:
A discriminative model using Logistic Regression.
A generative classifier using Gaussian Naive Bayes.
A comparison of their classification metrics.
Install dependencies:
python -m pip install numpy pandas scikit-learn
Complete executable program:

```python
import numpy as np
import pandas as pd
from sklearn.datasets import make_classification
from sklearn.model_selection import train_test_split
from sklearn.pipeline import Pipeline
from sklearn.preprocessing import StandardScaler
from sklearn.linear_model import LogisticRegression
from sklearn.naive_bayes import GaussianNB
from sklearn.metrics import accuracy_score, classification_report

# 1. Generate a reproducible classification dataset
X, y = make_classification(
    n_samples=1000,
    n_features=8,
    n_informative=5,
    n_redundant=1,
    n_classes=2,
    random_state=42
)

# 2. Stratified train-test split (80/20)
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.20, random_state=42, stratify=y
)

# 3. Discriminative model (Logistic Regression)
logistic_model = Pipeline([
    ("scaler", StandardScaler()),
    ("classifier", LogisticRegression(max_iter=1000, random_state=42))
])

# 4. Generative model (Gaussian Naive Bayes)
generative_model = Pipeline([
    ("scaler", StandardScaler()),
    ("classifier", GaussianNB())
])

# 5. Train both models
logistic_model.fit(X_train, y_train)
generative_model.fit(X_train, y_train)

# 6. Generate predictions
logistic_preds = logistic_model.predict(X_test)
generative_preds = generative_model.predict(X_test)

# 7. Model comparison
comparison = pd.DataFrame({
    "Model": ["Logistic Regression (Discriminative)", "Gaussian Naive Bayes (Generative)"],
    "Accuracy": [accuracy_score(y_test, logistic_preds), accuracy_score(y_test, generative_preds)]
})

print("MODEL COMPARISON:")
print(comparison.round(4).to_string(index=False))
print("\n--- LOGISTIC REGRESSION REPORT ---")
print(classification_report(y_test, logistic_preds))
print("--- GAUSSIAN NAIVE BAYES REPORT ---")
print(classification_report(y_test, generative_preds))
```

Expected output format:
MODEL COMPARISON Model Accuracy Logistic Regression 0.xxx Gaussian Naive Bayes 0.xxx LOGISTIC REGRESSION REPORT precision recall f1-score support 0 ... 1 ... GAUSSIAN NAIVE BAYES REPORT precision recall f1-score support 0 ... 1 ...
The exact metrics are calculated at runtime. They should not be memorized as fixed values because they depend on the generated data and software version.
Analysis: Logistic Regression directly models the conditional class probability. Gaussian Naive Bayes models class-conditional feature distributions and class priors, then applies Bayes' theorem.
2.1.9 Examiner's flags
Important
ANI, AGI and ASI describe capability levels, not model sizes.
Machine Learning is a subset of AI.
Deep Learning is a subset of Machine Learning.
A generative model is not necessarily a text generator.
LLM does not mean that every model has the same parameter count.
FP16, INT8 and INT4 describe numerical representations, not model intelligence.
Agent memory and model weights are different concepts.
An AI agent is not merely a chatbot. It can select and execute actions.
An API call should not be confused with the model's reasoning process.
Azure Machine Learning and Azure OpenAI are separate services.
EXPERIMENT 2.2: TRANSFORMER ARCHITECTURE, ATTENTION AND EMBEDDINGS
2.2.1 Aim
[DIRECTLY IN NOTES + RESTORED STANDARD THEORY]
To understand how modern Generative AI models process language using tokenization, embeddings, transformer architecture, attention mechanisms and prompt-based adaptation.
2.2.2 Evolution from RNNs to Transformers
Recurrent Neural Networks (RNNs)
An RNN processes sequential data one element at a time.
For an input sequence:
\[ x_1,x_2,\ldots,x_T \]
The hidden state at time \(t\) is:
\[ h_t=\tanh(W_{xh}x_t+W_{hh}h_{t-1}+b_h) \]
The current state depends on the previous hidden state.
Limitations:
Sequential processing makes parallelization difficult.
Long-range dependencies can be difficult to preserve.
Gradients may vanish or explode during training.
Processing long sequences can be slow.
Long Short-Term Memory (LSTM)
LSTM networks introduce gates to regulate information flow.
The forget gate is:
\[ f_t=\sigma(W_f[x_t,h_{t-1}]+b_f) \]
The input gate is:
\[ i_t=\sigma(W_i[x_t,h_{t-1}]+b_i) \]
The candidate cell state is:
\[ \tilde{C}_t=\tanh(W_C[x_t,h_{t-1}]+b_C) \]
The cell state is updated:
\[ C_t=f_t\odot C_{t-1}+i_t\odot\tilde{C}_t \]
The output gate is:
\[ o_t=\sigma(W_o[x_t,h_{t-1}]+b_o) \]
The hidden state is:
\[ h_t=o_t\odot\tanh(C_t) \]
LSTMs help preserve long-term information, but they still process sequences recurrently.
Transformers
Transformers use attention mechanisms to model relationships between tokens.
Unlike standard RNNs, transformer layers can process the tokens of an input sequence in parallel during training.
Advantages:
Better parallelization.
Effective modeling of long-range dependencies.
Flexible attention between tokens.
Strong performance in language, vision and multimodal tasks.
⚠ Examiner's flag: Transformers do not eliminate every computational limitation. Standard self-attention has a quadratic sequence-length cost in its attention matrix.
For sequence length \(n\), the attention matrix contains:
\[ n\times n=n^2 \]
attention scores per head.
2.2.3 Complete Transformer architecture
[RESTORED STANDARD THEORY]
The original Transformer architecture contains an encoder and a decoder.
SOURCE SENTENCE | v SOURCE TOKENIZER | v TOKEN EMBEDDINGS | v POSITIONAL ENCODING | v +---------------------+ | ENCODER STACK | | | | Multi-Head Attention| | Add & Layer Norm | | Feed Forward Network| | Add & Layer Norm | +---------------------+ | | Encoder output v +---------------------+ | DECODER STACK | | | TARGET TOKENS -> Masked Self-Attention | Add & Layer Norm | | Cross-Attention |<--- Encoder output | Add & Layer Norm | | Feed Forward Network| | Add & Layer Norm | +---------------------+ | v LINEAR LAYER | v SOFTMAX | v NEXT TOKEN OUTPUT
Encoder
The encoder reads the input sequence and creates contextual representations.
Each encoder layer typically contains:
Multi-head self-attention.
Residual connection and layer normalization.
Position-wise feed-forward network.
Another residual connection and normalization.
Decoder
The decoder generates output tokens.
It typically contains:
Masked self-attention.
Cross-attention to encoder output.
Feed-forward network.
Residual connections and layer normalization.
Model architecture families
Architecture
Structure
Example use
Encoder-only
Transformer encoder
Text classification and representation
Decoder-only
Causal transformer decoder
Autoregressive text generation
Encoder-decoder
Both encoder and decoder
Sequence-to-sequence tasks
Examples:
BERT: Encoder-only.
GPT-style autoregressive models: Decoder-only.
T5: Encoder-decoder.
2.2.4 Token embeddings and positional encoding
A transformer receives numerical vectors rather than raw words.
Suppose a sentence is tokenized into:
AI models learn from data
A tokenizer may produce:
["AI", "models", "learn", "from", "data"]
Each token is converted into an embedding vector.
However, attention alone does not inherently encode token order. Positional information is therefore introduced.
Sinusoidal positional encoding
[RESTORED STANDARD THEORY]
For position \(pos\) and embedding dimension \(i\):
\[ PE(pos,2i)= \sin\left( \frac{pos}{10000^{2i/d_{\text{model}}}} \right) \]
\[ PE(pos,2i+1)= \cos\left( \frac{pos}{10000^{2i/d_{\text{model}}}} \right) \]
Where:
\(pos\): Token position.
\(i\): Dimension index.
\(d_{\text{model}}\): Embedding dimension.
The positional encoding is added to the token embedding:
\[ Z=E+PE \]
Where:
\(E\): Token embedding matrix.
\(PE\): Positional encoding matrix.
\(Z\): Position-aware input representation.
Why use sine and cosine?
Different dimensions use different frequencies. This creates a representation of position that varies smoothly and can help the model learn relative positions.
2.2.5 Scaled Dot-Product Attention
High-yield derivation
[RESTORED STANDARD THEORY]
Attention enables each token to assign different importance to other tokens.
The three principal matrices are:
Query \(Q\)
Key \(K\)
Value \(V\)
Step 1: Calculate similarity scores
The dot product between queries and keys is:
\[ S=QK^T \]
A large score indicates a stronger compatibility between a query and a key.
Step 2: Scale the scores
\[ S_{\text{scaled}}= \frac{QK^T}{\sqrt{d_k}} \]
Where \(d_k\) is the key-vector dimension.
Step 3: Apply softmax
\[ A=\operatorname{softmax} \left( \frac{QK^T}{\sqrt{d_k}} \right) \]
The softmax function is:
\[ \operatorname{softmax}(z_i)= \frac{e^{z_i}}{\sum_j e^{z_j}} \]
Each row of the resulting attention matrix represents normalized attention weights.
Step 4: Multiply by values
\[ \boxed{ \operatorname{Attention}(Q,K,V)= \operatorname{softmax} \left( \frac{QK^T}{\sqrt{d_k}} \right)V } \]
Why divide by \(\sqrt{d_k}\)?
Suppose the query and key components are independent, zero-mean random variables with unit variance.
The dot product is:
\[ q\cdot k=\sum_{i=1}^{d_k}q_i k_i \]
Under these assumptions, the variance of the sum grows approximately as:
\[ \operatorname{Var}(q\cdot k)=d_k \]
Therefore, the standard deviation grows as:
\[ \operatorname{Std}(q\cdot k)=\sqrt{d_k} \]
If \(d_k\) is large, the dot-product scores can become large in magnitude.
Large logits can push softmax toward saturated probabilities. In saturated regions, gradients become small, making learning less stable.
Dividing by \(\sqrt{d_k}\) keeps the score scale more controlled.
Conclusion: The scaling factor helps stabilize softmax inputs and their gradients.
2.2.6 Multi-Head Attention
Instead of performing attention once, the transformer performs several attention operations in parallel.
For head \(i\):
\[ head_i= \operatorname{Attention} (QW_i^Q,KW_i^K,VW_i^V) \]
The heads are concatenated:
\[ MultiHead(Q,K,V)= Concat(head_1,\ldots,head_h)W^O \]
Where:
\(h\): Number of attention heads.
\(W_i^Q\): Query projection.
\(W_i^K\): Key projection.
\(W_i^V\): Value projection.
\(W^O\): Output projection.
Different heads can learn different relationships, such as:
Local word relationships.
Long-range dependencies.
Syntactic patterns.
Semantic relationships.
2.2.7 Python implementation of scaled dot-product attention
[LAB / EXAM SUPPORT]
Install NumPy:
python -m pip install numpy
Complete code:

```python
import numpy as np

def softmax(x, axis=-1):
    """Numerically stable softmax along specified axis."""
    x_shifted = x - np.max(x, axis=axis, keepdims=True)
    exp_x = np.exp(x_shifted)
    return exp_x / np.sum(exp_x, axis=axis, keepdims=True)

def scaled_dot_product_attention(Q, K, V):
    """
    Computes Scaled Dot-Product Attention:
    Attention(Q, K, V) = softmax(Q @ K.T / sqrt(d_k)) @ V
    """
    d_k = K.shape[-1]
    # Step 1: Raw dot-product compatibility scores
    scores = Q @ K.T
    # Step 2: Scale by sqrt(d_k) to prevent gradient saturation
    scaled_scores = scores / np.sqrt(d_k)
    # Step 3: Normalize with Softmax to get attention weights
    weights = softmax(scaled_scores, axis=-1)
    # Step 4: Weighted combination of Values
    output = weights @ V
    return output, weights

# Example with 3 sequence tokens, key dimension d_k = 2, value dimension d_v = 2
Q = np.array([[1.0, 0.0], [0.0, 1.0], [1.0, 1.0]])
K = np.array([[1.0, 0.0], [0.0, 1.0], [1.0, 1.0]])
V = np.array([[10.0, 0.0], [0.0, 10.0], [5.0, 5.0]])

output, weights = scaled_dot_product_attention(Q, K, V)
print("ATTENTION WEIGHTS MATRIX (Sum of each row = 1.0):")
print(np.round(weights, 4))
print("\nCONTEXTUAL ATTENTION OUTPUT:")
print(np.round(output, 4))
```

Expected output:
ATTENTION WEIGHTS: [[0.4011 0.1978 0.4011] [0.1978 0.4011 0.4011] [0.2483 0.2483 0.5035]] ATTENTION OUTPUT: [[6.012 3.989] [3.989 6.012] [4.765 4.765]]
Small rounding differences may occur. The weights in each row should sum to approximately 1.2.2.8 Subword tokenization algorithms
[DIRECTLY IN NOTES: TOKENIZATION; RESTORED STANDARD ALGORITHMS]
Tokenization converts text into units that a model can process.
A tokenizer may use:
Words.
Subwords.
Characters.
Bytes.
Punctuation marks.
Subword tokenization balances vocabulary size and the ability to represent rare words.
A. Byte-Pair Encoding (BPE)
BPE starts with small units, commonly characters or bytes, and repeatedly merges the most frequent adjacent pair.
Example training corpus:
low lower lowest new newer
For a simplified character-level demonstration, consider the words:
l o w l o w e r l o w e s t
The pair l o occurs three times, so merge it:
Iteration
Most frequent pair
Merge result
Initial
None
l o w
1
l + o
lo
2
lo + w
low
3
e + r
er
4
e + s
es
The learned vocabulary can now represent common word fragments efficiently.
BPE inference example:
lowest
Possible segmentation:
low + est
The exact segmentation depends on the learned merge ranks.
B. WordPiece
WordPiece is a subword tokenization algorithm used in models such as BERT.
It builds a vocabulary of subword units and selects segmentations based on a learned scoring criterion.
A simplified segmentation example:
unhappiness
Possible result:
un ##happi ##ness
The ## marker indicates that the subword is not at the beginning of the word.
WordPiece does not simply choose the most frequent adjacent pair in the same way as basic BPE.
C. SentencePiece
SentencePiece is a tokenizer framework that can operate directly on raw text without requiring conventional word-level preprocessing.
It supports algorithms such as:
Unigram language model tokenization.
BPE tokenization.
It commonly represents spaces using a special visible marker such as:
▁
Example:
I love machine learning
Possible token representation:
▁I ▁love ▁machine ▁learning
Comparison
Feature
BPE
WordPiece
SentencePiece
Core idea
Repeated pair merging
Score-based subword vocabulary
Tokenizer framework
Input
Characters or bytes
Usually pre-tokenized words
Raw text
Space handling
Depends on implementation
Usually word-aware
Explicit whitespace representation
Common association
GPT-style tokenizers
BERT
T5 and multilingual models
⚠ Examiner's flag: BPE, WordPiece and SentencePiece are not three identical algorithms. SentencePiece is a framework that can implement different subword approaches.
2.2.9 Word and sentence embeddings
[DIRECTLY IN NOTES + RESTORED STANDARD THEORY]
An embedding is a numerical vector representation of a token, word, sentence or document.
Example:
"machine learning"
May be represented by a vector such as:
\[ v=[0.12,0.45,0.31,0.78] \]
Real embeddings usually contain many more dimensions.
A. Word2Vec
Word2Vec learns word representations from context.
Two major architectures are:
CBOW: Continuous Bag of Words
Predicts the center word from surrounding context words.
Context words | v CBOW | v Predicted center word
Example:
The student studies machine ___
The model predicts:
learning
Skip-Gram
Predicts surrounding context words from a center word.
Center word | v Skip-Gram | v Context words
Example:
Center word: learning
Possible context predictions:
machine, studies
B. GloVe
GloVe stands for Global Vectors for Word Representation.
It learns word vectors using global word co-occurrence statistics.
The objective is commonly written as:
\[ J=\sum_{i,j}f(X_{ij}) \left( w_i^T\tilde{w}_j+b_i+\tilde{b}_j -\log X_{ij} \right)^2 \]
Where:
\(X_{ij}\): Number of times word \(j\) occurs in the context of word \(i\).
\(w_i\): Word vector.
\(\tilde{w}_j\): Context vector.
\(b_i,\tilde{b}_j\): Bias terms.
\(f(X_{ij})\): Weighting function.
C. Contextual transformer embeddings
Traditional Word2Vec and GloVe generally assign a fixed vector to a word.
Transformer-based embeddings can change according to context.
Example:
The bank approved the loan.
The boat reached the river bank.
The word "bank" has different meanings in the two sentences. Contextual embeddings can represent those meanings differently.
2.2.10 Cosine similarity
Cosine similarity measures the angle between two vectors.
\[ \boxed{ \operatorname{cosine}(A,B)= \frac{A\cdot B}{\|A\|\|B\|} } \]
Where:
\[ A\cdot B=\sum_{i=1}^{n}A_iB_i \]
\[ \|A\|=\sqrt{\sum_{i=1}^{n}A_i^2} \]
Interpretation:
Similarity
General interpretation
Near +1
Similar direction
Near 0
Approximately orthogonal
Near -1
Opposite direction
Solved numerical example
Let:
\[ A=[1,2,3] \]
\[ B=[2,4,6] \]
Dot product:
\[ A\cdot B=1(2)+2(4)+3(6)=28 \]
Norms:
\[ \|A\|=\sqrt{1+4+9}=\sqrt{14} \]
\[ \|B\|=\sqrt{4+16+36}=\sqrt{56} \]
Therefore:
\[ \operatorname{cosine}(A,B)= \frac{28}{\sqrt{14}\sqrt{56}} \]
\[ \boxed{\operatorname{cosine}(A,B)=1} \]
The vectors point in exactly the same direction.
Python implementation:

```python
import numpy as np

def cosine_similarity(a, b):
    """Calculates cosine similarity between two 1D numerical vectors."""
    a = np.asarray(a, dtype=float)
    b = np.asarray(b, dtype=float)
    if a.shape != b.shape:
        raise ValueError("Vectors must have identical dimensions.")
    norm_a = np.linalg.norm(a)
    norm_b = np.linalg.norm(b)
    if norm_a == 0 or norm_b == 0:
        raise ValueError("Cosine similarity undefined for zero vectors.")
    return np.dot(a, b) / (norm_a * norm_b)

v_tech1 = [0.9, 0.8, 0.1]  # Vector for 'deep learning'
v_tech2 = [0.85, 0.75, 0.15]  # Vector for 'neural networks'
v_food = [0.05, 0.1, 0.95]  # Vector for 'pizza recipe'

print(f"Cosine Similarity (Tech1 vs Tech2): {cosine_similarity(v_tech1, v_tech2):.4f} (High semantic match)")
print(f"Cosine Similarity (Tech1 vs Food):  {cosine_similarity(v_tech1, v_food):.4f} (Near orthogonal)")
```

Expected output:
A and B: 1.0 A and C: 0.2673
2.2.11 Prompt Engineering versus RAG versus PEFT/LoRA
[RESTORED STANDARD THEORY]
These are different strategies for adapting a model to an application.
A. Prompt Engineering
Prompt engineering changes the input instructions without modifying the model's learned parameters.
Example:
You are a university teaching assistant. Explain the concept of tokenization. Use a simple example. Include one mathematical definition. Finish with three viva questions.
Advantages:
Easy to implement.
No model retraining.
Quick to modify.
Suitable for task-specific instructions.
Limitations:
Does not permanently teach new facts to the model.
Prompt length consumes context-window capacity.
Cannot guarantee factual accuracy.
B. Retrieval-Augmented Generation (RAG)
RAG retrieves relevant external information and provides it to a language model as context.
USER QUESTION | v QUERY EMBEDDING | v VECTOR DATABASE | v RETRIEVE TOP-K DOCUMENTS | v CONTEXT + USER QUERY | v LANGUAGE MODEL | v GROUNDED ANSWER
Mathematical representation:
\[ D=\operatorname{Retrieve}(q,\mathcal{K}) \]
\[ y=\operatorname{Generate}(q,D) \]
Where:
\(q\): User query.
\(\mathcal{K}\): Knowledge base.
\(D\): Retrieved documents.
\(y\): Generated response.
C. Parameter-Efficient Fine-Tuning (PEFT)
PEFT adapts a pretrained model by training only a small subset of parameters or adding small trainable modules.
LoRA: Low-Rank Adaptation
Instead of updating a full weight matrix \(W\), LoRA introduces a low-rank update:
\[ W'=W+\Delta W \]
\[ \Delta W=BA \]
Where:
\(A\): Low-rank matrix.
\(B\): Low-rank matrix.
\(r\): Rank, generally much smaller than the original dimensions.
For an original matrix:
\[ W\in\mathbb{R}^{d\times k} \]
LoRA uses:
\[ A\in\mathbb{R}^{r\times k} \]
\[ B\in\mathbb{R}^{d\times r} \]
The number of trainable parameters becomes:
\[ r(k+d) \]
rather than:
\[ dk \]
when \(r\) is sufficiently small.
Comparison
Method
What changes?
Best suited for
Prompt Engineering
Input instructions
Quick task adaptation
RAG
External knowledge supplied at runtime
Current or private information
PEFT / LoRA
Small trainable model parameters
Persistent behavior or domain adaptation
⚠ Examiner's flag: RAG does not normally retrain the model. LoRA does not automatically provide access to current external documents. Prompt engineering does not modify model weights.
EXPERIMENT 2.3: NATURAL LANGUAGE PROCESSING PIPELINES AND AZURE AI LANGUAGE
2.3.1 Aim and objectives
[DIRECTLY IN NOTES]
Aim: To study and implement text analysis using Natural Language Processing, including tokenization, normalization, stopword removal, stemming, lemmatization, POS tagging, named entity recognition, sentiment analysis and semantic text processing.
Objectives:
Convert unstructured text into structured information.
Apply text preprocessing techniques.
Identify grammatical roles using POS tagging.
Extract named entities from text.
Perform sentiment analysis.
Understand Azure AI Language capabilities.
2.3.2 Introduction to NLP
Natural Language Processing is a branch of AI that enables computers to process, analyze and understand human language.
Examples:
Chatbots.
Machine translation.
Spam detection.
Sentiment analysis.
Text summarization.
Entity recognition.
Information extraction.
Document classification.
NLP processing architecture
RAW TEXT INPUT | v TEXT NORMALIZATION | v TOKENIZATION | v STOPWORD REMOVAL | v STEMMING / LEMMA | v POS TAGGING | v NAMED ENTITY RECOGNITION | v FEATURE REPRESENTATION | v NLP MODEL / TEXT ANALYSIS | v STRUCTURED OUTPUT
2.3.3 Text normalization
[DIRECTLY IN NOTES]
Text normalization converts text into a standard format.
Typical operations:
Lowercase conversion.
Removing unnecessary punctuation.
Removing extra whitespace.
Standardizing special characters.
Correcting inconsistent text representations.
Example:
Original:
Artificial Intelligence IS Powerful!!!
Normalized:
artificial intelligence is powerful
Python:
import re text = "Artificial Intelligence IS Powerful!!!" normalized = text.lower() normalized = re.sub(r"[^a-z0-9\s]", "", normalized) normalized = re.sub(r"\s+", " ", normalized).strip() print(normalized)
Output:
artificial intelligence is powerful
Important: Normalization must be selected according to the task. Removing punctuation, case information or numbers can destroy information that may matter for sentiment, named entities, legal documents or financial data.
2.3.4 Tokenization
Tokenization divides a sentence or document into smaller units called tokens.
Example:
Natural Language Processing is interesting.
Word tokens:
Natural Language Processing is interesting .
There are different tokenization approaches:
Type
Description
Sentence tokenization
Splits text into sentences
Word tokenization
Splits sentences into words
Character tokenization
Splits text into characters
Subword tokenization
Splits words into smaller units
Byte tokenization
Represents text as byte-level units
Python using NLTK:
import nltk nltk.download("punkt") nltk.download("punkt_tab") from nltk.tokenize import sent_tokenize, word_tokenize text = "AI is transforming education. NLP helps computers understand language." print("Sentences:") print(sent_tokenize(text)) print("\nWords:") print(word_tokenize(text))
Expected output:
Sentences: ['AI is transforming education.', 'NLP helps computers understand language.'] Words: ['AI', 'is', 'transforming', 'education', '.', 'NLP', 'helps', 'computers', 'understand', 'language', '.']
2.3.5 Stopword removal
[DIRECTLY IN NOTES]
Stopwords are frequently occurring words that may contribute relatively little to a particular text-analysis task.
Examples:
the, is, am, are, a, an, it, of, and, to
Example:
Original:
AI is transforming the world.
After stopword removal:
AI transforming world
Mathematical view
Let the original token set be:
\[ T=\{t_1,t_2,\ldots,t_n\} \]
Let \(S\) be the stopword set.
The filtered set is:
\[ T'=T\setminus S \]
Python:
import nltk nltk.download("stopwords") from nltk.corpus import stopwords from nltk.tokenize import word_tokenize text = "AI is transforming the world of education." stop_words = set(stopwords.words("english")) tokens = word_tokenize(text) filtered = [ word for word in tokens if word.lower() not in stop_words ] print(filtered)
Possible output:
['AI', 'transforming', 'world', 'education', '.']
⚠ Examiner's flag: Stopword removal can be harmful in sentiment analysis. For example, removing the word "not" from "not good" reverses the meaning.
2.3.6 Stemming versus lemmatization
[DIRECTLY IN NOTES]
Both methods reduce words to a base-like form, but they use different approaches.
A. Stemming
Stemming removes or modifies word endings using heuristic rules.
Examples:
Original
Stem
playing
play
played
play
studies
studi
connected
connect
running
run
Stemming may produce a result that is not a valid dictionary word.
Porter stemming
Porter Stemmer is a rule-based stemming algorithm.
from nltk.stem import PorterStemmer stemmer = PorterStemmer() words = ["playing", "played", "studies", "connected", "running"] for word in words: print(word, "->", stemmer.stem(word))
Typical output:
playing -> play played -> play studies -> studi connected -> connect running -> run
B. Lemmatization
Lemmatization converts a word to its dictionary base form, called a lemma.
Examples:
Original
Lemma
running
run
better
good
children
child
studies
study
was
be
Lemmatization uses linguistic information such as vocabulary and grammatical role.
WordNet lemmatization
import nltk nltk.download("wordnet") nltk.download("omw-1.4") from nltk.stem import WordNetLemmatizer lemmatizer = WordNetLemmatizer() words = ["running", "cars", "children", "studies"] for word in words: print(word, "->", lemmatizer.lemmatize(word))
Without POS information, WordNet may not always return the expected verb form.
For example, running may remain running when treated as a noun.
A POS-aware example:
from nltk.stem import WordNetLemmatizer lemmatizer = WordNetLemmatizer() print(lemmatizer.lemmatize("running", pos="v")) print(lemmatizer.lemmatize("better", pos="a")) print(lemmatizer.lemmatize("children", pos="n"))
Output:
run good child
Stemming versus lemmatization
Feature
Stemming
Lemmatization
Method
Rule-based truncation
Vocabulary and linguistic analysis
Speed
Usually faster
Usually slower
Accuracy
Less linguistically precise
Usually more linguistically precise
Valid word guaranteed?
No
Usually
Example
studies → studi
studies → study
2.3.7 Part-of-Speech tagging
[DIRECTLY IN NOTES]
POS tagging identifies the grammatical category of each token.
Common POS categories:
POS
Meaning
Example
NN
Singular noun
student
NNS
Plural noun
students
VB
Base verb
study
VBD
Past-tense verb
studied
JJ
Adjective
intelligent
RB
Adverb
quickly
PRP
Personal pronoun
he
IN
Preposition
in
Example:
The intelligent student studies carefully.
Possible tags:
The DT intelligent JJ student NN studies VBZ carefully RB
NLTK POS tagging
import nltk nltk.download("punkt") nltk.download("punkt_tab") nltk.download("averaged_perceptron_tagger_eng") from nltk.tokenize import word_tokenize text = "The intelligent student studies carefully." tokens = word_tokenize(text) tags = nltk.pos_tag(tokens) for word, tag in tags: print(f"{word:15} {tag}")
2.3.8 Named Entity Recognition (NER)
[DIRECTLY IN NOTES]
NER identifies important named entities in text.
Typical entity types:
Entity
Meaning
Example
PERSON
Person name
A. P. J. Abdul Kalam
ORG
Organization
Microsoft
GPE
Country, city or geopolitical entity
India
DATE
Date
21 November 2026
MONEY
Monetary value
₹5,000
TIME
Time expression
10:30 AM
LOC
Location
Himalayas
Example text:
Microsoft was founded by Bill Gates and Paul Allen.
Possible NER output:
Microsoft ORG Bill Gates PERSON Paul Allen PERSON
NER using spaCy
import spacy nlp = spacy.load("en_core_web_sm") text = """ Microsoft was founded by Bill Gates and Paul Allen. The company operates in the United States. """ doc = nlp(text) for entity in doc.ents: print(entity.text, "->", entity.label_)
Install spaCy model:
python -m pip install spacy python -m spacy download en_core_web_sm
2.3.9 Full NLP pipeline using NLTK and spaCy
Complete practical script
[RESTORED STANDARD CODE BASED ON DIRECT COURSE TOPICS]
This program demonstrates:
Text normalization.
Sentence tokenization.
Word tokenization.
Stopword removal.
Porter stemming.
WordNet lemmatization.
POS tagging.
NER using spaCy.
Word-frequency analysis.
TF-IDF feature extraction.
Installation
python -m pip install nltk spacy scikit-learn pandas python -m spacy download en_core_web_sm
Complete executable script:

Save as `nlp_pipeline.py`.

```python
import re
import nltk
import spacy
import pandas as pd
from collections import Counter
from nltk.tokenize import sent_tokenize, word_tokenize
from nltk.corpus import stopwords
from nltk.stem import PorterStemmer, WordNetLemmatizer
from sklearn.feature_extraction.text import TfidfVectorizer

# 1. Download required NLTK resources
for res in ["punkt", "punkt_tab", "stopwords", "wordnet", "omw-1.4", "averaged_perceptron_tagger_eng"]:
    nltk.download(res, quiet=True)

# 2. Load spaCy model
try:
    nlp = spacy.load("en_core_web_sm")
except OSError:
    import sys
    sys.exit("spaCy model missing. Run: python -m spacy download en_core_web_sm")

# 3. Sample Corpus
documents = [
    "Artificial Intelligence and Machine Learning are transforming modern higher education.",
    "Natural Language Processing enables computers to understand, parse, and generate human language.",
    "Deep neural networks, Large Language Models, and Generative AI synthesize text, code, and images."
]
corpus_text = " ".join(documents)

# 4. Text Normalization
def normalize(text):
    text = text.lower()
    text = re.sub(r"[^a-z0-9\s]", " ", text)
    text = re.sub(r"\s+", " ", text).strip()
    return text

normalized_text = normalize(corpus_text)
print("1. NORMALIZED CORPUS:")
print(normalized_text)

# 5. Tokenization
sentences = sent_tokenize(corpus_text)
words = word_tokenize(normalized_text)
print(f"\n2. SENTENCES: {len(sentences)} detected")
print(f"3. WORD TOKENS: {len(words)} tokens")

# 6. Stopwords & Lemmatization
stop_words = set(stopwords.words("english"))
clean_tokens = [w for w in words if w not in stop_words and w.isalnum()]

stemmer = PorterStemmer()
lemmatizer = WordNetLemmatizer()

nlp_table = []
for w in clean_tokens[:10]:
    nlp_table.append({
        "Token": w,
        "Stem (Porter)": stemmer.stem(w),
        "Lemma (WordNet)": lemmatizer.lemmatize(w)
    })
print("\n4. STEMMING & LEMMATIZATION TABLE:")
print(pd.DataFrame(nlp_table).to_string(index=False))

# 7. POS Tagging
pos_tags = nltk.pos_tag(clean_tokens[:12])
print("\n5. PART-OF-SPEECH (POS) TAGS:")
for word, tag in pos_tags:
    print(f"   {word:20} -> {tag}")

# 8. Named Entity Recognition with spaCy
print("\n6. NAMED ENTITY RECOGNITION:")
for doc_text in documents:
    doc = nlp(doc_text)
    for ent in doc.ents:
        print(f"   {ent.text:25} -> {ent.label_:15} ({spacy.explain(ent.label_)})")

# 9. TF-IDF Representation
vectorizer = TfidfVectorizer(stop_words="english")
tfidf_matrix = vectorizer.fit_transform(documents)
print(f"\n7. TF-IDF MATRIX SHAPE: {tfidf_matrix.shape}")
```

Expected output structure
1. NORMALIZED TEXT artificial intelligence is transforming education ... 2. SENTENCES 1 Artificial Intelligence is transforming education. 2 Machine learning helps computers learn from data. ... 3. WORD TOKENS ['artificial', 'intelligence', 'is', ...] 4. STOPWORD-FREE TOKENS ['artificial', 'intelligence', 'transforming', ...] 5. STEMMED WORDS ['artifici', 'intellig', 'transform', ...] 6. LEMMATIZED WORDS ['artificial', 'intelligence', 'transforming', ...] 7. POS TAGGING artificial JJ intelligence NN ... 8. NAMED ENTITY RECOGNITION Microsoft ORG ... ... 9. TOP WORD FREQUENCIES Word Frequency ... 10. TF-IDF MATRIX ... TF-IDF SHAPE: (3, ...) NLP PIPELINE COMPLETED SUCCESSFULLY.
The exact POS tags, NER labels, vocabulary order and numerical TF-IDF values depend on the installed model and library versions.
2.3.10 TF-IDF mathematical foundation
[DIRECTLY IN NOTES: TF-IDF; RESTORED MATHEMATICS]
TF-IDF stands for Term Frequency-Inverse Document Frequency.
It assigns a weight to a term based on its frequency in a document and its rarity across the entire document collection.
Term Frequency
A basic term-frequency definition is:
\[ TF(t,d)= \frac{f_{t,d}}{\sum_{k}f_{k,d}} \]
Where:
\(f_{t,d}\): Frequency of term \(t\) in document \(d\).
Denominator: Total term occurrences in the document.
Inverse Document Frequency
A common smoothed definition is:
\[ IDF(t)= \log\left( \frac{N+1}{DF(t)+1} \right)+1 \]
Where:
\(N\): Total number of documents.
\(DF(t)\): Number of documents containing term \(t\).
TF-IDF
\[ \boxed{TFIDF(t,d)=TF(t,d)\times IDF(t)} \]
Interpretation:
A frequent word in one document can receive a higher TF.
A word appearing in nearly every document receives a lower IDF.
A distinctive word can receive a higher overall TF-IDF weight.
Example: The word "the" often has low discriminative value because it occurs in many documents. A technical word such as "transformer" may be more useful for identifying a document's subject.
2.3.11 Sentiment analysis
[DIRECTLY IN NOTES: SENTIMENT ANALYSIS; RESTORED IMPLEMENTATIONS]
Sentiment analysis identifies the emotional polarity of a text.
Common labels:
Positive.
Negative.
Neutral.
Example:
Text
Expected sentiment
The product is excellent.
Positive
The service was terrible.
Negative
The package arrived today.
Neutral
A. VADER sentiment analysis
VADER is a lexicon and rule-based sentiment analysis tool, commonly used for social-media-style English text.
Install:
python -m pip install vaderSentiment
Code:
from vaderSentiment.vaderSentiment import SentimentIntensityAnalyzer analyzer = SentimentIntensityAnalyzer() sentences = [ "This product is absolutely amazing!", "The service was terrible and disappointing.", "The package arrived today." ] for sentence in sentences: scores = analyzer.polarity_scores(sentence) compound = scores["compound"] if compound >= 0.05: sentiment = "Positive" elif compound <= -0.05: sentiment = "Negative" else: sentiment = "Neutral" print("\nText:", sentence) print("Scores:", scores) print("Sentiment:", sentiment)
VADER returns:
pos: Positive proportion.
neg: Negative proportion.
neu: Neutral proportion.
compound: Combined normalized sentiment score.
B. TextBlob sentiment
Install:
python -m pip install textblob
Code:
from textblob import TextBlob sentences = [ "I love this application.", "This software is extremely frustrating.", "The application was released yesterday." ] for sentence in sentences: result = TextBlob(sentence).sentiment print("\nText:", sentence) print("Polarity:", round(result.polarity, 3)) print("Subjectivity:", round(result.subjectivity, 3))
Polarity generally ranges from -1 to +1.
Subjectivity generally ranges from 0 to 1.
C. Scikit-Learn sentiment classification
This approach trains a model using labeled examples.
from sklearn.pipeline import Pipeline from sklearn.feature_extraction.text import TfidfVectorizer from sklearn.linear_model import LogisticRegression texts = [ "I love this product", "This is an excellent service", "The application is wonderful", "I hate this product", "This service is terrible", "The application is disappointing", "The package arrived today", "The product is available now", "The service starts tomorrow" ] labels = [ "positive", "positive", "positive", "negative", "negative", "negative", "neutral", "neutral", "neutral" ] model = Pipeline([ ("tfidf", TfidfVectorizer()), ("classifier", LogisticRegression(max_iter=1000)) ]) model.fit(texts, labels) test_sentences = [ "The product is wonderful", "The service is terrible", "The package arrived" ] predictions = model.predict(test_sentences) for text, prediction in zip(test_sentences, predictions): print(text, "->", prediction)
Expected output:
The product is wonderful -> positive The service is terrible -> negative The package arrived -> neutral
The dataset is intentionally small for demonstration. It is not sufficient for a reliable real-world sentiment system.
2.3.12 Azure AI Language Studio and Text Analytics
[DIRECTLY IN NOTES: AZURE AI TOOLS; RESTORED STANDARD WORKFLOW]
Azure AI Language provides language-processing capabilities through managed services and APIs.
Important operations include:
Capability
Purpose
Sentiment analysis
Identify positive, negative or neutral sentiment
Key phrase extraction
Extract important phrases
Named entity recognition
Identify people, organizations and places
Entity linking
Link recognized entities to known knowledge sources
PII detection
Detect personal information
Language detection
Identify the language
Summarization
Produce shorter versions of documents
Azure AI Language workflow
INPUT DOCUMENT | v AZURE AI LANGUAGE | +--------------+--------------+ | | | v v v Sentiment Key Phrase NER Analysis Extraction | | | | +--------------+--------------+ | v PII DETECTION | v STRUCTURED JSON OUTPUT | v APPLICATION / DATABASE
Azure AI Language Studio practical workflow
Open the Azure portal.
Create an Azure AI Language resource.
Note the resource endpoint and key.
Open the supported Language Studio experience.
Select a text-analysis feature.
Enter sample text.
Run the analysis.
Inspect the structured result.
Integrate the operation into a Python or application workflow.
Python example: Azure AI Language Text Analytics
Install the SDK:
python -m pip install azure-ai-textanalytics azure-core
Configure environment variables.
macOS / Linux:
export AZURE_LANGUAGE_ENDPOINT="https://YOUR-RESOURCE.cognitiveservices.azure.com/" export AZURE_LANGUAGE_KEY="YOUR-RESOURCE-KEY"
Windows PowerShell:
$env:AZURE_LANGUAGE_ENDPOINT="https://YOUR-RESOURCE.cognitiveservices.azure.com/" $env:AZURE_LANGUAGE_KEY="YOUR-RESOURCE-KEY"
Complete script:
import os from azure.core.credentials import AzureKeyCredential from azure.ai.textanalytics import TextAnalyticsClient endpoint = os.environ.get("AZURE_LANGUAGE_ENDPOINT") key = os.environ.get("AZURE_LANGUAGE_KEY") if not endpoint or not key: raise SystemExit( "Set AZURE_LANGUAGE_ENDPOINT and AZURE_LANGUAGE_KEY first." ) client = TextAnalyticsClient( endpoint=endpoint, credential=AzureKeyCredential(key) ) documents = [ "Microsoft is developing AI tools in the United States.", "The customer service was excellent and very helpful." ] # ----------------------------------------- # 1. KEY PHRASE EXTRACTION # ----------------------------------------- print("\nKEY PHRASES") phrase_results = client.extract_key_phrases(documents) for result in phrase_results: if result.is_error: print("Error:", result.error) else: print(result.key_phrases) # ----------------------------------------- # 2. NAMED ENTITY RECOGNITION # ----------------------------------------- print("\nNAMED ENTITIES") entity_results = client.recognize_entities(documents) for result in entity_results: if result.is_error: print("Error:", result.error) else: for entity in result.entities: print( entity.text, "->", entity.category, "->", entity.confidence_score ) # ----------------------------------------- # 3. SENTIMENT ANALYSIS # ----------------------------------------- print("\nSENTIMENT ANALYSIS") sentiment_results = client.analyze_sentiment( documents, show_opinion_mining=True ) for result in sentiment_results: if result.is_error: print("Error:", result.error) else: print("Sentiment:", result.sentiment) print("Positive:", result.confidence_scores.positive) print("Neutral:", result.confidence_scores.neutral) print("Negative:", result.confidence_scores.negative) # ----------------------------------------- # 4. PII DETECTION # ----------------------------------------- print("\nPII DETECTION") pii_documents = [ "Contact John at john@example.com or call 555-123-4567." ] pii_results = client.recognize_pii_entities(pii_documents) for result in pii_results: if result.is_error: print("Error:", result.error) else: print("Redacted text:", result.redacted_text) for entity in result.entities: print( entity.text, "->", entity.category ) print("\nAZURE AI LANGUAGE TASKS COMPLETED.")
Expected output structure:
KEY PHRASES ['Microsoft', 'AI tools', 'United States'] ['customer service'] NAMED ENTITIES Microsoft -> Organization -> 0.xxx United States -> Location -> 0.xxx ... SENTIMENT ANALYSIS Sentiment: neutral Positive: ... Neutral: ... Negative: ... PII DETECTION Redacted text: Contact *************** or call ************ john@example.com -> Email 555-123-4567 -> PhoneNumber AZURE AI LANGUAGE TASKS COMPLETED.
The exact entities, scores, categories and redaction format are service-generated and can change with the deployed API version and language resource configuration.
Security note
Never place Azure keys directly into source code or commit them to GitHub. Use environment variables, a secret manager or managed identity. PII detection and redaction should be tested before processing real personal data.
2.3.13 Examiner's flags
Tokenization and normalization are different operations.
Stopword removal is task-dependent.
Stemming may produce invalid dictionary words.
Lemmatization uses linguistic information.
POS tagging identifies grammatical roles, not named entities.
NER detects entity mentions, not necessarily their complete real-world identity.
TF-IDF is a statistical feature representation, not a contextual embedding.
VADER is rule-based, whereas Logistic Regression is a trained classifier.
A sentiment model can fail on sarcasm and context-dependent expressions.
PII detection is not a substitute for a complete privacy and security program.
EXPERIMENT 2.4: GENERATIVE AI ON AZURE AND PROMPT ENGINEERING
2.4.1 Aim
[RESTORED STANDARD LAB SUPPORT]
To understand Generative AI workflows, prompt engineering, Azure OpenAI model deployment, Prompt Flow orchestration, output evaluation, token management and cost optimization.
The repository's Experiment 2.4 study-package file is a placeholder rather than a full technical lab manual. The following material therefore supplies the standard practical implementation needed to complete the experiment.
2.4.2 Azure OpenAI Studio and Azure AI Foundry
Azure AI Foundry is Microsoft's platform for building, evaluating and managing generative AI applications and agents.
The Azure portal and Foundry experiences may evolve over time. The names and exact locations of individual interface controls can differ by product version.
Typical workflow
AZURE PORTAL | v AI FOUNDRY PROJECT | v MODEL CATALOG | v SELECT FOUNDATION MODEL | v CREATE DEPLOYMENT | v OBTAIN ENDPOINT AND ACCESS | v BUILD APPLICATION | +---------+---------+ | | v v PROMPT DESIGN DATA / RAG | | +---------+---------+ | v MODEL INFERENCE | v EVALUATION AND TESTING | v DEPLOY APPLICATION
Common workflow steps
Sign in to the Azure portal.
Create or select the appropriate Azure AI Foundry resource/project.
Select an available foundation model.
Deploy the model, subject to regional availability and quota.
Obtain the deployment name, endpoint and authentication configuration.
Build an application using the supported SDK.
Test prompts and output formats.
Evaluate quality, cost, latency and safety.
Deploy the application with appropriate access controls.
2.4.3 Prompt engineering
[DIRECTLY IN NOTES + RESTORED STANDARD THEORY]
A prompt is the instruction or input provided to a language model.
A prompt can include:
Role or system instructions.
User request.
Context.
Examples.
Output constraints.
Formatting requirements.
A. System instructions
System instructions establish the model's intended role, behavior and constraints.
Example:
You are a university-level computer science tutor. Explain technical concepts accurately. Use clear mathematical notation. Do not invent experimental results. If a fact is uncertain, state the uncertainty.
B. User instructions
The user instruction specifies the current task.
Example:
Explain the difference between RNNs and Transformers. Include a comparison table and one practical example.
C. Few-shot prompting
Few-shot prompting provides examples to guide the model's output.
Example:
Classify the sentiment. Example 1: Text: "This product is excellent." Label: Positive Example 2: Text: "The product is terrible." Label: Negative Now classify: Text: "The product is acceptable." Label:
D. In-context learning
In-context learning is the model's ability to adapt its output based on examples and instructions in the current prompt, without updating its model weights.
E. Zero-shot prompting
Zero-shot prompting asks the model to perform a task without providing examples.
Example:
Classify the sentiment of this sentence: "The application is extremely useful."
Prompting comparison
Method
Examples supplied?
Typical use
Zero-shot
No
General instructions
One-shot
One
Demonstrate expected format
Few-shot
A few
Guide task behavior
In-context learning
Depends on prompt
Adapt behavior from supplied context
2.4.4 Temperature and Top-p sampling
[RESTORED STANDARD THEORY]
Language models generate output using a probability distribution over possible next tokens.
Suppose the model produces logits:
\[ z_1,z_2,\ldots,z_n \]
Temperature
Temperature modifies the distribution:
\[ P_i= \frac{\exp(z_i/T)} {\sum_j\exp(z_j/T)} \]
Where \(T\) is temperature.
General behavior:
Temperature
Typical effect
Near 0
More deterministic, higher-probability choices
0.3
Lower variation
0.7
Moderate variation
1.0
Original distribution scale
Above 1
Flatter distribution and more variation
A low temperature does not guarantee factual correctness. It only changes sampling behavior.
Top-p sampling
Top-p, also called nucleus sampling, selects from the smallest set of candidate tokens whose cumulative probability reaches a threshold \(p\).
Suppose the sorted probabilities are:
Token
Probability
Cumulative probability
A
0.50
0.50
B
0.25
0.75
C
0.15
0.90
D
0.07
0.97
E
0.03
1.00
For:
\[ p=0.90 \]
The candidate nucleus includes A, B and C.
Temperature versus Top-p
Temperature reshapes the probability distribution.
Top-p truncates the candidate token set.
Both affect output diversity.
They do not replace good prompt design or factual verification.
⚠ Examiner's flag: A higher temperature does not make a model more intelligent. It generally increases variation in sampling.
2.4.5 Prompt Flow and DAG architecture
[RESTORED STANDARD AZURE LAB THEORY]
Prompt Flow is used to build and evaluate workflows involving prompts, Python code, model calls and data connections.
A DAG is a Directed Acyclic Graph.
Directed: Connections have direction.
Acyclic: The graph contains no directed cycles.
Graph: It contains nodes and edges.
Example LLM workflow
USER QUESTION | v INPUT VALIDATION | v QUERY CLEANING | v DOCUMENT SEARCH | v CONTEXT PREPARATION | v LLM GENERATION | v OUTPUT VALIDATION | v FINAL RESPONSE
Each node performs a specific operation.
Evaluation metrics
Metric
Purpose
Groundedness
Whether the response is supported by supplied evidence
Relevance
Whether the answer addresses the user's question
Coherence
Whether the response is logically organized
Fluency
Whether the language is readable
Correctness
Whether the answer is factually correct
Safety
Whether the response avoids prohibited or harmful output
Groundedness
A grounded response is supported by retrieved or supplied evidence.
Example:
Context:
The university library opens at 8 AM.
Question:
When does the library open?
Grounded answer:
The library opens at 8 AM.
Ungrounded answer:
The library opens at 9 AM.
Relevance
An answer is relevant when it addresses the user's actual question rather than providing unrelated information.
Coherence
A coherent answer is logically structured and does not contradict itself.
Important: Automated evaluation metrics are indicators, not absolute proof that a response is correct or safe. High-stakes applications require additional validation.
2.4.6 Complete Azure OpenAI Python SDK implementation
Complete practical script
[RESTORED STANDARD CODE]
The following example uses the official OpenAI Python SDK configured for an Azure OpenAI endpoint.
The exact endpoint and authentication method depend on the Azure deployment and API configuration. This example uses API-key authentication and the chat-completions interface.
Installation
python -m pip install --upgrade openai
Configure environment variables
macOS / Linux:
export AZURE_OPENAI_ENDPOINT="https://YOUR-RESOURCE.openai.azure.com/" export AZURE_OPENAI_API_KEY="YOUR-API-KEY" export AZURE_OPENAI_DEPLOYMENT="YOUR-DEPLOYMENT-NAME" export AZURE_OPENAI_API_VERSION="YOUR-SUPPORTED-API-VERSION"
Windows PowerShell:
$env:AZURE_OPENAI_ENDPOINT="https://YOUR-RESOURCE.openai.azure.com/" $env:AZURE_OPENAI_API_KEY="YOUR-API-KEY" $env:AZURE_OPENAI_DEPLOYMENT="YOUR-DEPLOYMENT-NAME" $env:AZURE_OPENAI_API_VERSION="YOUR-SUPPORTED-API-VERSION"
Complete code: Chat completion with system instructions

Save as `azure_openai_chat.py`.

```python
import os
import json
from openai import AzureOpenAI

# 1. Read Azure OpenAI Environment Variables
endpoint = os.getenv("AZURE_OPENAI_ENDPOINT")
api_key = os.getenv("AZURE_OPENAI_API_KEY")
deployment = os.getenv("AZURE_OPENAI_DEPLOYMENT", "gpt-4o")
api_version = os.getenv("AZURE_OPENAI_API_VERSION", "2024-02-15-preview")

if not endpoint or not api_key:
    print("Azure OpenAI credentials not set. Showing implementation template.")
    print("To execute, configure AZURE_OPENAI_ENDPOINT and AZURE_OPENAI_API_KEY.")
else:
    client = AzureOpenAI(
        azure_endpoint=endpoint,
        api_key=api_key,
        api_version=api_version
    )

    system_prompt = """
    You are an expert AI professor. Explain technical concepts with rigor,
    clear mathematical definitions, and practical engineering examples.
    """

    user_prompt = """
    Explain the difference between Self-Attention and Cross-Attention in Transformers.
    """

    response = client.chat.completions.create(
        model=deployment,
        messages=[
            {"role": "system", "content": system_prompt},
            {"role": "user", "content": user_prompt}
        ],
        temperature=0.3,
        max_tokens=600
    )

    print("AZURE OPENAI RESPONSE:")
    print(response.choices[0].message.content)

    if response.usage:
        print(f"\nTOKEN USAGE: Prompt={response.usage.prompt_tokens}, Completion={response.usage.completion_tokens}, Total={response.usage.total_tokens}")
```

Expected output
The model should return an explanation containing:
A definition of Machine Learning.
A definition of Deep Learning.
Three differences.
A real-world example.
The exact wording is generated dynamically.
The token usage section should display the prompt, completion and total token counts when returned by the service.
2.4.7 JSON mode implementation
JSON mode requests that the model return valid JSON rather than ordinary free-form prose.
Important: JSON mode ensures JSON formatting when supported by the deployment, but it does not guarantee that the returned JSON conforms to every application-specific schema. Validate the result in Python.
Save as azure_openai_json.py.
import os import json from openai import AzureOpenAI endpoint = os.getenv("AZURE_OPENAI_ENDPOINT") api_key = os.getenv("AZURE_OPENAI_API_KEY") deployment = os.getenv("AZURE_OPENAI_DEPLOYMENT") api_version = os.getenv("AZURE_OPENAI_API_VERSION") if not all([endpoint, api_key, deployment, api_version]): raise SystemExit("Azure OpenAI configuration is incomplete.") client = AzureOpenAI( azure_endpoint=endpoint, api_key=api_key, api_version=api_version ) response = client.chat.completions.create( model=deployment, messages=[ { "role": "system", "content": ( "You classify text sentiment. " "Return a JSON object with keys " "sentiment, confidence, and explanation. " "The sentiment must be positive, negative, " "or neutral. Confidence must be a number " "between 0 and 1." ) }, { "role": "user", "content": ( "Analyze this sentence: " "'The application is useful and easy to operate.'" ) } ], response_format={ "type": "json_object" }, temperature=0.1, max_tokens=200 ) content = response.choices[0].message.content try: result = json.loads(content) except json.JSONDecodeError: raise SystemExit("The model did not return valid JSON.") # Validate required fields required_fields = { "sentiment", "confidence", "explanation" } if not required_fields.issubset(result): raise SystemExit("JSON response is missing required fields.") if result["sentiment"] not in { "positive", "negative", "neutral" }: raise SystemExit("Invalid sentiment value.") confidence = result["confidence"] if not isinstance(confidence, (int, float)): raise SystemExit("Confidence must be numeric.") if not 0 <= confidence <= 1: raise SystemExit("Confidence must be between 0 and 1.") print("\nVALIDATED JSON RESPONSE") print(json.dumps(result, indent=4))
Expected output format:
{ "sentiment": "positive", "confidence": 0.95, "explanation": "The sentence expresses a favorable opinion." }
The confidence value and explanation are model-generated. They should not be treated as calibrated statistical probabilities unless the application has separately validated their calibration.
2.4.8 Token management and context windows
[RESTORED STANDARD THEORY]
A token is a unit of text processed by a language model.
A token may represent:
A complete word.
Part of a word.
Punctuation.
A whitespace-associated text fragment.
A byte-level unit.
Token count is not equal to word count.
Context-window budget
A simplified context budget is:
\[ T_{\text{input}}+T_{\text{output}} \leq T_{\text{context}} \]
Where:
\(T_{\text{input}}\): Input tokens.
\(T_{\text{output}}\): Generated tokens.
\(T_{\text{context}}\): Available context capacity.
For an application that includes system instructions, user input and retrieved documents:
\[ T_{\text{system}}+ T_{\text{user}}+ T_{\text{retrieved}}+ T_{\text{output}} \leq T_{\text{context}} \]
A safe implementation reserves space for the generated response and service overhead.
Example
Suppose the application has a hypothetical context capacity of 16,000 tokens.
Component
Tokens
System instructions
500
User request
1,000
Retrieved documents
8,000
Output reserve
2,000
Remaining margin
4,500
This is only an illustrative budget. Actual model limits and API accounting depend on the deployed model and service configuration.
2.4.9 Cost management
For a simple token-based pricing model:
\[ C= \frac{T_{\text{in}}}{10^6}R_{\text{in}} + \frac{T_{\text{out}}}{10^6}R_{\text{out}} \]
Where:
\(T_{\text{in}}\): Input token count.
\(T_{\text{out}}\): Output token count.
\(R_{\text{in}}\): Input price per million tokens.
\(R_{\text{out}}\): Output price per million tokens.
Actual Azure pricing varies by model, deployment type, region and service configuration. Some services also have additional charges.
Example calculation
Assume, only for illustration:
Input tokens = 10,000.
Output tokens = 2,000.
Input rate = $2 per million tokens.
Output rate = $8 per million tokens.
Input cost:
\[ C_{\text{in}}= \frac{10,000}{1,000,000}\times2 \]
\[ C_{\text{in}}=\$0.02 \]
Output cost:
\[ C_{\text{out}}= \frac{2,000}{1,000,000}\times8 \]
\[ C_{\text{out}}=\$0.016 \]
Total:
\[ \boxed{C=\$0.036} \]
These are hypothetical rates, not current Azure prices.
Cost optimization techniques
Use a smaller model for simpler tasks.
Limit unnecessary output length.
Avoid repeatedly sending large instructions.
Retrieve only relevant documents in RAG.
Cache repeated responses where appropriate.
Use batch processing when supported.
Monitor actual input and output token usage.
Set quotas and application-level spending limits.
2.4.10 Latency management
Latency is the time taken to receive a response.
A simplified breakdown is:
\[ T_{\text{total}}= T_{\text{network}}+ T_{\text{queue}}+ T_{\text{processing}}+ T_{\text{generation}} \]
Important factors:
Model size.
Input token count.
Output token count.
Network conditions.
Service load.
Deployment capacity.
Tool execution.
Retrieval time.
Practical optimization
Technique
Expected benefit
Shorter prompts
Less input processing
Smaller model
Often lower inference latency
Streaming output
Faster perceived response
Parallel independent calls
Lower total wall-clock time
Caching
Avoid repeated model calls
Efficient retrieval
Reduce RAG overhead
Output token limit
Control generation duration
⚠ Examiner's flag: Streaming improves perceived responsiveness, but it does not necessarily reduce the total time required to generate the complete response.
2.4.11 Examiner's flags
A prompt is not the same as model fine-tuning.
Few-shot prompting provides examples inside the input context.
In-context learning does not require weight updates.
Temperature changes sampling behavior, not factual knowledge.
Top-p uses cumulative probability to select a candidate nucleus.
JSON mode does not guarantee application-level schema correctness.
Prompt Flow represents connected workflow operations.
Groundedness, relevance and coherence measure different qualities.
Context windows are measured in tokens, not words.
Model pricing and quotas must be checked for the actual Azure deployment.
UNIT 2 MASTER VIVA VOCE AND EXAMINER CHECKLIST
2.5.1 Ten high-yield viva questions with model answers
Q1. Differentiate Artificial Intelligence, Machine Learning and Deep Learning.
Model answer:
Artificial Intelligence is the broad field of creating intelligent systems. Machine Learning is a subset of AI in which systems learn patterns from data. Deep Learning is a subset of Machine Learning that uses neural networks with multiple layers.
Examiner follow-up: Is every AI system based on Machine Learning?
Answer: No. Rule-based expert systems are examples of AI that can operate without learning from data.
Q2. What is the difference between generative and discriminative models?
Model answer:
A discriminative model learns the conditional probability \(P(Y\mid X)\), while a generative model learns a data distribution such as \(P(X,Y)\) or \(P(X)\).
A discriminative model predicts a class, whereas a generative model can learn to generate new samples.
Examiner follow-up: Is Logistic Regression generative or discriminative?
Answer: Discriminative.
Q3. Why is quantization used in LLMs?
Model answer:
Quantization reduces the numerical precision used to represent model parameters. It reduces parameter memory requirements and can improve inference efficiency, depending on hardware and implementation.
Examiner follow-up: How much raw parameter memory does a 7-billion-parameter model require in INT8?
Answer:
\[ 7\times10^9\times1 =7\times10^9\text{ bytes} \]
Approximately 7 GB in decimal units, excluding runtime overhead.
Q4. Explain the four pillars of an AI agent.
Model answer:
Perception receives information from the environment.
Planning determines the steps required to achieve the goal.
Memory stores relevant information.
Action executes operations using tools, APIs or other external systems.
Examiner follow-up: What is the difference between an AI chatbot and an AI agent?
Answer: A basic chatbot mainly responds to messages. An agent can additionally plan and execute actions using tools and observe the results.
Q5. Why do Transformers use attention?
Model answer:
Attention enables the model to calculate relationships between tokens and assign different weights to relevant tokens. This helps the model capture contextual dependencies.
Examiner follow-up: What is the purpose of the scaling factor in scaled dot-product attention?
Answer: It controls the magnitude of dot-product scores, helping prevent softmax saturation and stabilizing gradients.
Q6. Differentiate BPE, WordPiece and SentencePiece.
Model answer:
BPE repeatedly merges frequent adjacent token pairs.
WordPiece learns a subword vocabulary using a scoring criterion.
SentencePiece is a tokenizer framework that can implement BPE or Unigram tokenization directly on raw text.
Examiner follow-up: Which algorithm is associated with BERT?
Answer: WordPiece is commonly associated with BERT.
Q7. What is the difference between stemming and lemmatization?
Model answer:
Stemming reduces words using heuristic rules and may produce invalid words. Lemmatization uses vocabulary and grammatical information to find a valid dictionary base form.
Examiner follow-up: Give an example.
Answer:
Stemming: studies → studi
Lemmatization: studies → study
Q8. What is TF-IDF?
Model answer:
TF-IDF measures the importance of a term in a document relative to a collection of documents.
\[ TFIDF(t,d)=TF(t,d)\times IDF(t) \]
It is used to convert text into numerical features for text analysis and traditional machine-learning models.
Examiner follow-up: Why does a common word usually receive a lower IDF?
Answer: Because it appears in many documents and therefore has less power to distinguish one document from another.
Q9. What is Retrieval-Augmented Generation?
Model answer:
RAG combines information retrieval with language generation. The system retrieves relevant external documents and provides them as context to the language model before generating an answer.
Examiner follow-up: Does RAG retrain the language model?
Answer: Normally, no. RAG retrieves information at inference time without updating the model's parameters.
Q10. Explain temperature and Top-p sampling.
Model answer:
Temperature modifies the probability distribution over possible next tokens. Lower temperature generally produces less varied output, while higher temperature produces more varied output.
Top-p sampling selects a candidate set of tokens whose cumulative probability reaches a specified threshold.
Examiner follow-up: Does temperature zero guarantee a correct answer?
Answer: No. It may make output more deterministic, but it cannot guarantee factual accuracy.
2.5.2 Practical debugging checklist
Problem
Likely cause
Solution
Context window overflow
Input and output token budget exceeds the model limit
Reduce prompt size, retrieve fewer documents, shorten output
Hallucinated answer
Missing or insufficient evidence
Use RAG, citations and verification
Temperature runaway
Excessively varied output
Lower temperature and constrain the task
Embedding dimensionality mismatch
Query and document vectors have different dimensions
Use the same embedding model and version
Poor retrieval quality
Inappropriate chunk size or embedding model
Tune chunking, overlap and retrieval settings
NLTK resource error
Missing tokenizer or corpus data
Run the required nltk.download() commands
spaCy model not found
English language model not installed
Run python -m spacy download en_core_web_sm
Incorrect stemming result
Stemmer uses heuristic rules
Use lemmatization when linguistic accuracy matters
Incorrect sentiment
Negation, sarcasm or context is not captured
Use contextual models and evaluate on representative data
Azure authentication failure
Incorrect key, endpoint or environment variable
Verify resource configuration and credentials
Azure deployment not found
Wrong deployment name
Use the deployment name, not necessarily the model family name
Unsupported API version
API version incompatible with the deployment
Use a supported version for the configured service
JSON parsing error
Model returned invalid or incomplete JSON
Use supported JSON mode and validate with json.loads()
Slow generation
Large model, prompt or output
Reduce token count, stream responses, optimize retrieval
High API cost
Excessive input/output tokens or repeated calls
Track usage, cache and select suitable models
2.5.3 Unit 2 quick revision formula sheet
Probability and machine learning
Concept
Formula
Conditional probability
\(P(A\mid B)=\frac{P(A\cap B)}{P(B)}\)
Bayes' theorem
\(P(A\mid B)=\frac{P(B\mid A)P(A)}{P(B)}\)
Joint probability
\(P(X,Y)=P(X\mid Y)P(Y)\)
Discriminative probability
\(P(Y\mid X)\)
Logistic sigmoid
\(\sigma(z)=\frac{1}{1+e^{-z}}\)
Neural layer
\(a^{(l)}=\sigma(W^{(l)}a^{(l-1)}+b^{(l)})\)
Model memory
\[ \boxed{M=P\times B} \]
Format
Approximate bytes per parameter
FP32
4
FP16
2
INT8
1
INT4
0.5
Transformer equations
Sinusoidal positional encoding:
\[ PE(pos,2i)= \sin\left(\frac{pos}{10000^{2i/d_{\text{model}}}}\right) \]
\[ PE(pos,2i+1)= \cos\left(\frac{pos}{10000^{2i/d_{\text{model}}}}\right) \]
Scaled dot-product attention:
\[ \boxed{ Attention(Q,K,V)= softmax\left(\frac{QK^T}{\sqrt{d_k}}\right)V } \]
Multi-head attention:
\[ MultiHead(Q,K,V)= Concat(head_1,\ldots,head_h)W^O \]
Embeddings
Cosine similarity:
\[ \boxed{ cos(A,B)= \frac{A\cdot B}{\|A\|\|B\|} } \]
GloVe objective:
\[ J=\sum_{i,j}f(X_{ij}) \left( w_i^T\tilde{w}_j+b_i+\tilde{b}_j-\log X_{ij} \right)^2 \]
LoRA update:
\[ W'=W+BA \]
NLP
TF-IDF:
\[ TFIDF(t,d)=TF(t,d)\times IDF(t) \]
Smoothed IDF:
\[ IDF(t)= \log\left(\frac{N+1}{DF(t)+1}\right)+1 \]
Generative AI
Temperature-adjusted probability:
\[ P_i= \frac{e^{z_i/T}}{\sum_j e^{z_j/T}} \]
Token budget:
\[ T_{\text{input}}+T_{\text{output}} \leq T_{\text{context}} \]
Estimated token cost:
\[ C= \frac{T_{\text{in}}R_{\text{in}}}{10^6} + \frac{T_{\text{out}}R_{\text{out}}}{10^6} \]
2.5.4 Final Unit 2 examiner checklist
Before an examination or practical demonstration, ensure that you can:
Explain ANI, AGI and ASI.
Differentiate AI, ML, DL and Generative AI.
Derive Bayes' theorem and explain \(P(X,Y)\) versus \(P(Y\mid X)\).
Calculate approximate FP16, INT8 and INT4 model memory.
Explain perception, planning, memory and action in an AI agent.
Draw the Azure Machine Learning architecture.
Explain the difference between Azure Machine Learning and Azure OpenAI.
Draw the Transformer encoder-decoder architecture.
Derive scaled dot-product attention.
Explain why attention scores are divided by \(\sqrt{d_k}\).
Compare BPE, WordPiece and SentencePiece.
Explain CBOW, Skip-Gram and GloVe.
Calculate cosine similarity.
Differentiate prompt engineering, RAG and LoRA.
Execute an NLP preprocessing pipeline.
Perform tokenization, stemming and lemmatization.
Explain POS tagging and NER.
Calculate TF-IDF.
Run sentiment analysis using VADER or TextBlob.
Explain Azure AI Language sentiment, entity and PII operations.
Configure Azure OpenAI environment variables.
Execute a chat completion and JSON-mode request.
Explain temperature, Top-p and token budgeting.
Explain groundedness, relevance and coherence.
2.5.5 Experiment coverage matrix
Experiment
Main coverage
Practical implementation
2.1
AI taxonomy, ML, DL, GenAI, agents, Azure ML
Logistic Regression vs GaussianNB
2.2
RNN, LSTM, Transformers, attention, tokenization, embeddings, RAG, LoRA
Scaled dot-product attention and cosine similarity
2.3
NLP pipeline, stemming, lemmatization, POS, NER, TF-IDF, sentiment, Azure Language
Complete NLTK + spaCy pipeline and Azure Text Analytics
2.4
Azure OpenAI, prompts, JSON mode, Prompt Flow, evaluation, cost and latency
Complete Azure OpenAI SDK programs

# UNIT 3: SPEECH PROCESSING, COMPUTER VISION, OCR AND MASTER LAB COMPENDIUM

# **EXPERIMENT 3.1: SPEECH AI, AUDIO PROCESSING AND AZURE SPEECH SERVICES**

## **3.1.1 Aim and objectives**

**[DIRECTLY IN NOTES]**

**Aim:** To study speech-enabled AI applications and understand how speech recognition and speech synthesis are used to create intelligent voice-based systems.

Objectives:

1. Understand Speech-to-Text (STT) and Text-to-Speech (TTS).
2. Study the stages of speech recognition.
3. Understand audio preprocessing and feature extraction.
4. Study acoustic and language modelling.
5. Implement audio feature extraction.
6. Understand Azure AI Speech SDK services.

## **3.1.2 Speech AI architecture**

Speech AI enables users to communicate with computers using voice.

- **STT:** Converts spoken audio into text.
- **TTS:** Converts text into synthesized speech.
- **Speech translation:** Converts spoken language into another language, often producing translated text or audio.

### **Speech-to-Text architecture**

```
       HUMAN SPEECH
             |
             v
        MICROPHONE
             |
             v
       ANALOG-TO-DIGITAL
          CONVERSION
             |
             v
       AUDIO PREPROCESSING
       Noise reduction, VAD
             |
             v
       FEATURE EXTRACTION
        MFCC / Log-Mel
             |
             v
       ACOUSTIC ENCODER
       DNN / Transformer
             |
             v
       LANGUAGE MODEL
             |
             v
          DECODER
             |
             v
        RECOGNIZED TEXT
```

### **Text-to-Speech architecture**

```
          INPUT TEXT
              |
              v
       TEXT NORMALIZATION
              |
              v
      LINGUISTIC ANALYSIS
              |
              v
    GRAPHEME-TO-PHONEME
              |
              v
       PROSODY GENERATION
       Pitch, stress, pauses
              |
              v
       ACOUSTIC MODEL
              |
              v
       NEURAL VOCODER
              |
              v
        AUDIO WAVEFORM
              |
              v
       SPEAKER / HEADPHONES
```

The STT system estimates the most likely text sequence given an audio signal. A simplified probabilistic formulation is:

\[ \hat{W}=\arg\max_W P(W\mid A) \]

Using Bayes' theorem:

\[ P(W\mid A)\propto P(A\mid W)P(W) \]

Where:

- \(A\): Observed audio.
- \(W\): Candidate word sequence.
- \(P(A\mid W)\): Acoustic likelihood.
- \(P(W)\): Language-model probability.

The decoder selects the word sequence with the highest posterior probability.

## **3.1.3 Audio capture, sampling and Nyquist-Shannon theorem**

**[RESTORED STANDARD THEORY]**

Sound is a continuous-time pressure wave. A computer processes a discrete sequence of samples.

Sampling converts a continuous signal \(x(t)\) into discrete values:

\[ x[n]=x\left(\frac{n}{f_s}\right) \]

Where:

- \(f_s\): Sampling frequency in samples per second.
- \(n\): Sample index.

### **Nyquist-Shannon sampling theorem**

A band-limited signal with maximum frequency \(f\_{\max}\) can theoretically be reconstructed from its samples if:

\[ \boxed{f_s>2f\_{\max}} \]

The Nyquist frequency is:

\[ f_N=\frac{f_s}{2} \]

Example:

If the highest frequency to be represented is 4,000 Hz, the sampling frequency must be greater than 8,000 samples per second, with appropriate anti-aliasing filtering.

| Sampling rate | Nyquist frequency |
| ------------- | ----------------- |
| 8 kHz         | 4 kHz             |
| 16 kHz        | 8 kHz             |
| 22.05 kHz     | 11.025 kHz        |
| 44.1 kHz      | 22.05 kHz         |
| 48 kHz        | 24 kHz            |

**⚠ Examiner's flag:** Sampling at exactly twice the maximum frequency is a theoretical boundary. Real systems use practical margins and anti-aliasing filters.

## **3.1.4 Framing and windowing**

Speech is non-stationary over long intervals, but it can often be approximated as locally stationary over short frames.

The audio signal is divided into overlapping frames.

Example configuration:

- Sampling frequency: 16,000 Hz.
- Frame duration: 25 ms.
- Frame shift: 10 ms.

Frame length:

\[ N=0.025\times16000=400 \]

Frame shift:

\[ H=0.010\times16000=160 \]

Therefore, each frame contains 400 samples and successive frames begin 160 samples apart.

### **Windowing**

Windowing reduces discontinuities at frame boundaries before spectral analysis.

The Hamming window is:

\[ \boxed{ w[n]=0.54-0.46\cos\left(\frac{2\pi n}{N-1}\right) } \]

For \(0\leq n\<N\).

The Hann window is:

\[ \boxed{ w[n]=0.5\left(1-\cos\left(\frac{2\pi n}{N-1}\right)\right) } \]

The windowed frame is:

\[ x_w[n]=x[n]w[n] \]

## **3.1.5 Discrete Fourier Transform and spectrograms**

The Discrete Fourier Transform converts a finite sequence from the time domain into its frequency-domain representation.

\[ \boxed{ X[k]=\sum\_{n=0}^{N-1}x[n]e^{-j2\pi kn/N} } \]

The inverse DFT is:

\[ x[n]=\frac{1}{N} \sum\_{k=0}^{N-1}X[k]e^{j2\pi kn/N} \]

The Fast Fourier Transform (FFT) is an efficient algorithm for computing the DFT.

### **Short-Time Fourier Transform**

For speech, the Short-Time Fourier Transform (STFT) is calculated over successive windowed frames:

\[ STFT(m,k)= \sum\_{n=0}^{N-1} x[n+mH]w[n]e^{-j2\pi kn/N} \]

A spectrogram displays signal energy across time and frequency:

\[ S(m,k)=|STFT(m,k)|^2 \]

```
       FREQUENCY
           ^
           |
       High|  .  .  .  .
           |  || ||  || 
           | |||||||||||
        Low|____________________> TIME
             Speech energy
```

A spectrogram is useful for visualizing vowels, consonants, pauses, harmonics and noise.

## **3.1.6 Mel-frequency filter banks and MFCC derivation**

**[RESTORED STANDARD THEORY]**

The human auditory system does not perceive frequency linearly. Mel-frequency scaling approximates this non-linear frequency perception.

A commonly used Mel conversion is:

\[ \boxed{ m(f)=2595\log\_{10}\left(1+\frac{f}{700}\right) } \]

The inverse is:

\[ f(m)=700\left(10^{m/2595}-1\right) \]

### **MFCC extraction steps**

```
          RAW AUDIO
              |
              v
       PRE-EMPHASIS
              |
              v
       FRAMING + WINDOWING
              |
              v
             FFT
              |
              v
        POWER SPECTRUM
              |
              v
      MEL FILTER BANKS
              |
              v
       LOG MEL ENERGIES
              |
              v
             DCT
              |
              v
            MFCCs
```

**Step 1: Pre-emphasis**

\[ y[n]=x[n]-\alpha x[n-1] \]

A typical value is \(\alpha\approx0.97\), although modern pipelines may omit or alter this step.

**Step 2: Power spectrum**

\[ P[k]=\frac{|X[k]|^2}{N} \]

**Step 3: Mel filter-bank energy**

For filter \(m\):

\[ E_m=\sum_k H_m[k]P[k] \]

Where \(H_m[k]\) is the triangular Mel filter.

**Step 4: Log energy**

\[ L_m=\ln(E_m+\epsilon) \]

A small \(\epsilon\) prevents taking the logarithm of zero.

**Step 5: Discrete Cosine Transform**

\[ \boxed{ MFCC_n= \sum\_{m=0}^{M-1} L_m \cos\left[ \frac{\pi n}{M} \left(m+\frac12\right) \right] } \]

Where:

- \(M\): Number of Mel filters.
- \(n\): Cepstral coefficient index.

MFCCs provide a compact representation of the spectral envelope of speech.

## **3.1.7 Acoustic and language modelling**

### **Acoustic models**

Acoustic models map audio features to phonetic or linguistic units.

| Model                       | Description                                             |
| --------------------------- | ------------------------------------------------------- |
| HMM                         | Represents temporal state transitions                   |
| GMM-HMM                     | Uses Gaussian mixtures for acoustic observations        |
| DNN-HMM                     | Uses neural networks to estimate acoustic probabilities |
| CTC                         | Handles unaligned input and output sequences            |
| Conformer                   | Combines convolution and Transformer attention          |
| Encoder-decoder Transformer | Uses attention-based sequence modelling                 |

### **HMM-GMM**

A Hidden Markov Model assumes hidden states \(q_t\) that evolve over time.

\[ P(Q,O)=P(q_1) \prod\_{t=2}^{T}P(q_t\mid q\_{t-1}) \prod\_{t=1}^{T}P(o_t\mid q_t) \]

Where:

- \(Q\): Hidden state sequence.
- \(O\): Observed feature sequence.
- \(P(q_t\mid q\_{t-1})\): Transition probability.
- \(P(o_t\mid q_t)\): Emission probability.

A Gaussian Mixture Model represents an observation distribution as:

\[ p(x)=\sum\_{k=1}^{K} \pi_k\mathcal{N}(x\mid\mu_k,\Sigma_k) \]

### **Language models**

An N-gram language model approximates a word's probability using previous words.

\[ P(w_1,\ldots,w_n) \approx \prod\_{i=1}^{n} P(w_i\mid w\_{i-(N-1)},\ldots,w\_{i-1}) \]

Neural language models can capture longer-range context and more complex language patterns.

**Examiner's comparison:**

- Acoustic model: What sounds were spoken?
- Language model: Which word sequence is linguistically plausible?
- Decoder: Which sequence best combines both sources of evidence?

## **3.1.8 Azure AI Speech Services**

**[DIRECTLY IN NOTES: SPEECH RECOGNITION AND SYNTHESIS]**

Azure AI Speech provides managed speech capabilities, including:

- Real-time speech recognition.
- Batch transcription.
- Text-to-speech synthesis.
- Speech translation.
- Speech SDK integration.
- SSML-based voice control.

### **Azure Speech architecture**

```
       PYTHON / APPLICATION
                |
                v
          AZURE SPEECH SDK
                |
       +--------+---------+
       |        |         |
       v        v         v
      STT      TTS    TRANSLATION
       |        |         |
       +--------+---------+
                |
                v
         AZURE SPEECH SERVICE
                |
                v
        TEXT / AUDIO RESPONSE
```

### **Installation**

```
python -m pip install azure-cognitiveservices-speech
```

Configure credentials:

macOS / Linux:

```
export AZURE_SPEECH_KEY="YOUR_SPEECH_KEY"
export AZURE_SPEECH_REGION="YOUR_RESOURCE_REGION"
```

### **Complete Azure Speech SDK script**

Save as `azure_speech_demo.py`.

```python
import os
import azure.cognitiveservices.speech as speechsdk

speech_key = os.getenv("AZURE_SPEECH_KEY")
speech_region = os.getenv("AZURE_SPEECH_REGION")

if not speech_key or not speech_region:
    print("Azure Speech credentials not set. Showing architecture and execution template.")
    print("Configure AZURE_SPEECH_KEY and AZURE_SPEECH_REGION to run live audio.")
else:
    speech_config = speechsdk.SpeechConfig(subscription=speech_key, region=speech_region)
    speech_config.speech_recognition_language = "en-US"

    # 1. Speech-to-Text from Microphone
    print("Speak into microphone for Speech-to-Text...")
    audio_config = speechsdk.audio.AudioConfig(use_default_microphone=True)
    recognizer = speechsdk.SpeechRecognizer(speech_config=speech_config, audio_config=audio_config)

    result = recognizer.recognize_once_async().get()
    if result.reason == speechsdk.ResultReason.RecognizedSpeech:
        print(f"Recognized Text: {result.text}")
    elif result.reason == speechsdk.ResultReason.NoMatch:
        print("No speech could be recognized.")
    elif result.reason == speechsdk.ResultReason.Canceled:
        print(f"Recognition canceled: {result.cancellation_details.reason}")

    # 2. Text-to-Speech Synthesis with SSML
    print("\nSynthesizing speech with SSML prosody control...")
    synthesizer = speechsdk.SpeechSynthesizer(speech_config=speech_config)
    ssml_text = """
    <speak version='1.0' xmlns='http://www.w3.org/2001/10/synthesis' xml:lang='en-US'>
        <voice name='en-US-JennyNeural'>
            <prosody rate='+10%' pitch='+2Hz'>
                Welcome to Chandigarh University AI Applications Laboratory.
            </prosody>
        </voice>
    </speak>
    """
    synth_result = synthesizer.speak_ssml_async(ssml_text).get()
    if synth_result.reason == speechsdk.ResultReason.SynthesizingAudioCompleted:
        print("SSML speech synthesis completed successfully.")
```

**Expected output:**

```
AZURE SPEECH MENU
1. Speech to Text
2. Text to Speech
3. SSML Synthesis
4. Exit

Choose: 1
Speak into your microphone.
Recognized: Hello, welcome to the AI lab.
```

The recognized sentence depends on the audio, language configuration and service response.

### **SSML**

Speech Synthesis Markup Language controls how synthesized speech is delivered.

Common SSML controls:

- Voice selection.
- Speaking rate.
- Pitch.
- Volume.
- Pauses.
- Pronunciation.
- Emphasis.

### **Speech translation**

A translation workflow can be implemented with the Speech SDK's translation classes. The service needs a supported source language and one or more target languages.

```
import osimport azure.cognitiveservices.speech as speechsdkkey = os.getenv("AZURE_SPEECH_KEY")region = os.getenv("AZURE_SPEECH_REGION")if not key or not region:    raise SystemExit("Set Azure Speech credentials.")config = speechsdk.translation.SpeechTranslationConfig(    subscription=key,    region=region)config.speech_recognition_language = "en-US"config.add_target_language("hi")audio = speechsdk.audio.AudioConfig(    use_default_microphone=True)recognizer = speechsdk.translation.TranslationRecognizer(    translation_config=config,    audio_config=audio)print("Speak an English sentence.")result = recognizer.recognize_once_async().get()if result.reason == speechsdk.ResultReason.TranslatedSpeech:    print("Original:", result.text)    print("Hindi:", result.translations.get("hi", ""))else:    print("Translation failed:", result.reason)
```

## **3.1.9 Audio feature extraction and MFCC visualization**

**[LAB / EXAM SUPPORT]**

### **Installation**

```
python -m pip install librosa matplotlib numpy soundfile
```

### **Complete executable script**

Save as `audio_features.py`.

```
import sysimport numpy as npimport librosaimport librosa.displayimport matplotlib.pyplot as pltif len(sys.argv) < 2:    raise SystemExit(        "Usage: python audio_features.py input.wav"    )audio_path = sys.argv[1]# Load audio as mono at 16 kHzsignal, sample_rate = librosa.load(    audio_path,    sr=16000,    mono=True)duration = len(signal) / sample_rateprint("Sample rate:", sample_rate)print("Number of samples:", len(signal))print("Duration:", round(duration, 3), "seconds")# Extract MFCCmfcc = librosa.feature.mfcc(    y=signal,    sr=sample_rate,    n_mfcc=13,    n_fft=400,    hop_length=160,    n_mels=40)# Extract STFT magnitudestft = np.abs(    librosa.stft(        signal,        n_fft=512,        hop_length=160    ))# Convert to decibel scalespectrogram_db = librosa.amplitude_to_db(    stft,    ref=np.max)# Plot waveformplt.figure(figsize=(12, 3))librosa.display.waveshow(signal, sr=sample_rate)plt.title("Audio Waveform")plt.xlabel("Time (seconds)")plt.ylabel("Amplitude")plt.tight_layout()plt.show()# Plot spectrogramplt.figure(figsize=(12, 4))librosa.display.specshow(    spectrogram_db,    sr=sample_rate,    hop_length=160,    x_axis="time",    y_axis="hz")plt.colorbar(format="%+2.0f dB")plt.title("Magnitude Spectrogram")plt.tight_layout()plt.show()# Plot MFCCplt.figure(figsize=(12, 4))librosa.display.specshow(    mfcc,    sr=sample_rate,    hop_length=160,    x_axis="time")plt.colorbar()plt.title("13 MFCC Coefficients")plt.ylabel("MFCC coefficient")plt.tight_layout()plt.show()print("MFCC matrix shape:", mfcc.shape)print("Audio feature extraction completed.")
```

Run:

```
python audio_features.py speech.wav
```

**Expected output:**

```
Sample rate: 16000
Number of samples: ...
Duration: ... seconds
MFCC matrix shape: (13, ...)
Audio feature extraction completed.
```

The script generates waveform, spectrogram and MFCC plots. The number of frames depends on the recording duration and hop length.

## **3.1.10 Examiner's flags**

1. Sampling rate is measured in samples per second, not bits per second.
2. Bit depth controls amplitude quantization resolution.
3. Nyquist frequency is half the sampling rate.
4. Framing and windowing are not the same operation.
5. FFT computes frequency-domain information, not text.
6. MFCCs are compact audio features, not recognized words.
7. Acoustic models and language models have different responsibilities.
8. STT and TTS are inverse in task direction, not mathematical inverses.
9. SSML controls speech delivery, not the semantic content of a sentence.
10. A Speech SDK requires valid credentials, region and network access.

# **EXPERIMENT 3.2: COMPUTER VISION, CNNs AND DEEPFACE**

## **3.2.1 Aim and objectives**

**[DIRECTLY IN NOTES]**

To study computer vision and understand how AI systems process, classify, detect and interpret visual information.

Objectives:

- Understand digital image representation.
- Study image processing and filters.
- Understand convolution and CNN architecture.
- Compare CNNs and Vision Transformers.
- Explore facial analysis and Azure AI Vision.

## **3.2.2 Digital image representation**

An image is a two-dimensional or multi-dimensional array of pixel values.

### **Grayscale image**

A grayscale image has one channel.

\[ I\in\mathbb{R}^{H\times W} \]

For an 8-bit grayscale image:

\[ I(i,j)\in\\{0,1,\ldots,255\\} \]

- 0: Black.
- 255: White.
- Intermediate values: Gray levels.

### **RGB image**

An RGB image has three channels.

\[ I\in\mathbb{R}^{H\times W\times3} \]

The channels are:

- Red.
- Green.
- Blue.

For an image of 224 × 224 pixels:

\[ 224\times224\times3=150,528 \]

pixel-channel values.

```
           RGB IMAGE
      +-------------------+
      |       PIXELS      |
      |                   |
      |   R   G   B       |
      |   |   |   |       |
      +---|---|---|-------+
          |   |   |
       Red Green Blue
```

### **Common color spaces**

| Color space | Purpose                               |
| ----------- | ------------------------------------- |
| RGB         | General color representation          |
| Grayscale   | Intensity-only processing             |
| HSV         | Hue, saturation and value             |
| BGR         | OpenCV's common default channel order |
| LAB         | Perceptual color representation       |

**⚠ Examiner's flag:** OpenCV commonly loads color images in BGR order, while many other libraries use RGB.

## **3.2.3 Fundamental image processing**

**[RESTORED STANDARD THEORY]**

### **A. Thresholding**

Thresholding converts an image into a binary image using a threshold \(T\).

\[ I'(x,y)= \begin{cases} 255,&I(x,y)>T\\\ 0,&I(x,y)\leq T \end{cases} \]

### **B. Gaussian blur**

Gaussian blur reduces high-frequency noise.

\[ G(x,y)= \frac{1}{2\pi\sigma^2} e^{-\frac{x^2+y^2}{2\sigma^2}} \]

The filtered image is:

\[ I\_{\text{blur}}=I\*G \]

### **C. Sobel edge detection**

Sobel approximates image intensity derivatives.

Horizontal kernel:

\[ G_x= \begin{bmatrix} -1&0&1\\\ -2&0&2\\\ -1&0&1 \end{bmatrix} \]

Vertical kernel:

\[ G_y= \begin{bmatrix} -1&-2&-1\\\ 0&0&0\\\ 1&2&1 \end{bmatrix} \]

Gradient magnitude:

\[ \boxed{ G=\sqrt{G_x^2+G_y^2} } \]

### **D. Canny edge detection**

Canny edge detection typically consists of:

1. Gaussian smoothing.
2. Gradient computation.
3. Non-maximum suppression.
4. Double thresholding.
5. Edge tracking by hysteresis.

## **3.2.4 CNN architecture**

A Convolutional Neural Network learns spatial features from images.

Typical architecture:

```
        INPUT IMAGE
       224 x 224 x 3
              |
              v
       CONVOLUTION LAYER
              |
              v
             ReLU
              |
              v
         MAX POOLING
              |
              v
       CONVOLUTION LAYER
              |
              v
             ReLU
              |
              v
         MAX POOLING
              |
              v
           FLATTEN
              |
              v
       FULLY CONNECTED
              |
              v
           SOFTMAX
              |
              v
       CLASS PREDICTION
```

### **A. 2D convolution**

For image \(I\) and kernel \(K\):

\[ \boxed{ (I\*K)(i,j)= \sum_m\sum_n I(i-m,j-n)K(m,n) } \]

In practical deep-learning libraries, the operation is often implemented as cross-correlation rather than a mathematically flipped convolution kernel. The terminology "convolution" is commonly retained.

### **B. Output dimension**

For an input width or height \(W\), kernel size \(K\), padding \(P\) and stride \(S\):

\[ \boxed{ O=\left\lfloor \frac{W-K+2P}{S} \right\rfloor+1 } \]

Example:

- Input width: 32.
- Kernel: 3.
- Padding: 1.
- Stride: 1.

\[ O= \left\lfloor \frac{32-3+2}{1} \right\rfloor+1 =32 \]

The output spatial dimension remains 32.

### **C. ReLU activation**

\[ \boxed{ReLU(x)=\max(0,x)} \]

### **D. Leaky ReLU**

\[ LeakyReLU(x)= \begin{cases} x,&x\geq0\\\ \alpha x,&x<0 \end{cases} \]

### **E. Pooling**

Max pooling selects the largest value in a local region.

Average pooling computes the mean of the local region.

For a 2 × 2 max-pooling region:

\[ \begin{bmatrix} 1&3\\\ 2&4 \end{bmatrix} \rightarrow4 \]

### **F. Fully connected layer**

\[ z=Wx+b \]

### **G. Softmax**

For class \(i\):

\[ \boxed{ P(y=i\mid x)= \frac{e^{z_i}}{\sum_j e^{z_j}} } \]

The output values sum to 1 and represent the model's class probabilities.

## **3.2.5 Vision Transformers versus CNNs**

**[DIRECTLY IN NOTES: VISION TRANSFORMERS]**

A Vision Transformer divides an image into patches, converts each patch into a vector and applies self-attention.

For an image of size \(H\times W\), with patch size \(P\times P\), the number of patches is:

\[ N=\frac{HW}{P^2} \]

For a 224 × 224 image and 16 × 16 patches:

\[ N=\frac{224\times224}{16^2}=196 \]

Each patch is flattened and projected:

\[ z_i=x_iE \]

Where \(E\) is a learned projection matrix.

The patch embeddings are combined with positional embeddings:

\[ Z_0=[x\_{\text{class}};z_1;\ldots;z_N]+E\_{\text{pos}} \]

Self-attention then models relationships among image patches.

| CNN                                 | Vision Transformer                          |
| ----------------------------------- | ------------------------------------------- |
| Convolution filters                 | Patch embeddings and attention              |
| Strong local inductive bias         | Global attention relationships              |
| Naturally captures local patterns   | Learns relationships across patches         |
| Often efficient on smaller datasets | Often benefits from large-scale pretraining |
| Spatial feature maps                | Token sequence representations              |

## **3.2.6 Image processing with OpenCV**

Install:

```
python -m pip install opencv-python matplotlib numpy
```

Complete script:

```python
import cv2
import numpy as np
import matplotlib.pyplot as plt
import sys

image_path = sys.argv[1] if len(sys.argv) > 1 else None

if image_path:
    img = cv2.imread(image_path)
    if img is None:
        sys.exit(f"Could not load image: {image_path}")
else:
    # Create 300x300 synthetic test image with shapes
    img = np.ones((300, 300, 3), dtype=np.uint8) * 200
    cv2.circle(img, (150, 150), 60, (50, 50, 200), -1)
    cv2.rectangle(img, (50, 50), (120, 120), (200, 100, 50), -1)
    print("Using synthetic geometric image for demonstration.")

# 1. Grayscale Conversion (BGR -> Gray)
gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)

# 2. Gaussian Blur (Noise Reduction)
blurred = cv2.GaussianBlur(gray, (5, 5), 1.5)

# 3. Binary Thresholding
_, thresh = cv2.threshold(blurred, 127, 255, cv2.THRESH_BINARY)

# 4. Sobel Edge Detection (G_x and G_y)
sobel_x = cv2.Sobel(blurred, cv2.CV_64F, 1, 0, ksize=3)
sobel_y = cv2.Sobel(blurred, cv2.CV_64F, 0, 1, ksize=3)
sobel_mag = np.sqrt(sobel_x**2 + sobel_y**2)
sobel_mag = np.uint8(np.clip(sobel_mag, 0, 255))

# 5. Canny Edge Detection (Hysteresis & Non-Max Suppression)
canny_edges = cv2.Canny(blurred, threshold1=50, threshold2=150)

# 6. Plotting Image Processing Pipeline
fig, axes = plt.subplots(2, 3, figsize=(12, 8))
axes[0, 0].imshow(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
axes[0, 0].set_title("Original RGB")
axes[0, 1].imshow(gray, cmap="gray")
axes[0, 1].set_title("Grayscale")
axes[0, 2].imshow(blurred, cmap="gray")
axes[0, 2].set_title("Gaussian Blur")
axes[1, 0].imshow(thresh, cmap="gray")
axes[1, 0].set_title("Binary Threshold")
axes[1, 1].imshow(sobel_mag, cmap="gray")
axes[1, 1].set_title("Sobel Gradient Magnitude")
axes[1, 2].imshow(canny_edges, cmap="gray")
axes[1, 2].set_title("Canny Edges")

for ax in axes.flatten():
    ax.axis("off")

plt.tight_layout()
plt.show()
print("Image processing pipeline successfully executed.")
```

## **3.2.7 DeepFace facial attribute analysis**

**[LAB / EXAM SUPPORT]**

DeepFace provides high-level facial analysis functions. Depending on the version and selected backend, it can estimate attributes such as age, gender presentation, emotion and demographic categories.

These are model predictions, not verified facts about a person. Such inferences can be inaccurate and may be inappropriate for consequential decisions. Obtain consent and use only for legitimate, low-risk demonstrations.

### **Installation**

```
python -m pip install deepface opencv-python
```

### **Complete script**

```
from deepface import DeepFaceimport sysif len(sys.argv) < 2:    raise SystemExit("Usage: python deepface_analysis.py face.jpg")image_path = sys.argv[1]try:    results = DeepFace.analyze(        img_path=image_path,        actions=[            "age",            "gender",            "emotion"        ],        enforce_detection=True    )    if isinstance(results, dict):        results = [results]    for index, result in enumerate(results, start=1):        print(f"\nFACE {index}")        print("Estimated age:", result.get("age"))        print("Gender scores:", result.get("gender"))        print("Dominant emotion:", result.get("dominant_emotion"))        print("Emotion scores:", result.get("emotion"))        print(            "Face region:",            result.get("region")        )
```

**Expected output structure:**

```
FACE 1
Estimated age: ...
Gender scores: {...}
Dominant emotion: ...
Emotion scores: {...}
Face region: {...}
```

Exact values depend on the input image, model weights and installed DeepFace version.

## **3.2.8 Azure AI Vision Image Analysis**

**[RESTORED STANDARD AZURE LAB SUPPORT]**

Azure AI Vision supports image-analysis tasks such as:

- Image captions.
- Dense captions where supported.
- Tags.
- Object detection.
- Smart crops.
- OCR/read operations.

### **Conceptual architecture**

```
             IMAGE INPUT
                  |
                  v
           AZURE AI VISION
                  |
       +----------+----------+
       |          |          |
       v          v          v
    CAPTION     TAGS      OBJECTS
       |          |          |
       +----------+----------+
                  |
                  v
             OCR / READ
                  |
                  v
          STRUCTURED RESPONSE
```

### **SDK installation**

```
python -m pip install azure-ai-vision-imageanalysis
```

The current SDK interface and supported features depend on the installed package and resource configuration. The following example uses the Image Analysis 4.0 client pattern.

Configure:

```
export AZURE_VISION_ENDPOINT="https://YOUR-RESOURCE.cognitiveservices.azure.com/"
export AZURE_VISION_KEY="YOUR_KEY"
```

### **Complete script**

```
import osimport sysfrom azure.ai.vision.imageanalysis import ImageAnalysisClientfrom azure.ai.vision.imageanalysis.models import VisualFeaturesfrom azure.core.credentials import AzureKeyCredentialendpoint = os.getenv("AZURE_VISION_ENDPOINT")key = os.getenv("AZURE_VISION_KEY")if not endpoint or not key:    raise SystemExit("Set Azure Vision endpoint and key.")if len(sys.argv) < 2:    raise SystemExit("Usage: python azure_vision.py image.jpg")image_path = sys.argv[1]client = ImageAnalysisClient(    endpoint=endpoint,    credential=AzureKeyCredential(key))with open(image_path, "rb") as image_file:    image_data = image_file.read()result = client.analyze(    image_data=image_data,    visual_features=[        VisualFeatures.CAPTION,        VisualFeatures.DENSE_CAPTIONS,        VisualFeatures.TAGS,        VisualFeatures.OBJECTS,        VisualFeatures.READ    ]
```

**Note:** Smart crop support and output availability can vary by API version, model and resource region. Verify the exact supported feature list for the deployed service before using it in a practical examination.

## **3.2.9 Examiner's flags**

1. A pixel is a numerical representation, not a physical dot of fixed size.
2. RGB and BGR use different channel orders.
3. Grayscale conversion does not mean thresholding.
4. Gaussian blur reduces noise but may also remove useful detail.
5. Sobel estimates gradients; Canny includes multiple edge-processing stages.
6. CNN convolution output size depends on padding, stride and kernel size.
7. Pooling reduces spatial dimensions, not necessarily the number of channels.
8. Softmax converts logits into normalized class scores.
9. Object detection predicts locations and classes; segmentation predicts pixel labels.
10. DeepFace demographic and emotion outputs are estimates, not objective identity facts.

# **EXPERIMENT 3.3: INFORMATION EXTRACTION, OCR AND AZURE DOCUMENT INTELLIGENCE**

## **3.3.1 Aim and objectives**

**[DIRECTLY IN NOTES]**

**Aim:** To study AI-based information extraction and understand how structured data can be extracted from unstructured documents using OCR, field extraction, field mapping and data normalization.

Objectives:

1. Understand information extraction.
2. Study Optical Character Recognition.
3. Understand OCR preprocessing.
4. Differentiate OCR and intelligent document processing.
5. Extract fields and key-value pairs.
6. Study Azure AI Document Intelligence.

## **3.3.2 Information Extraction**

Information Extraction (IE) converts unstructured or semi-structured data into structured information.

Examples:

| Input             | Information to extract                |
| ----------------- | ------------------------------------- |
| Invoice           | Invoice number, date, vendor, total   |
| Receipt           | Store, date, items, tax, total        |
| Identity document | Name, document number, expiry date    |
| Medical record    | Patient details, diagnoses, medicines |
| Business card     | Name, email, phone, organization      |
| Application form  | Name, address, selected options       |

### **IE architecture**

```
        UNSTRUCTURED INPUT
                 |
      +----------+----------+
      |          |          |
      v          v          v
    TEXT      IMAGE       PDF
      |          |          |
      +----------+----------+
                 |
                 v
           OCR / PARSING
                 |
                 v
        TEXT + LAYOUT OUTPUT
                 |
                 v
          FIELD DETECTION
                 |
                 v
          FIELD ASSOCIATION
                 |
                 v
       NORMALIZATION / VALIDATION
                 |
                 v
         STRUCTURED INFORMATION
                 |
                 v
         DATABASE / APPLICATION
```

### **Two important stages**

**1. Text extraction:** OCR identifies visible characters and produces text.

**2. Field extraction:** The system interprets the text and associates it with meaningful field names.

Example:

OCR text:

```
Invoice No: INV-2026-105
Date: 21/11/2026
Total: ₹5,500
```

Structured output:

```
{
  "invoice_number": "INV-2026-105",
  "invoice_date": "2026-11-21",
  "total_amount": 5500
}
```

## **3.3.3 OCR pipeline**

**[DIRECTLY IN NOTES + RESTORED STANDARD THEORY]**

OCR converts text contained in images or scanned documents into machine-readable text.

```
           IMAGE ACQUISITION
                  |
                  v
           IMAGE PREPROCESSING
                  |
       +----------+----------+
       |          |          |
       v          v          v
    DENOISE    BINARIZE    DESKEW
       |          |          |
       +----------+----------+
                  |
                  v
           TEXT REGION DETECTION
                  |
                  v
            LINE SEGMENTATION
                  |
                  v
          CHARACTER RECOGNITION
                  |
                  v
          POST-PROCESSING
                  |
                  v
             OCR OUTPUT
```

### **A. Binarization**

Binarization converts an image into foreground and background pixels.

Global thresholding:

\[ I'(x,y)= \begin{cases} 255,&I(x,y)>T\\\ 0,&I(x,y)\leq T \end{cases} \]

Adaptive thresholding calculates a local threshold for different image regions. It is often more suitable for uneven illumination.

### **B. Deskewing**

Deskewing corrects tilted text.

If the document is rotated by angle \(\theta\), the image is transformed using a rotation matrix:

\[ R(\theta)= \begin{bmatrix} \cos\theta&-\sin\theta\\\ \sin\theta&\cos\theta \end{bmatrix} \]

### **C. Line segmentation**

The OCR system identifies separate text lines, often using connected components or horizontal projection profiles.

For a binary image, a horizontal projection profile can be calculated as:

\[ H(y)=\sum_x I(x,y) \]

Rows with few or no foreground pixels may indicate gaps between text lines.

### **D. Character recognition**

The OCR model classifies character shapes using pattern recognition or learned neural representations.

### **E. Post-processing**

Post-processing can include:

- Spelling correction.
- Language-model correction.
- Date normalization.
- Currency normalization.
- Reading-order correction.
- Confidence-based review.

## **3.3.4 Raw OCR versus Intelligent Document Processing**

| Raw OCR                                | Intelligent Document Processing                 |
| -------------------------------------- | ----------------------------------------------- |
| Reads visible text                     | Understands document structure and fields       |
| Produces character strings             | Produces structured data                        |
| May preserve basic positions           | Uses layout, labels and relationships           |
| Does not inherently know field meaning | Associates values with field names              |
| Requires further processing            | Can combine extraction, validation and workflow |

### **Key-value association**

Example:

```
Invoice Number: INV-105
Invoice Date: 21/11/2026
Total Amount: ₹5,500
```

The system identifies:

\[ Key=\text{Invoice Number} \]

\[ Value=\text{INV-105} \]

It uses proximity, layout, text relationships and model predictions to associate labels and values.

## **3.3.5 Bounding boxes and confidence scores**

Document extraction systems often return the position of words, lines or fields.

A bounding box can be represented as:

\[ B=(x_1,y_1,x_2,y_2) \]

Where:

- \(x_1,y_1\): Top-left coordinate.
- \(x_2,y_2\): Bottom-right coordinate.

Some services return polygons instead of four-coordinate rectangles.

Confidence is generally a score between 0 and 1:

\[ 0\leq c\leq1 \]

A higher confidence score indicates greater model confidence, not guaranteed correctness.

**⚠ Examiner's flag:** Bounding-box coordinates may be normalized, pixel-based or expressed in page units. Always inspect the returned coordinate system and page dimensions.

## **3.3.6 Azure AI Document Intelligence**

**[RESTORED STANDARD AZURE LAB SUPPORT]**

Azure AI Document Intelligence extracts text, layout and structured fields from documents.

### **Common model categories**

| Model type                  | Use                                        |
| --------------------------- | ------------------------------------------ |
| Prebuilt invoice            | Invoice fields and line items              |
| Prebuilt receipt            | Merchant, date, total and items            |
| Prebuilt identity document  | Supported identity-document fields         |
| Layout model                | Text, tables, selection marks and geometry |
| Custom extraction model     | User-defined document fields               |
| Custom classification model | Document-type classification               |

### **Architecture**

```
             DOCUMENT INPUT
                   |
                   v
        AZURE DOCUMENT INTELLIGENCE
                   |
          +--------+--------+
          |                 |
          v                 v
      PREBUILT MODEL    CUSTOM MODEL
          |                 |
          +--------+--------+
                   |
                   v
           OCR + LAYOUT ANALYSIS
                   |
                   v
           FIELD EXTRACTION
                   |
                   v
          CONFIDENCE SCORING
                   |
                   v
           VALIDATION RULES
                   |
                   v
          STRUCTURED JSON DATA
```

### **Installation**

The current SDK is:

```
python -m pip install azure-ai-documentintelligence azure-core
```

The older `azure-ai-formrecognizer` package is the predecessor. For new projects, prefer the current `azure-ai-documentintelligence` package unless the lab specifically requires the legacy SDK.

### **Configure credentials**

```
export AZURE_DOCUMENT_INTELLIGENCE_ENDPOINT="https://YOUR-RESOURCE.cognitiveservices.azure.com/"
export AZURE_DOCUMENT_INTELLIGENCE_KEY="YOUR-KEY"
```

### **Complete Azure Document Intelligence script**

Save as `azure_document_intelligence.py`.

```
import osimport sysimport jsonfrom azure.core.credentials import AzureKeyCredentialfrom azure.ai.documentintelligence import DocumentIntelligenceClientendpoint = os.getenv("AZURE_DOCUMENT_INTELLIGENCE_ENDPOINT")key = os.getenv("AZURE_DOCUMENT_INTELLIGENCE_KEY")if not endpoint or not key:    raise SystemExit(        "Set AZURE_DOCUMENT_INTELLIGENCE_ENDPOINT "        "and AZURE_DOCUMENT_INTELLIGENCE_KEY."    )if len(sys.argv) < 2:    raise SystemExit(        "Usage: python azure_document_intelligence.py invoice.pdf"    )file_path = sys.argv[1]client = DocumentIntelligenceClient(    endpoint=endpoint,    credential=AzureKeyCredential(key))with open(file_path, "rb") as document:    poller = client.begin_analyze_document(        "prebuilt-invoice",        body=document,        content_type="application/pdf"    )
```

**Important compatibility note:** The SDK's accepted request shape and returned field-value properties can differ between package versions. If your installed version rejects `body` or a field property, check that version's API reference and use its corresponding input stream and typed field accessors. The endpoint, key, deployed resource and model availability must also be configured.

## **3.3.7 Local OCR using OpenCV and Tesseract**

**[LAB / EXAM SUPPORT]**

### **Installation**

macOS:

```
brew install tesseract
python -m pip install pytesseract opencv-python matplotlib
```

Ubuntu:

```
sudo apt-get install tesseract-ocr
python -m pip install pytesseract opencv-python matplotlib
```

### **Complete executable script**

Save as `local_ocr.py`.

```
import cv2import pytesseractimport sysimport reimport jsonif len(sys.argv) < 2:    raise SystemExit("Usage: python local_ocr.py document.png")image_path = sys.argv[1]image = cv2.imread(image_path)if image is None:    raise SystemExit("Could not read the image.")# 1. Grayscale conversiongray = cv2.cvtColor(    image,    cv2.COLOR_BGR2GRAY)# 2. Denoisingdenoised = cv2.fastNlMeansDenoising(    gray,    None,    10,    7,    21)# 3. Adaptive thresholdingbinary = cv2.adaptiveThreshold(    denoised,    255,    cv2.ADAPTIVE_THRESH_GAUSSIAN_C,    cv2.THRESH_BINARY,    31,    11)# 4. OCRcustom_config = "--oem 3 --psm 6"text = pytesseract.image_to_string(    binary,    config=custom_config)print("\nOCR TEXT")print(text)# 5. Word-level OCR data and bounding boxesdata = pytesseract.image_to_data(    binary,    output_type=pytesseract.Output.DICT,    config=custom_config)print("\nWORD BOUNDING BOXES")for i, word in enumerate(data["text"]):    word = word.strip()    if not word:        continue    try:        confidence = float(data["conf"][i])    except ValueError:        continue    x = data["left"][i]    y = data["top"][i]    width = data["width"][i]    height = data["height"][i]    print({        "text": word,        "confidence": confidence,        "bbox": [            x,            y,            x + width,            y + height        ]    })# 6. Simple field extractionfields = {}patterns = {    "invoice_number": r"Invoice\s*(?:No|Number)?\s*[:#]?\s*([A-Z0-9-]+)",    "date": r"Date\s*[:#]?\s*([0-9./-]+)",    "total": r"Total\s*[:#]?\s*[$₹]?\s*([0-9,]+(?:\.[0-9]{1,2})?)"}for field_name, pattern in patterns.items():    match = re.search(        pattern,        text,        flags=re.IGNORECASE    )    fields[field_name] = (        match.group(1) if match else None    )print("\nEXTRACTED FIELDS")print(json.dumps(fields, indent=4))# 7. Save preprocessed imagecv2.imwrite("preprocessed_ocr.png", binary)print("\nSaved preprocessed image as preprocessed_ocr.png")
```

**Expected output structure:**

```
OCR TEXT
Invoice No: INV-105
Date: 21/11/2026
Total: ₹5,500

WORD BOUNDING BOXES
{'text': 'Invoice', 'confidence': ..., 'bbox': [...]}
...

EXTRACTED FIELDS
{
    "invoice_number": "INV-105",
    "date": "21/11/2026",
    "total": "5,500"
}

Saved preprocessed image as preprocessed_ocr.png
```

The regex extractor is a teaching example. Production document extraction requires stronger validation, currency parsing, locale-aware dates and document-specific field association.

## **3.3.8 Examiner's flags**

1. OCR and field extraction are different stages.
2. Poor input image quality lowers recognition accuracy.
3. Deskewing corrects rotation; denoising removes unwanted variation.
4. A bounding box describes location, not semantic meaning.
5. Confidence is not a guarantee of correctness.
6. OCR may confuse similar characters such as `0/O`, `1/I` and `5/S`.
7. Table extraction must preserve row and column relationships.
8. Custom extraction models require representative training documents.
9. Validate extracted dates, amounts and totals.
10. Do not store identity-document or financial data without appropriate authorization and security.

# **4. TEN HIGH-YIELD SOLVED LAB PRACTICAL PROGRAMS**

The following programs are standalone practicals. Each program includes its own imports and sample data or input handling. Install the required dependencies before running it.

## **Program 1. End-to-end data preprocessing and outlier treatment**

**Objective:** Handle missing values, encode categorical variables, scale numeric features and treat outliers using the IQR method.

**[LAB / EXAM SUPPORT]**

Install:

```
python -m pip install pandas numpy scikit-learn
```

Complete script:

```
import numpy as np
import pandas as pd
from sklearn.compose import ColumnTransformer
from sklearn.preprocessing import StandardScaler, OneHotEncoder
from sklearn.impute import SimpleImputer
from sklearn.pipeline import Pipeline

# 1. Sample Dataset with Missing Values and Outliers
data = {
    "age": [18, 19, 20, 21, 22, np.nan, 19, 120],
    "marks": [75, 82, 90, 65, np.nan, 88, 79, 95],
    "attendance": [80, 85, 90, 70, 75, 88, 82, 99],
    "department": ["CSE", "IT", "CSE", "ECE", "IT", "CSE", "ECE", "CSE"]
}
df = pd.DataFrame(data)
print("ORIGINAL DATA:")
print(df)

# 2. IQR-Based Outlier Detection and Capping
numeric_cols = ["age", "marks", "attendance"]
for col in numeric_cols:
    q1 = df[col].quantile(0.25)
    q3 = df[col].quantile(0.75)
    iqr = q3 - q1
    lower = q1 - 1.5 * iqr
    upper = q3 + 1.5 * iqr
    print(f"{col}: Q1={q1:.1f}, Q3={q3:.1f}, IQR={iqr:.1f}, Lower={lower:.2f}, Upper={upper:.2f}")
    df[col] = df[col].clip(lower=lower, upper=upper)

print("\nDATA AFTER OUTLIER CAPPING:")
print(df)

# 3. ColumnTransformer Pipeline for Imputation and Scaling
numeric_transformer = Pipeline([
    ("imputer", SimpleImputer(strategy="median")),
    ("scaler", StandardScaler())
])

categorical_transformer = Pipeline([
    ("imputer", SimpleImputer(strategy="most_frequent")),
    ("onehot", OneHotEncoder(sparse_output=False, drop="first"))
])

preprocessor = ColumnTransformer(
    transformers=[
        ("num", numeric_transformer, numeric_cols),
        ("cat", categorical_transformer, ["department"])
    ]
)

transformed_matrix = preprocessor.fit_transform(df)
cat_names = list(preprocessor.named_transformers_["cat"].named_steps["onehot"].get_feature_names_out(["department"]))
feature_names = numeric_cols + cat_names

print("\nTRANSFORMED NUMERICAL MATRIX:")
transformed_df = pd.DataFrame(transformed_matrix, columns=feature_names)
print(transformed_df.round(3))
print("\nFinal Matrix Shape:", transformed_matrix.shape)

```

**Expected output:** The program displays the original dataset, IQR bounds, a transformed numerical matrix and its shape. The matrix contains scaled numerical columns and one-hot encoded department columns.

**Examiner's flag:** In a real ML workflow, fit the outlier boundaries and preprocessing transformations on training data only. Applying them to the full dataset before splitting can leak information from the test set.

## **Program 2. Comprehensive EDA with heatmaps and correlation analysis**

**Objective:** Perform descriptive statistics, missing-value analysis, correlation analysis and visualization.

Install:

```
python -m pip install pandas numpy matplotlib seaborn
```

Complete script:

```
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

np.random.seed(42)
n = 150
df = pd.DataFrame({
    "age": np.random.randint(18, 60, n),
    "study_hours": np.random.uniform(1, 10, n),
    "attendance": np.random.uniform(50, 100, n),
    "marks": np.random.normal(70, 12, n)
})
df["marks"] = (df["marks"] + df["study_hours"] * 1.5 + df["attendance"] * 0.08).clip(0, 100)

# Introduce controlled missing values
df.loc[[4, 17, 42], "marks"] = np.nan

print("1. DATA HEAD:")
print(df.head())
print("\n2. DATASET INFO:")
print(df.info())
print("\n3. DESCRIPTIVE STATISTICS:")
print(df.describe().round(2))
print("\n4. MISSING VALUES PER COLUMN:")
print(df.isna().sum())

# Clean missing values for correlation analysis
df_clean = df.fillna(df.median())

# Correlation Matrix
corr_matrix = df_clean.corr()
print("\n5. PEARSON CORRELATION MATRIX:")
print(corr_matrix.round(3))

# Visualizations
fig, axes = plt.subplots(1, 3, figsize=(16, 5))

# Heatmap
sns.heatmap(corr_matrix, annot=True, cmap="coolwarm", fmt=".2f", ax=axes[0], square=True)
axes[0].set_title("Correlation Heatmap")

# Boxplot for Outliers
sns.boxplot(data=df_clean, ax=axes[1])
axes[1].set_title("Boxplots of Numerical Features")

# Scatter Plot with Regression Trendline
sns.regplot(data=df_clean, x="study_hours", y="marks", scatter_kws={"alpha": 0.6}, line_kws={"color": "red"}, ax=axes[2])
axes[2].set_title("Study Hours vs Marks (Trendline)")

plt.tight_layout()
plt.show()
print("\nEDA Visualizations successfully generated.")

```

**Expected output:** Dataset preview, descriptive statistics, missing-value counts, correlation matrix, heatmap, boxplot and scatter plot.

**Examiner's flag:** Correlation measures association, not causation. A strong correlation does not prove that one variable causes another.

## **Program 3. Supervised classification pipeline with feature scaling**

**Objective:** Train a classification model with a stratified train-test split and a leakage-safe preprocessing pipeline.

Install:

```
python -m pip install scikit-learn pandas numpy
```

Complete script:

```
import numpy as np
import pandas as pd
from sklearn.datasets import load_breast_cancer
from sklearn.model_selection import train_test_split
from sklearn.pipeline import Pipeline
from sklearn.impute import SimpleImputer
from sklearn.preprocessing import StandardScaler
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score, classification_report, confusion_matrix, roc_auc_score

# 1. Load Dataset
dataset = load_breast_cancer(as_frame=True)
X, y = dataset.data, dataset.target

# 2. Stratified Train-Test Split (80/20)
X_train, X_test, y_train, y_test = train_test_split(
    X, y, test_size=0.20, random_state=42, stratify=y
)

# 3. Leakage-Free Classification Pipeline
model = Pipeline([
    ("imputer", SimpleImputer(strategy="median")),
    ("scaler", StandardScaler()),
    ("classifier", LogisticRegression(max_iter=3000, random_state=42))
])

# 4. Fit Model on Training Set
model.fit(X_train, y_train)

# 5. Predict on Test Set
predictions = model.predict(X_test)
probabilities = model.predict_proba(X_test)[:, 1]

# 6. Evaluation Metrics
acc = accuracy_score(y_test, predictions)
auc = roc_auc_score(y_test, probabilities)
cm = confusion_matrix(y_test, predictions)

print(f"ACCURACY:  {acc:.4f}")
print(f"ROC-AUC:   {auc:.4f}")
print("\nCONFUSION MATRIX:")
print(cm)
print("\nCLASSIFICATION REPORT:")
print(classification_report(y_test, predictions, target_names=dataset.target_names))

print("SAMPLE ACTUAL VS PREDICTED (FIRST 10 SAMPLES):")
comparison = pd.DataFrame({"Actual": y_test.iloc[:10].values, "Predicted": predictions[:10]})
print(comparison)

```

**Expected output:** Accuracy, confusion matrix, precision, recall, F1-score and actual-versus-predicted values.

**Examiner's flag:** The breast-cancer dataset's numeric target labels map to the dataset's target names. Do not assume that class `1` always means "positive" in another dataset.

## **Program 4. Comparative multi-model benchmark with 5-fold Stratified CV**

**Objective:** Compare multiple classifiers using identical stratified folds and evaluation metrics.

Install:

```
python -m pip install scikit-learn pandas matplotlib
```

Complete script:

```
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
from sklearn.datasets import load_breast_cancer
from sklearn.model_selection import StratifiedKFold, cross_validate
from sklearn.pipeline import Pipeline
from sklearn.preprocessing import StandardScaler
from sklearn.impute import SimpleImputer
from sklearn.linear_model import LogisticRegression
from sklearn.svm import SVC
from sklearn.neighbors import KNeighborsClassifier
from sklearn.tree import DecisionTreeClassifier
from sklearn.ensemble import RandomForestClassifier
from sklearn.naive_bayes import GaussianNB

# Load dataset
dataset = load_breast_cancer(as_frame=True)
X, y = dataset.data, dataset.target

# 6 Classifiers inside Preprocessing Pipelines
models = {
    "Logistic Regression": Pipeline([
        ("imputer", SimpleImputer(strategy="median")),
        ("scaler", StandardScaler()),
        ("classifier", LogisticRegression(max_iter=3000, random_state=42))
    ]),
    "SVC (RBF)": Pipeline([
        ("imputer", SimpleImputer(strategy="median")),
        ("scaler", StandardScaler()),
        ("classifier", SVC(probability=True, random_state=42))
    ]),
    "KNN (k=5)": Pipeline([
        ("imputer", SimpleImputer(strategy="median")),
        ("scaler", StandardScaler()),
        ("classifier", KNeighborsClassifier(n_neighbors=5))
    ]),
    "Decision Tree": Pipeline([
        ("imputer", SimpleImputer(strategy="median")),
        ("classifier", DecisionTreeClassifier(max_depth=5, random_state=42))
    ]),
    "Random Forest": Pipeline([
        ("imputer", SimpleImputer(strategy="median")),
        ("classifier", RandomForestClassifier(n_estimators=100, random_state=42))
    ]),
    "Gaussian NB": Pipeline([
        ("imputer", SimpleImputer(strategy="median")),
        ("classifier", GaussianNB())
    ])
}

# 5-Fold Stratified Cross-Validation
cv = StratifiedKFold(n_splits=5, shuffle=True, random_state=42)
scoring = {
    "accuracy": "accuracy",
    "precision": "precision",
    "recall": "recall",
    "f1": "f1",
    "roc_auc": "roc_auc"
}

results = []
for name, pipeline in models.items():
    scores = cross_validate(pipeline, X, y, cv=cv, scoring=scoring, n_jobs=-1)
    results.append({
        "Model": name,
        "Accuracy": scores["test_accuracy"].mean(),
        "Precision": scores["test_precision"].mean(),
        "Recall": scores["test_recall"].mean(),
        "F1-Score": scores["test_f1"].mean(),
        "ROC-AUC": scores["test_roc_auc"].mean(),
        "Std Dev": scores["test_accuracy"].std()
    })

comparison_df = pd.DataFrame(results).sort_values(by="F1-Score", ascending=False).reset_index(drop=True)
print("MULTI-MODEL COMPARISON TABLE (5-FOLD STRATIFIED CV):")
print(comparison_df.round(4).to_string(index=False))

# Grouped Bar Chart
comparison_df.set_index("Model")[["Accuracy", "Precision", "Recall", "F1-Score", "ROC-AUC"]].plot(
    kind="bar", figsize=(12, 6), width=0.8
)
plt.title("Comparative Performance of 6 Classification Algorithms (5-Fold CV)")
plt.ylabel("Score")
plt.ylim(0.80, 1.02)
plt.xticks(rotation=25, ha="right")
plt.grid(axis="y", linestyle="--", alpha=0.5)
plt.tight_layout()
plt.show()

```

**Expected output:** A comparison table containing mean accuracy, precision, recall, F1 and ROC-AUC for six classifiers, followed by a grouped bar chart.

**Examiner's flag:** Cross-validation scores estimate generalization performance. Do not use the same final test set repeatedly to select models and tune hyperparameters.

## **Program 5. Tokenization, stemming and lemmatization using NLTK**

**Objective:** Demonstrate fundamental NLP preprocessing operations.

Install:

```
python -m pip install nltk
```

Complete script:

```
import nltk
from nltk.tokenize import sent_tokenize, word_tokenize
from nltk.corpus import stopwords
from nltk.stem import PorterStemmer, WordNetLemmatizer
import pandas as pd

# Download required NLTK resources
for resource in ["punkt", "punkt_tab", "stopwords", "wordnet", "omw-1.4"]:
    nltk.download(resource, quiet=True)

text = (
    "Students are studying artificial intelligence, designing intelligent algorithms, "
    "and optimizing neural networks in modern computer laboratories."
)

print("ORIGINAL TEXT:")
print(text)

# 1. Tokenization
sentences = sent_tokenize(text)
tokens = word_tokenize(text)
print(f"\nTotal Sentences: {len(sentences)}")
print(f"Total Word Tokens: {len(tokens)}")

# 2. Stopword Filtering
stop_words = set(stopwords.words("english"))
filtered_tokens = [w.lower() for w in tokens if w.isalpha() and w.lower() not in stop_words]
print(f"Filtered Tokens (non-stopwords): {filtered_tokens}")

# 3. Stemming vs Lemmatization
stemmer = PorterStemmer()
lemmatizer = WordNetLemmatizer()

comparison = []
for word in filtered_tokens:
    stem = stemmer.stem(word)
    lemma_noun = lemmatizer.lemmatize(word, pos="n")
    lemma_verb = lemmatizer.lemmatize(word, pos="v")
    comparison.append({
        "Word": word,
        "Porter Stem": stem,
        "Lemma (Noun)": lemma_noun,
        "Lemma (Verb)": lemma_verb
    })

comparison_df = pd.DataFrame(comparison)
print("\nSTEMMING VS LEMMATIZATION COMPARISON:")
print(comparison_df.to_string(index=False))

```

**Expected output:** Token list, filtered words, Porter stems and WordNet lemmas.

**Examiner's flag:** Lemmatization without POS information can produce a different result from verb-aware lemmatization.

## **Program 6. Named Entity Recognition and dependency parsing using spaCy**

**Objective:** Identify entities and grammatical dependency relationships.

Install:

```
python -m pip install spacy
python -m spacy download en_core_web_sm
```

Complete script:

```
import spacy
import pandas as pd

# Load spaCy English core model
try:
    nlp = spacy.load("en_core_web_sm")
except OSError:
    import sys
    sys.exit("spaCy model missing. Run: python -m spacy download en_core_web_sm")

text = (
    "Microsoft Corporation was founded by Bill Gates and Paul Allen on April 4, 1975, "
    "in Albuquerque, New Mexico. In 2026, the company invested $10 billion in AI research."
)

doc = nlp(text)

print("1. TOKENS, POS TAGS AND DEPENDENCY PARSING:")
token_data = []
for token in doc:
    token_data.append({
        "Text": token.text,
        "Lemma": token.lemma_,
        "POS": token.pos_,
        "Tag": token.tag_,
        "Dep": token.dep_,
        "Head": token.head.text
    })
token_df = pd.DataFrame(token_data)
print(token_df.head(15).to_string(index=False))

print("\n2. NAMED ENTITY RECOGNITION (NER):")
entity_data = []
for ent in doc.ents:
    entity_data.append({
        "Entity": ent.text,
        "Label": ent.label_,
        "Explanation": spacy.explain(ent.label_)
    })
entity_df = pd.DataFrame(entity_data)
print(entity_df.to_string(index=False))

print("\n3. SENTENCE ROOT TOKENS:")
for sent in doc.sents:
    print(f"Sentence: '{sent.text.strip()}' -> Root: {sent.root.text} ({sent.root.pos_})")

```

**Expected output:** Token-level POS and dependency information, named entities and sentence root tokens.

**Examiner's flag:** NER identifies entity mentions. It does not guarantee that two mentions refer to the same real-world entity.

## **Program 7. TF-IDF matrix and cosine similarity matching**

**Objective:** Convert text documents into TF-IDF vectors and calculate document similarity.

Install:

```
python -m pip install scikit-learn numpy
```

Complete script:

```
import numpy as np
import pandas as pd
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.metrics.pairwise import cosine_similarity

documents = [
    "Artificial intelligence uses machine learning algorithms for predictions.",
    "Machine learning and deep learning are subsets of artificial intelligence.",
    "Computer vision algorithms analyze visual scenes, images, and video frames.",
    "Natural language processing processes human text and speech signals."
]

# 1. Compute TF-IDF Matrix
vectorizer = TfidfVectorizer(stop_words="english")
tfidf_matrix = vectorizer.fit_transform(documents)
feature_names = vectorizer.get_feature_names_out()

print("1. VOCABULARY FEATURES (TOTAL: " + str(len(feature_names)) + "):")
print(feature_names)

print("\n2. TF-IDF MATRIX:")
tfidf_df = pd.DataFrame(tfidf_matrix.toarray(), columns=feature_names)
print(tfidf_df.round(3).to_string())

# 3. Pairwise Document Cosine Similarity
similarity_matrix = cosine_similarity(tfidf_matrix)
print("\n3. DOCUMENT PAIRWISE COSINE SIMILARITY:")
sim_df = pd.DataFrame(similarity_matrix, index=[f"Doc {i+1}" for i in range(len(documents))],
                                       columns=[f"Doc {i+1}" for i in range(len(documents))])
print(sim_df.round(3))

# 4. Search Query Matching
query = ["machine learning in artificial intelligence"]
query_vector = vectorizer.transform(query)
query_similarities = cosine_similarity(query_vector, tfidf_matrix).flatten()

print(f"\n4. QUERY: '{query[0]}'")
print("SIMILARITY SCORES WITH CORPUS:")
for idx, score in enumerate(query_similarities):
    print(f"Doc {idx+1}: {score:.4f} -> \"{documents[idx]}\"")

best_doc_idx = np.argmax(query_similarities)
print(f"\nBest Matching Document: Doc {best_doc_idx+1} (Score: {query_similarities[best_doc_idx]:.4f})")

```

**Expected output:** Vocabulary, TF-IDF feature matrix, similarity matrix and best-matching document.

**Examiner's flag:** Cosine similarity measures vector direction, not semantic understanding by itself. TF-IDF similarity is lexical and may miss synonyms.

## **Program 8. Audio feature extraction with Librosa**

**Objective:** Generate MFCC and spectrogram features from a supplied audio file.

Install:

```
python -m pip install librosa matplotlib numpy soundfile
```

Complete script:

```
import sys
import numpy as np
import librosa
import librosa.display
import matplotlib.pyplot as plt

# Generate a synthetic audio chirp/tone if no file provided
audio_path = sys.argv[1] if len(sys.argv) > 1 else None

if audio_path:
    signal, sr = librosa.load(audio_path, sr=16000, mono=True)
else:
    # 2 seconds of 440 Hz (A4) sine wave at 16 kHz
    sr = 16000
    t = np.linspace(0, 2, int(sr * 2), endpoint=False)
    signal = 0.5 * np.sin(2 * np.pi * 440 * t) + 0.25 * np.sin(2 * np.pi * 880 * t)
    print("No audio file supplied. Using 2-second synthetic dual-harmonic tone at 16 kHz.")

duration = len(signal) / sr
print(f"Sample Rate: {sr} Hz")
print(f"Total Samples: {len(signal)}")
print(f"Duration: {duration:.3f} seconds")

# 1. Extract 13 MFCCs
mfcc = librosa.feature.mfcc(y=signal, sr=sr, n_mfcc=13, n_fft=400, hop_length=160, n_mels=40)
print(f"MFCC Matrix Shape: {mfcc.shape} (13 coefficients x {mfcc.shape[1]} frames)")

# 2. Extract Log-Mel Spectrogram
mel_spec = librosa.feature.melspectrogram(y=signal, sr=sr, n_fft=512, hop_length=160, n_mels=64)
mel_spec_db = librosa.power_to_db(mel_spec, ref=np.max)

# 3. Visualizations
fig, axes = plt.subplots(3, 1, figsize=(12, 9))

# Waveform
librosa.display.waveshow(signal, sr=sr, ax=axes[0])
axes[0].set_title("Audio Waveform")
axes[0].set_xlabel("Time (s)")
axes[0].set_ylabel("Amplitude")

# Mel Spectrogram
img_mel = librosa.display.specshow(mel_spec_db, sr=sr, hop_length=160, x_axis="time", y_axis="mel", ax=axes[1])
fig.colorbar(img_mel, ax=axes[1], format="%+2.0f dB")
axes[1].set_title("Log-Mel Spectrogram (64 Mel Bands)")

# MFCC Heatmap
img_mfcc = librosa.display.specshow(mfcc, sr=sr, hop_length=160, x_axis="time", ax=axes[2])
fig.colorbar(img_mfcc, ax=axes[2])
axes[2].set_title("13 Mel-Frequency Cepstral Coefficients (MFCCs)")
axes[2].set_ylabel("MFCC Index")

plt.tight_layout()
plt.show()
print("Audio feature extraction and visualizations completed.")

```

**Expected output:** Audio sample rate, duration, MFCC matrix dimensions, Mel spectrogram dimensions and two visualizations.

**Examiner's flag:** Always check whether the input is mono or stereo and whether the library resampled it to the requested rate.

## **Program 9. CNN feature extraction and DeepFace facial emotion analysis**

**Objective:** Demonstrate CNN feature extraction using a pretrained image model and optional facial emotion analysis.

Install:

```
python -m pip install tensorflow pillow deepface
```

Complete script:

```
import sys
import numpy as np
from PIL import Image

image_path = sys.argv[1] if len(sys.argv) > 1 else None

# Part A: CNN Feature Extraction using TensorFlow/Keras or PyTorch
try:
    from tensorflow.keras.applications import MobileNetV2
    from tensorflow.keras.applications.mobilenet_v2 import preprocess_input, decode_predictions

    model = MobileNetV2(weights="imagenet", include_top=True)
    feature_extractor = MobileNetV2(weights="imagenet", include_top=False, pooling="avg")

    if image_path:
        img = Image.open(image_path).convert("RGB").resize((224, 224))
    else:
        # Synthetic test image
        img = Image.fromarray(np.random.randint(0, 255, (224, 224, 3), dtype=np.uint8))
        print("Using synthetic 224x224 RGB image for demonstration.")

    img_array = np.expand_dims(np.asarray(img, dtype=np.float32), axis=0)
    preprocessed_img = preprocess_input(img_array)

    # Classification Output
    preds = model.predict(preprocessed_img, verbose=0)
    top3 = decode_predictions(preds, top=3)[0]
    print("1. TOP-3 IMAGENET CLASSIFICATIONS:")
    for rank, (class_id, label, prob) in enumerate(top3, start=1):
        print(f"   {rank}. {label} ({class_id}): {prob*100:.2f}%")

    # Feature Representation Vector
    features = feature_extractor.predict(preprocessed_img, verbose=0)
    print(f"\n2. EXTRACTED CNN EMBEDDING VECTOR: Shape={features.shape} (1280-dim representation)")
    print(f"   First 8 components: {np.round(features[0, :8], 4)}")

except ImportError:
    print("TensorFlow not installed. CNN feature extraction skipped.")

# Part B: DeepFace Facial Attribute Analysis
if image_path:
    try:
        from deepface import DeepFace
        analysis = DeepFace.analyze(img_path=image_path, actions=["age", "gender", "emotion"], enforce_detection=False)
        if isinstance(analysis, list):
            analysis = analysis[0]
        print("\n3. DEEPFACE FACIAL ANALYSIS RESULTS:")
        print(f"   Estimated Age: {analysis.get('age')}")
        print(f"   Dominant Emotion: {analysis.get('dominant_emotion')}")
        print(f"   Emotion Scores: {analysis.get('emotion')}")
        print(f"   Dominant Gender: {analysis.get('dominant_gender')}")
    except Exception as e:
        print(f"DeepFace analysis note: {e}")

```

**Expected output:** Top-5 ImageNet predictions, a CNN feature vector of shape approximately `(1, 1280)` for MobileNetV2's average-pooled feature output, and optional emotion estimates if a face is detected.

**Examiner's flag:** ImageNet object classification is not facial recognition. CNN feature extraction produces numerical representations, not human-readable descriptions.

## **Program 10. Document OCR and information extraction with bounding boxes**

**Objective:** Extract text and word-level bounding boxes from a document image.

Install:

```
python -m pip install opencv-python pytesseract
```

Also install the Tesseract OCR engine using the operating system package manager.

Complete script:

```
import sys
import cv2
import re
import json

image_path = sys.argv[1] if len(sys.argv) > 1 else None

try:
    import pytesseract
    from pytesseract import Output
except ImportError:
    import sys
    sys.exit("pytesseract missing. Run: python -m pip install pytesseract")

if image_path:
    image = cv2.imread(image_path)
    if image is None:
        sys.exit(f"Could not load image: {image_path}")
else:
    # Create synthetic invoice document image
    image = np.ones((400, 600, 3), dtype=np.uint8) * 255
    cv2.putText(image, "TAX INVOICE", (200, 50), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 0, 0), 2)
    cv2.putText(image, "Invoice No: INV-2026-8842", (50, 120), cv2.FONT_HERSHEY_SIMPLEX, 0.6, (0, 0, 0), 2)
    cv2.putText(image, "Date: 21/11/2026", (50, 160), cv2.FONT_HERSHEY_SIMPLEX, 0.6, (0, 0, 0), 2)
    cv2.putText(image, "Customer: ABC Technologies", (50, 200), cv2.FONT_HERSHEY_SIMPLEX, 0.6, (0, 0, 0), 2)
    cv2.putText(image, "Total Amount: $4,850.00", (50, 260), cv2.FONT_HERSHEY_SIMPLEX, 0.7, (0, 0, 0), 2)
    print("Generated synthetic test invoice document image.")

# 1. Grayscale & Denoising
gray = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
denoised = cv2.fastNlMeansDenoising(gray, None, 10, 7, 21)

# 2. Adaptive Binarization
binary = cv2.adaptiveThreshold(denoised, 255, cv2.ADAPTIVE_THRESH_GAUSSIAN_C, cv2.THRESH_BINARY, 31, 11)

# 3. Tesseract OCR Text Extraction
config = "--oem 3 --psm 6"
raw_text = pytesseract.image_to_string(binary, config=config)
print("1. EXTRACTED OCR RAW TEXT:")
print("-" * 40)
print(raw_text.strip())
print("-" * 40)

# 4. Word-Level Bounding Box Extraction
ocr_data = pytesseract.image_to_data(binary, output_type=Output.DICT, config=config)
boxes = []
for i in range(len(ocr_data["text"])):
    word = ocr_data["text"][i].strip()
    conf = float(ocr_data["conf"][i])
    if word and conf > 30:
        x, y, w, h = ocr_data["left"][i], ocr_data["top"][i], ocr_data["width"][i], ocr_data["height"][i]
        boxes.append({"word": word, "conf": round(conf, 1), "bbox": [x, y, x + w, y + h]})

print(f"\n2. DETECTED WORDS WITH BOUNDING BOXES (TOTAL: {len(boxes)}):")
for b in boxes[:8]:
    print(f"   '{b['word']}': Conf={b['conf']}%, BBox={b['bbox']}")

# 5. Field Extraction via RegEx Matching
fields = {}
patterns = {
    "invoice_number": r"Invoice\s*(?:No|Number)?\s*[:#]?\s*([A-Za-z0-9-]+)",
    "date": r"Date\s*[:#]?\s*([0-9]{1,2}[./-][0-9]{1,2}[./-][0-9]{2,4})",
    "total_amount": r"Total(?:\s*Amount)?\s*[:#]?\s*([$₹]?[0-9,]+(?:\.[0-9]{2})?)"
}

for field_name, pattern in patterns.items():
    match = re.search(pattern, raw_text, re.IGNORECASE)
    fields[field_name] = match.group(1) if match else "Not Found"

print("\n3. STRUCTURED KEY-VALUE EXTRACTION:")
print(json.dumps(fields, indent=4))

```

**Expected output:** Recognized document text, word-level confidence scores, bounding-box coordinates and an image showing the detected word boxes.

**Examiner's flag:** Tesseract's confidence scores are engine-specific and should not be interpreted as calibrated probabilities.

# **5. COMPREHENSIVE MASTER VIVA VOCE QUESTION BANK**

30 questions with model answers

The questions below span all three units. Each includes a likely examiner follow-up.

## **Questions 1–10: Data preprocessing, EDA and supervised ML**

### **Q1. What is data preprocessing?**

**Answer:** Data preprocessing converts raw data into a clean and suitable format for analysis or machine learning. It includes missing-value handling, duplicate removal, encoding, scaling and outlier treatment.

**Follow-up:** Why is preprocessing necessary?

**Answer:** Raw data may contain missing values, inconsistent formats, noise and outliers that can reduce model reliability.

### **Q2. Differentiate normalization and standardization.**

**Answer:**

Normalization commonly rescales data into a specified range:

\[ x'=\frac{x-x\_{\min}}{x\_{\max}-x\_{\min}} \]

Standardization transforms data to zero mean and unit standard deviation:

\[ z=\frac{x-\mu}{\sigma} \]

**Follow-up:** Which is affected more by extreme values?

**Answer:** Min-max normalization is especially sensitive to extreme minimum and maximum values.

### **Q3. What is an outlier?**

**Answer:** An outlier is an observation that lies unusually far from the majority of observations.

**Follow-up:** Explain IQR-based detection.

**Answer:**

\[ IQR=Q_3-Q_1 \]

An observation below \(Q_1-1.5IQR\) or above \(Q_3+1.5IQR\) is commonly flagged as an outlier.

### **Q4. What is EDA?**

**Answer:** Exploratory Data Analysis is the process of inspecting, summarizing and visualizing data to understand distributions, relationships, missing values and unusual observations.

**Follow-up:** Name three EDA techniques.

**Answer:** Descriptive statistics, correlation analysis and visualization.

### **Q5. What is correlation?**

**Answer:** Correlation measures the strength and direction of association between variables.

**Follow-up:** Does correlation prove causation?

**Answer:** No. Correlation alone cannot establish a causal relationship.

### **Q6. Differentiate supervised and unsupervised learning.**

**Answer:** Supervised learning uses labeled data. Unsupervised learning finds patterns in data without target labels.

**Follow-up:** Give one example of each.

**Answer:** Supervised: spam classification. Unsupervised: customer clustering.

### **Q7. What is overfitting?**

**Answer:** Overfitting occurs when a model learns the training data too closely, including noise, and performs poorly on unseen data.

**Follow-up:** How can it be reduced?

**Answer:** Cross-validation, regularization, pruning, data augmentation and simpler models.

### **Q8. What is a confusion matrix?**

**Answer:** A confusion matrix compares actual and predicted class labels. In binary classification it contains true positives, true negatives, false positives and false negatives.

**Follow-up:** What is a false positive?

**Answer:** The model predicts the positive class when the actual class is negative.

### **Q9. Differentiate precision and recall.**

**Answer:**

\[ Precision=\frac{TP}{TP+FP} \]

\[ Recall=\frac{TP}{TP+FN} \]

Precision measures how many predicted positives are correct. Recall measures how many actual positives are detected.

**Follow-up:** Which is important in disease screening?

**Answer:** Recall is often particularly important because missing a real case can be costly.

### **Q10. Why is Stratified K-Fold used?**

**Answer:** It maintains approximately the same class proportions in each fold as in the complete dataset.

**Follow-up:** When is it useful?

**Answer:** When class labels are imbalanced or the dataset is relatively small.

## **Questions 11–20: AI taxonomy, agents, Transformers, NLP and Azure OpenAI**

### **Q11. Differentiate ANI, AGI and ASI.**

**Answer:**

- ANI: AI designed for specific tasks.
- AGI: A hypothetical system with broad human-level general intelligence.
- ASI: A hypothetical intelligence exceeding human capabilities across many domains.

**Follow-up:** Which category describes today's task-specific commercial AI systems?

**Answer:** Narrow AI.

### **Q12. Differentiate Machine Learning and Deep Learning.**

**Answer:** Machine Learning includes algorithms that learn patterns from data. Deep Learning uses neural networks with multiple layers to learn hierarchical representations.

**Follow-up:** Does every ML model use neural networks?

**Answer:** No. Decision trees, KNN and Support Vector Machines are ML methods that are not necessarily neural networks.

### **Q13. What are the four pillars of an AI agent?**

**Answer:** Perception, planning, memory and action.

**Follow-up:** What is the role of environment feedback?

**Answer:** It helps the agent evaluate the outcome of an action and decide what to do next.

### **Q14. What is the difference between an LLM and an SLM?**

**Answer:** An LLM generally has a larger parameter count and broader capability, while an SLM is designed to be smaller and more resource-efficient.

**Follow-up:** Is parameter count the only factor determining model quality?

**Answer:** No. Training data, architecture, optimization, inference configuration and task fit also matter.

### **Q15. Why do Transformers use attention?**

**Answer:** Attention allows a model to assign different weights to different tokens based on their contextual relevance.

**Follow-up:** Why is attention divided by \(\sqrt{d_k}\)?

**Answer:** To control the scale of dot-product scores and reduce softmax saturation in high dimensions.

### **Q16. What is positional encoding?**

**Answer:** Positional encoding adds information about token positions to Transformer representations.

**Follow-up:** Why is it needed?

**Answer:** Attention alone does not inherently represent the order of tokens.

### **Q17. What is an embedding?**

**Answer:** An embedding is a numerical vector representing an item such as a word, sentence, image or audio segment.

**Follow-up:** What is cosine similarity used for?

**Answer:** It compares vector directions to estimate similarity.

### **Q18. Differentiate stemming and lemmatization.**

**Answer:** Stemming applies heuristic word-reduction rules, while lemmatization uses linguistic information to identify dictionary base forms.

**Follow-up:** Which is generally more linguistically accurate?

**Answer:** Lemmatization.

### **Q19. What is Named Entity Recognition?**

**Answer:** NER identifies entities such as people, organizations, places, dates and monetary values in text.

**Follow-up:** Is NER the same as POS tagging?

**Answer:** No. POS tagging identifies grammatical categories, while NER identifies named entity types.

### **Q20. What is RAG?**

**Answer:** Retrieval-Augmented Generation retrieves relevant external information and supplies it to a language model as context before generating a response.

**Follow-up:** Does standard RAG update the model's parameters?

**Answer:** No. It usually retrieves information at inference time without retraining the model.

## **Questions 21–30: Speech processing, vision, CNNs, OCR and Document Intelligence**

### **Q21. What is Speech-to-Text?**

**Answer:** STT converts spoken audio into machine-readable text.

**Follow-up:** Name two important components of an STT system.

**Answer:** Acoustic modelling and language modelling.

### **Q22. State the Nyquist-Shannon sampling theorem.**

**Answer:** A band-limited signal can be reconstructed theoretically when the sampling frequency is greater than twice its maximum frequency.

\[ f_s>2f\_{\max} \]

**Follow-up:** What is the Nyquist frequency for a 16 kHz recording?

**Answer:** 8 kHz.

### **Q23. What are MFCCs?**

**Answer:** Mel-Frequency Cepstral Coefficients are compact audio features derived from log Mel-filter-bank energies using a Discrete Cosine Transform.

**Follow-up:** Why use the Mel scale?

**Answer:** It approximates the non-linear frequency perception of human hearing.

### **Q24. Differentiate STT and TTS.**

**Answer:** STT converts audio into text. TTS converts text into synthesized audio.

**Follow-up:** What is SSML?

**Answer:** Speech Synthesis Markup Language, used to control voice characteristics such as pauses, pitch and speaking rate.

### **Q25. What is a digital image?**

**Answer:** A digital image is represented as a matrix or tensor of pixel values.

**Follow-up:** How many channels does an RGB image have?

**Answer:** Three.

### **Q26. What is convolution in CNNs?**

**Answer:** Convolution applies a filter or kernel across an image or feature map to calculate feature responses.

**Follow-up:** What can a convolutional filter detect?

**Answer:** Edges, lines, textures and more complex learned features.

### **Q27. What is pooling?**

**Answer:** Pooling reduces the spatial dimensions of feature maps.

**Follow-up:** Differentiate max and average pooling.

**Answer:** Max pooling selects the maximum value in a region; average pooling calculates the mean.

### **Q28. Differentiate CNNs and Vision Transformers.**

**Answer:** CNNs use convolutional filters to extract local spatial patterns. Vision Transformers divide images into patches and use attention to model relationships among them.

**Follow-up:** What is a patch embedding?

**Answer:** A vector representation created by flattening and projecting an image patch into an embedding space.

### **Q29. What is OCR?**

**Answer:** Optical Character Recognition converts text visible in images or scanned documents into machine-readable text.

**Follow-up:** Why is deskewing used?

**Answer:** To correct tilted text so that recognition becomes more accurate.

### **Q30. Differentiate OCR and Intelligent Document Processing.**

**Answer:** OCR extracts visible text. Intelligent Document Processing additionally identifies fields, associates values with labels, extracts tables, validates data and produces structured information.

**Follow-up:** What is a confidence score?

**Answer:** A score indicating how confident the recognition or extraction model is in a prediction. It is not a guarantee of correctness.

# **6. MASTER EXAMINER'S PITFALLS AND DEBUGGING CHECKLIST**

## **6.1 Fifteen common practical errors**

| No. | Common error                            | Why it happens                                        | Correct approach                                              |
| --- | --------------------------------------- | ----------------------------------------------------- | ------------------------------------------------------------- |
| 1   | Scaling before train-test split         | Preprocessing learns from the test data               | Fit scaling inside a training pipeline                        |
| 2   | Including target in feature matrix      | Target leakage                                        | Separate `X` and `y`                                          |
| 3   | Using accuracy alone on imbalanced data | Majority class dominates                              | Report precision, recall, F1 and ROC-AUC                      |
| 4   | Treating correlation as causation       | Misinterpreting association                           | Use causal analysis and experimental design                   |
| 5   | Missing-value conversion error          | Strings such as `?` remain in numeric columns         | Replace invalid markers and use imputers                      |
| 6   | NLTK tokenizer resource error           | Required data package is missing                      | Download the required NLTK resource                           |
| 7   | spaCy model missing                     | Language model not installed                          | Install `en_core_web_sm`                                      |
| 8   | Stopword removal changes sentiment      | Negation is removed                                   | Preserve negation terms such as `not`                         |
| 9   | Embedding dimensions mismatch           | Different models or vector configurations             | Use the same embedding model and dimension                    |
| 10  | Audio sampling mismatch                 | Model expects a different sample rate                 | Resample audio correctly and check channels                   |
| 11  | MFCC shape confusion                    | Frames and coefficients are reversed or misunderstood | Inspect matrix shape and axis conventions                     |
| 12  | OpenCV image appears incorrect          | BGR and RGB are confused                              | Convert BGR to RGB for plotting                               |
| 13  | CNN tensor shape error                  | Missing batch or channel dimension                    | Check shape, such as `(1, 224, 224, 3)`                       |
| 14  | OCR returns scrambled text              | Low resolution, rotation or noise                     | Deskew, denoise, threshold and use suitable page segmentation |
| 15  | Azure authentication failure            | Wrong key, endpoint, region or deployment             | Verify resource configuration and environment variables       |

## **6.2 Common Python debugging commands**

Check installed packages:

```
python -m pip list
```

Check Python version:

```
python --version
```

Install a missing library:

```
python -m pip install PACKAGE_NAME
```

Check Tesseract:

```
tesseract --version
```

Check spaCy models:

```
python -m spacy validate
```

Check NLTK data paths:

```
import nltkprint(nltk.data.path)
```

Check an array's dimensions:

```
print(array.shape)print(array.dtype)
```

Check a DataFrame's missing values:

```
print(df.isnull().sum())
```

Check model input dimensions:

```
print(X_train.shape)print(X_test.shape)
```

Check Azure environment variables:

```
import osprint(bool(os.getenv("AZURE_SPEECH_KEY")))print(bool(os.getenv("AZURE_SPEECH_REGION")))
```

Do not print actual secrets in logs or screenshots.

# **7. ULTIMATE REVISION CHEAT SHEET**

## **7.1 Statistics and preprocessing**

| Concept             | Formula                                                  |
| ------------------- | -------------------------------------------------------- |
| Mean                | \(\bar{x}=\frac{1}{n}\sum\_{i=1}^n x_i\)               |
| Population variance | \(\sigma^2=\frac{1}{N}\sum\_{i=1}^{N}(x_i-\mu)^2\)     |
| Sample variance     | \(s^2=\frac{1}{n-1}\sum\_{i=1}^{n}(x_i-\bar{x})^2\)    |
| Standard deviation  | \(\sigma=\sqrt{\sigma^2}\)                             |
| Range               | \(x\_{\max}-x\_{\min}\)                                |
| IQR                 | \(Q_3-Q_1\)                                            |
| Z-score             | \(z=\frac{x-\mu}{\sigma}\)                             |
| Min-max scaling     | \(x'=\frac{x-x\_{\min}}{x\_{\max}-x\_{\min}}\)         |
| Standardization     | \(z=\frac{x-\mu}{\sigma}\)                             |
| Pearson correlation | \(r=\frac{\operatorname{Cov}(X,Y)}{\sigma_X\sigma_Y}\) |

### **Outlier boundaries**

\[ Lower=Q_1-1.5(IQR) \]

\[ Upper=Q_3+1.5(IQR) \]

## **7.2 Machine-learning metrics**

| Metric              | Formula                                                |
| ------------------- | ------------------------------------------------------ |
| Accuracy            | \(\frac{TP+TN}{TP+TN+FP+FN}\)                        |
| Precision           | \(\frac{TP}{TP+FP}\)                                 |
| Recall              | \(\frac{TP}{TP+FN}\)                                 |
| Specificity         | \(\frac{TN}{TN+FP}\)                                 |
| F1-score            | \(2\frac{Precision\times Recall}{Precision+Recall}\) |
| False Positive Rate | \(\frac{FP}{FP+TN}\)                                 |
| Error rate          | \(1-Accuracy\)                                       |

## **7.3 AI and Transformer formulas**

**Bayes' theorem:**

\[ P(A\mid B)= \frac{P(B\mid A)P(A)}{P(B)} \]

**Logistic sigmoid:**

\[ \sigma(z)=\frac{1}{1+e^{-z}} \]

**Softmax:**

\[ P_i=\frac{e^{z_i}}{\sum_j e^{z_j}} \]

**Scaled dot-product attention:**

\[ Attention(Q,K,V)= softmax\left(\frac{QK^T}{\sqrt{d_k}}\right)V \]

**Positional encoding:**

\[ PE(pos,2i)= \sin\left(\frac{pos}{10000^{2i/d\_{\text{model}}}}\right) \]

\[ PE(pos,2i+1)= \cos\left(\frac{pos}{10000^{2i/d\_{\text{model}}}}\right) \]

**Cosine similarity:**

\[ cos(A,B)=\frac{A\cdot B}{\\|A\\|\\|B\\|} \]

**TF-IDF:**

\[ TFIDF(t,d)=TF(t,d)\times IDF(t) \]

**LoRA:**

\[ W'=W+BA \]

## **7.4 Speech and audio formulas**

**Sampling:**

\[ x[n]=x\left(\frac{n}{f_s}\right) \]

**Nyquist condition:**

\[ f_s>2f\_{\max} \]

**Nyquist frequency:**

\[ f_N=\frac{f_s}{2} \]

**Hamming window:**

\[ w[n]=0.54-0.46\cos\left(\frac{2\pi n}{N-1}\right) \]

**Hann window:**

\[ w[n]=0.5\left(1-\cos\left(\frac{2\pi n}{N-1}\right)\right) \]

**DFT:**

\[ X[k]=\sum\_{n=0}^{N-1}x[n]e^{-j2\pi kn/N} \]

**Mel conversion:**

\[ m(f)=2595\log\_{10}\left(1+\frac{f}{700}\right) \]

**Pre-emphasis:**

\[ y[n]=x[n]-\alpha x[n-1] \]

## **7.5 Computer vision and CNN formulas**

**Convolution:**

\[ (I\*K)(i,j)=\sum_m\sum_n I(i-m,j-n)K(m,n) \]

**Convolution output size:**

\[ O=\left\lfloor\frac{W-K+2P}{S}\right\rfloor+1 \]

**ReLU:**

\[ ReLU(x)=\max(0,x) \]

**Leaky ReLU:**

\[ f(x)= \begin{cases} x,&x\geq0\\\ \alpha x,&x<0 \end{cases} \]

**Sobel gradient magnitude:**

\[ G=\sqrt{G_x^2+G_y^2} \]

**ViT patch count:**

\[ N=\frac{HW}{P^2} \]

## **7.6 OCR and information extraction**

**Bounding box:**

\[ B=(x_1,y_1,x_2,y_2) \]

**Confidence:**

\[ 0\leq c\leq1 \]

Remember:

- OCR: Reads text.
- IE: Extracts meaningful information.
- IDP: Combines document understanding, extraction, validation and workflow.
- Key-value association: Connects labels with corresponding values.
- Table extraction: Preserves row and column relationships.

## **7.7 Essential Scikit-Learn snippets**

**Train-test split:**

```
from sklearn.model_selection import train_test_splitX_train, X_test, y_train, y_test = train_test_split(    X,    y,    test_size=0.2,    random_state=42,    stratify=y)
```

**Standard scaling:**

```
from sklearn.preprocessing import StandardScalerscaler = StandardScaler()X_train_scaled = scaler.fit_transform(X_train)X_test_scaled = scaler.transform(X_test)
```

**Classification pipeline:**

```
from sklearn.pipeline import Pipelinefrom sklearn.preprocessing import StandardScalerfrom sklearn.linear_model import LogisticRegressionmodel = Pipeline([    ("scaler", StandardScaler()),    ("classifier", LogisticRegression(max_iter=2000))])model.fit(X_train, y_train)predictions = model.predict(X_test)
```

**Stratified cross-validation:**

```
from sklearn.model_selection import StratifiedKFoldcv = StratifiedKFold(    n_splits=5,    shuffle=True,    random_state=42)
```

**Evaluation:**

```
from sklearn.metrics import (    accuracy_score,    precision_score,    recall_score,    f1_score,    confusion_matrix)print(accuracy_score(y_test, predictions))print(precision_score(y_test, predictions))print(recall_score(y_test, predictions))print(f1_score(y_test, predictions))print(confusion_matrix(y_test, predictions))
```

## **7.8 Essential Azure environment variables**

macOS / Linux:

```
export AZURE_SPEECH_KEY="YOUR_KEY"
export AZURE_SPEECH_REGION="YOUR_REGION"

export AZURE_VISION_ENDPOINT="YOUR_ENDPOINT"
export AZURE_VISION_KEY="YOUR_KEY"

export AZURE_DOCUMENT_INTELLIGENCE_ENDPOINT="YOUR_ENDPOINT"
export AZURE_DOCUMENT_INTELLIGENCE_KEY="YOUR_KEY"

export AZURE_OPENAI_ENDPOINT="YOUR_ENDPOINT"
export AZURE_OPENAI_API_KEY="YOUR_KEY"
export AZURE_OPENAI_DEPLOYMENT="YOUR_DEPLOYMENT"
export AZURE_OPENAI_API_VERSION="YOUR_SUPPORTED_VERSION"
```

Python access:

```
import osspeech_key = os.getenv("AZURE_SPEECH_KEY")speech_region = os.getenv("AZURE_SPEECH_REGION")
```

Never hardcode or commit secrets to a public repository.

# **8. MASTER PRACTICAL EXAM PREPARATION CHECKLIST**

## **Before the practical**

- Python environment is working.
- Required libraries are installed.
- Dataset or sample input files are available.
- Correct file paths are used.
- Azure credentials are configured if needed.
- Tesseract is installed for local OCR.
- spaCy English model is installed.
- NLTK data resources are downloaded.
- Audio and image inputs can be opened.

## **During the practical**

- State the objective clearly.
- Explain the algorithm before running the code.
- Show input data and preprocessing steps.
- Run the program without skipping important stages.
- Display meaningful outputs.
- Explain the results and limitations.
- Handle errors without hiding them.
- Do not claim sample outputs are actual measured results.

## **Before submission**

- Include the program code.
- Include the required output or screenshots.
- Mention the libraries used.
- Explain the main algorithm.
- Include the result and conclusion.
- Verify that the code runs from a clean environment.

# **9. FINAL UNIT 3 COMPLETION MATRIX**

| Component                       | Coverage                                                                    |
| ------------------------------- | --------------------------------------------------------------------------- |
| Experiment 3.1: Speech AI       | STT, TTS, sampling, framing, FFT, MFCC, acoustic models, Azure Speech       |
| Experiment 3.2: Computer Vision | Pixels, image processing, CNNs, ViTs, DeepFace, Azure Vision                |
| Experiment 3.3: OCR and IE      | OCR pipeline, field extraction, bounding boxes, Azure Document Intelligence |
| Solved practicals               | 10 standalone Python programs                                               |
| Viva question bank              | 30 model answers with follow-ups                                            |
| Examiner pitfalls               | 15 common errors and fixes                                                  |
| Revision cheat sheet            | Statistics, ML, Transformers, audio, vision and OCR formulas                |

## **Important practical notes**

1. The sample datasets in the solved programs are for demonstration. Use the actual course repository datasets when a question specifically requires them.
2. Azure examples require a valid Azure resource, supported model or deployment, endpoint, credentials and applicable quota.
3. The exact Azure SDK interface may change between package releases. Keep the package version and service API version compatible.
4. DeepFace and other facial attribute models produce estimates. Do not treat age, gender presentation or emotion outputs as verified personal characteristics.
5. Model performance values are not invented in this compendium. Your actual scores depend on your input data, train-test split, library versions and model configuration.