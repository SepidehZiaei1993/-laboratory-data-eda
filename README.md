# 🏥 Laboratory Data Quality Assessment & Exploratory Analysis

*A portfolio project demonstrating end-to-end EDA on synthetic patient laboratory data.*

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)


## 📋 Project Overview
This project performs a comprehensive data quality assessment and exploratory data analysis (EDA) on a synthetic patient-level laboratory dataset. The objective is to clean the data, summarize key variables, investigate relationships between selected laboratory measurements, and prepare clear, publication-style visualizations suitable for a professional internal report.

## 📁 Dataset Description
- **Source**: Synthetic patient-level laboratory records (provided as `laboratory_patient_data_raw.xlsx`).
- **Size**: ~500 patient records.
- **Features**: Demographics (`Age`, `Sex`, `BMI`), Laboratory measurements (`Glucose`, `HbA1c`, `Total Cholesterol`, `LDL`, `HDL`, `Triglycerides`, `Systolic BP`, `Diastolic BP`), and a binary target (`Diabetes`).
- **Known Issues**: The dataset intentionally contains realistic data-quality issues, including missing values, categorical inconsistencies, exact duplicates, and a few physiologically implausible outliers.

## 🛠️ Methodology
1. **Data Quality & Cleaning**:
   - Inspected data types and structure.
   - Standardized categorical variables (e.g., `Sex`).
   - Identified and removed exact duplicate records.
   - Flagged (but did not silently delete) physiologically implausible values based on standard clinical reference ranges.
   - Documented all cleaning decisions in a reproducible cleaning log.
2. **Descriptive Analysis**:
   - Calculated summary statistics (mean, median, std, quartiles) for all numeric variables.
   - Generated count and percentage distributions for categorical variables.
   - Compared key laboratory variables between Male and Female subgroups.
3. **Exploratory Visualization**:
   - Utilized histograms for univariate distributions.
   - Utilized side-by-side boxplots to compare distributions across sexes.
   - Utilized scatter plots to investigate bivariate relationships (e.g., BMI vs. Glucose, Triglycerides vs. HDL).

## ⚠️ Assumptions & Limitations
- This is an **exploratory data analysis (EDA)** task, not a clinical diagnostic tool. No medical diagnoses or causal claims are made.
- Missing values were handled contextually during analysis; however, if data is not Missing Completely at Random (MCAR), summary statistics may carry slight bias.
- The dataset is synthetic, meaning findings are for demonstration purposes only.

## 💻 How to Reproduce

### Prerequisites
- Python 3.8 or higher
- Jupyter Notebook or JupyterLab

### Installation Steps
1. Install the required Python packages using pip:
2. Navigate to the project folder in your terminal or command prompt.
3. Launch Jupyter Notebook:
4. Open the file `Patients data analysis-project notebook.ipynb` from the Jupyter interface.

5. Run all cells sequentially from top to bottom.

### Alternative: Using Anaconda
If you're using Anaconda:
1. Open Anaconda Navigator
2. Launch Jupyter Notebook
3. Navigate to your project folder
4. Open `Patients data analysis-project notebook.ipynb`
5. Run all cells

## 📦 Deliverables
1. `Patients-data-analysis-notebook.ipynb` - The complete, reproducible Python workflow.
2. `laboratory_patient_data_cleaned.xlsx` - The cleaned dataset (generated after running the notebook).
3. `data_cleaning_log.csv` - A transparent record of all data quality decisions.
4. `Exploratory-analysis_report.pdf` - A client facing report 
5. `README.md` - This file, explaining the project, methods, and limitations.

## 📊 Key Findings
- Identified and standardized categorical inconsistencies in the `Sex` column.
- Removed 3 exact duplicate records.
- Flagged physiologically implausible values for review.
- Identified strong correlations between Total Cholesterol and LDL (r ≈ 0.916).
- Observed expected biological patterns (e.g., higher HDL in females, higher triglycerides in males).
- Visualized the positive relationship between BMI and Glucose levels.

## 🔧 Technologies Used
- Python 3.x
- Pandas (data manipulation)
- NumPy (numerical computing)
- Matplotlib (visualization)
- Seaborn (statistical visualization)
- Jupyter Notebook (interactive development)
