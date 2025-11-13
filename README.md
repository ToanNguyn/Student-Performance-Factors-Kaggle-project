# Student Performance Analysis and Prediction

## Project Overview

This project analyzes a dataset of student exam scores to identify key factors influencing academic performance. The analysis involves data cleaning, in-depth exploratory data analysis (EDA), and the development of predictive models to forecast student scores.

A summary dashboard is also provided to visualize key findings and performance indicators.

## Dataset

The dataset (`StudentPerformanceFactors.csv`) contains 6607 student records with the following attributes:
* **Target Variable:** `Exam_Score`
* **Academic Factors:** `Hours_Studied`, `Attendance`, `Previous_Scores`, `Teacher_Quality`,`Tutoring_Sessions`, `Learning_Disabilities`
* **Home & Socio-Economic Factors:** `Parental_Involvement`, `Parental_Education_Level`, `Family_Income`, `Access_to_Resources`, `Internet_Access`, `Distance_from_Home`
* **Personal & Behavioral Factors:** `Extracurricular_Activities`, `Sleep_Hours`, `Motivation_Level`, `Peer_Influence`, `Physical_Activity`, `Gender`
* **School Factors:** `School_Type`

## Project Workflow

The project is structured in a Jupyter Notebook (`Student Performance Factors.ipynb`) and follows these key steps:

### 1. Data Cleaning and Preparation

* Checked for and handled missing values and duplicates.
* Standardized column names for consistency.

### 2. Exploratory Data Analysis (EDA)

Conducted in-depth EDA to understand the data distributions and relationships between variables:
* **Univariate Analysis:** Analyzed the distribution of individual features like gender, race/ethnicity, and parental education.
* **Bivariate Analysis:** Investigated the impact of various factors on exam scores, including:
    * School type vs. Scores 
    * Distance from home vs. Scores
    * Gender vs. Scores
    * School type vs. Access to resources
* **Correlation Analysis:** A heatmap was generated to visualize the strong positive correlation between variables.

### 3. Predictive Modeling

The goal was to predict the `Exam Score` based on the available features.
* **Preprocessing:** Categorical features were converted into numerical format using One-Hot Encoding.
* **Model Building:** Two different regression models were built and evaluated:
    1.  **Linear Regression**
    2.  **Lasso Regression**
* **Evaluation:** Models were assessed using metrics such as **R-squared (R2)**. A final comparison showed that all models performed similarly well, with high R2 scores.

### 4. Dashboard Visualization

A summary "Student Performance Analysis" dashboard (`Dashboard.pdf`) was designed to present the key findings in an accessible format.
* **Key KPIs:** Includes total students, gender distribution, and average/min/max scores.
* **Key Insights:** Features visualizations that show the relationship between scores and factors like gender, parental education, school type and test preparation.
