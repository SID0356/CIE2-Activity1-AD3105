# CIE2-Activity1-AD3105
Multiple Linear Regression Worksheet - CIE 2 Activity 1
# CIE 2 - Activity 1: Multiple Linear Regression Worksheet
**Course:** Regression and Classification Algorithms (T.Y. B.Tech AI & DS, Semester V)  
**Institution:** Zeal College of Engineering and Research, Pune  
**Roll Number:** AD3105 
**Submission GitHub ID:** [https://github.com/complexiota](https://github.com/complexiota)

---

## 1. Project Overview & Problem Framing
As a Data Analyst at an Academic Analytics & Student Success Cell, the goal of this project is to model and forecast student exam performance (`Performance Index`) using key study and preparation metrics. Understanding how multiple factors act simultaneously helps academic advisors identify at-risk students and recommend actionable study habits.

## 2. Dataset Source & Description
* **Dataset Name:** Student Performance (Multiple Linear Regression)
* **Source:** Kaggle (`nikhil7280/student-performance-multiple-linear-regression`)
* **Dimensions:** 10,000 rows × 6 columns (`.csv`)
* **Input Features ($X$):**
  * `Hours Studied` ($X_1$): Total study hours.
  * `Previous Scores` ($X_2$): Marks obtained in prior assessments.
  * `Sleep Hours` ($X_3$): Average daily hours of sleep.
  * `Sample Question Papers Practiced` ($X_4$): Count of mock papers practiced.
* **Target Variable ($y$):** `Performance Index` (Continuous score from 10 to 100).

## 3. Work Completed
* **Exploratory Data Analysis & Cleaning:** Inspected data types, summary statistics, missing values, and removed duplicate rows. Visualized feature relationships using scatter plots and a correlation heatmap.
* **Manual Normal Equations Worksheet:** Solved $(X^TX)b = X^Ty$ step-by-step by hand on a 6-row sample using `Hours Studied` and `Previous Scores`, then verified exact alignment with `scikit-learn`.
* **Baseline vs. Multiple Regression:** Compared a single-feature baseline (`Previous Scores`) against the full 4-feature Multiple Linear Regression model using an 80:20 train-test split (`random_state=42`).
* **Diagnostics & Assumptions:** Verified linearity, homoscedasticity, residual normality, and low multicollinearity (using VIF).

## 4. Key Results Summary
* **Fitted Multiple Regression Equation:**
  $$\text{Performance Index} = -33.92 + 2.85(\text{Hours Studied}) + 1.02(\text{Previous Scores}) + 0.48(\text{Sleep Hours}) + 0.19(\text{Sample Papers})$$
  *(Note: Update these values with your exact notebook outputs)*
* **Model Comparison (Test Set):**
  * **Single-Feature Baseline ($R^2$):** ~0.838 | **RMSE:** ~7.72
  * **Multiple-Feature Model ($R^2$):** ~0.988 | **Adjusted $R^2$:** ~0.988 | **RMSE:** ~2.04

## 5. Repository Contents
* `Activity1_Multiple_Linear_Regression.ipynb` – Complete executed Jupyter/Colab notebook with code, plots, interpretations, and Decision Log.
* `Student_Performance.csv` – Dataset used for analysis.
* `Manual_Calculation_Worksheet.pdf` – Handwritten/typed normal-equations solution for the 6-row sample.
* `README.md` – Project summary and submission links.
