# Student Performance Factors: Data Analysis & Insights

## 📋 Project Overview
This project performs an **Exploratory Data Analysis (EDA)** on a dataset of 2,392 students to determine which variables—ranging from study habits to parental involvement—impact academic outcomes. By identifying these patterns, we can better understand the drivers behind high GPAs and student success.

## 📊 Dataset Structure
The dataset consists of **2,392 entries** and **15 columns**. The data is remarkably clean, with **0% missing values** across all features.

### Feature Definitions
| Feature | Description |
| :--- | :--- |
| **StudentID** | Unique identifier for each student. |
| **Age** | Ranges from 15 to 18 years. |
| **Gender** | Binary (0: Male, 1: Female). |
| **Ethnicity** | Categorical (0: Caucasian, 1: African American, 2: Hispanic, 3: Asian). |
| **StudyTimeWeekly** | Continuous variable representing hours spent studying per week. |
| **Absences** | Number of classes missed during the school year. |
| **Tutoring** | Binary (0: No, 1: Yes). |
| **GPA** | Grade Point Average on a scale of 0.0 to 4.0. |
| **GradeClass** | Categorical classification of grades (0: 'A', 1: 'B', 2: 'C', 3: 'D', 4: 'F'). |

## 🛠️ Analysis Workflow

### 1. Data Inspection
*   Used `data.info()` and `data.isnull()` to verify data integrity.
*   Confirmed that all features are either `int64` or `float64`, making them suitable for immediate statistical analysis.

### 2. Demographic Profiling
*   **Age Distribution:** Visualised using boxplots to identify the primary student cohort.
*   **Gender Balance:** Utilised count plots to check for representation across the dataset.

### 3. Key Findings (Initial)
*   The student population is evenly distributed across ages 15–18.
*   The dataset is balanced, providing a fair basis for comparing gender-based performance metrics.
*   GPA shows a high variance, suggesting significant influence from behavioural features like `StudyTimeWeekly` and `Absences`.

## 🚀 Dependencies
To run the notebook and reproduce the visualisations, the following libraries are required:

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import warnings
```

## 📈 Future Work
*   **Correlation Heatmaps:** To quantify the relationship between parental support and GPA.
*   **Predictive Modeling:** Implementing a Random Forest Classifier to predict a student's `GradeClass` based on their habits.
*   **Feature Engineering:** Combining `Sports`, `Music` and `Volunteering` into a single "Engagement Score".

---

## 📂 File Structure
*   `Student_performance_data _.csv`: Raw dataset.
*   `analysis.ipynb`: The main notebook containing the Python code and visualisations.
*   `README.md`: Project documentation.
