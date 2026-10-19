# Project Brief
## Laboratory Data Quality Assessment and Exploratory Analysis Using Python

### Client
A private diagnostic laboratory is preparing an internal report from a historical dataset of routine laboratory measurements. The laboratory wants an initial assessment of data quality and a concise exploratory analysis before using the dataset for further statistical work.

### Objective
Clean and assess the dataset, summarize the main variables, investigate relationships between selected laboratory measurements, and prepare clear visualizations suitable for a professional report.

### Source data
The supplied Excel file contains synthetic patient-level laboratory records created specifically for this portfolio project. It intentionally includes realistic data-quality issues so the analyst can demonstrate cleaning and validation skills.

### Deliverables
1. A cleaned dataset in Excel format.
2. A Jupyter Notebook containing the complete Python workflow.
3. A concise exploratory-analysis report (PDF or HTML).
4. Clear, publication-style charts.
5. A short README explaining the project, methods, assumptions, and limitations.

### Required analysis

#### A. Data quality
- Inspect the dataset structure and data types.
- Identify missing values and report their frequency.
- Identify exact duplicate records.
- Check categorical consistency in Sex and Diabetes.
- Identify physiologically implausible or clearly invalid values.
- Document every cleaning decision.
- Do not silently delete observations.

#### B. Descriptive analysis
For Age, BMI, Glucose, HbA1c, Total Cholesterol, LDL, HDL, Triglycerides, Systolic BP, and Diastolic BP:
- Calculate appropriate descriptive statistics.
- Summarize categorical variables with counts and percentages.
- Compare key laboratory variables between males and females.

#### C. Exploratory visualization
Create appropriate charts to investigate:
- Distribution of age.
- Distribution of BMI.
- Distribution of glucose.
- Distribution of LDL and HDL.
- Sex differences in selected laboratory variables.
- Relationship between BMI and glucose.
- Relationship between triglycerides and HDL.
Choose the chart type based on the question rather than using the same chart for everything.

#### D. Findings
Write a concise summary of:
- Important data-quality problems.
- Major descriptive patterns.
- Any notable relationships visible in the data.
- Limitations of drawing clinical conclusions from this dataset.

### Technical requirements
- Python
- Pandas
- NumPy
- Matplotlib
- Clean, readable code with comments where useful.
- Reproducible workflow.
- No manual editing of the raw dataset.

### Important
This is an exploratory data-analysis task, not a clinical diagnostic task. Do not make medical diagnoses or causal claims from the data.

### Success criteria
The final work should be understandable to a non-programming client, reproducible by another analyst, and polished enough to be presented as a freelance data-analysis portfolio project.
