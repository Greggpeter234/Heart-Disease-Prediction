# ![My logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

# HEART DISEASE PREDICTION 

## Overview
-- This project uses a real world clinical datasets from UCI Library to predict the presence of heart disease in patients using Exploratory Data Analysis (EDA), Hypothesis Testing and Logistic Regression Model. The workflow is to perform an ETL (Extract, Transform, Load), create visualizations using Python and associated libraries such as matplotlib, seaborn for static visualisations and plotly was also used to create interactive visualisation. Carry out Hypothesis Testing and Logistic regression Model to predict a Target Variable (Presence of Heart Disease) among various features.



## Project Objectives

- Understand the relationships between various clinical features and heart disease.
- Perform statistical hypothesis testing to validate significant variables
- Build and evaluate a logistic regression model to predict the likelihood of a heart disease.

## Workflow and Tasks

- **Extract** data from a CSV file
- **Transform** the data using cleaning and preprocessing techniques
- **Load** the data into a pandas DataFrame for analysis
- Perform **exploratory data analysis (EDA)**
- Perform Hypothesis Testing
- Create visualizations using **matplotlib**, **seaborn** and **plotly**
- Export cleaned heart_disease datasets to Power BI
- Create 4 advanced visualizations and Dashboard on Power BI

## Technologies Used

- Python 3.12.8
- pandas
- matplotlib
- seaborn
- plotly
- ScikitLearn
- NumPy
- Power BI
- Jupyter Notebook
- Git & GitHub
- vs code
## Datasets

The dataset used is a CSV file containing clinical data from UCI Heart Disease Library. The original data was collected from 4 Locations:
 - 1. Cleveland Clinic Foundation (cleveland.data)
 - 2. Hungarian Institute of Cardiology, Budapest (hungarian.data)
 - 3. V.A. Medical Center, Long Beach, CA (long-beach-va.data)
 - 4. University Hospital, Zurich, Switzerland (switzerland.data)

The original databases have 76 raw attributes or features, only 14 of them are actually used and i only used 13 of the features aside the target variable. Thus I've taken the liberty of making 2 copies of each datasets and loaded them on jupiter notebook. The authors of the datasets have made request that any publications resulting from the use of the data include the names of the principal investigator responsible for the data collection at each institution.  They would be:
 - 1. Hungarian Institute of Cardiology. Budapest: Andras Janosi, M.D.
 - 2. University Hospital, Zurich, Switzerland: William Steinbrunn, M.D.
 - 3. University Hospital, Basel, Switzerland: Matthias Pfisterer, M.D.
 - 4. V.A. Medical Center, Long Beach and Cleveland Clinic Foundation:
	  Robert Detrano, M.D., Ph.D.

- **Source**: [UCI Heart Disease Dataset] (https://archive.ics.uci.edu/dataset/45/heart+disease) or from Kaggle equivalent.
- **Target Variable**: 'target' -- 1 (disease present), 0 (no disease)
- **Clinical features**:
Data columns (total 14 columns):
 # Column                Datatype              Description
  
 - 1  age                numeric                Age in Years
 - 2  sex                category (binary)      1 = Male 0 = Female
 - 3  chest pain type    category (Ordinal)     4 Values(-- 1 = typical angina, 
                                                         -- 2 = atypical angina, 
                                                          -- 3 = non-anginal pain, 
                                                         -- 4 = asymptomatic pain)
 - 4 resting systolic bp  numeric               Resting blood pressure (in mm Hg on admission to the hospital
 - 5 cholesterol          numeric               serum cholesterol in mg/dl

 - 6 fasting blood sugar  category (binary)          fasting blood sugar > 120 mg/dl)  (1 = true; 0 = false)
 - 7 resting ECG          category (ordinal)             3 Values (resting electrocardiographic results 
                                                0 = normal,                                                       1 = having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of >0.05mV)
                                                2 = showing probable or definite LVH

 - 8 max heart rate        numeric            maximum heart rate achieved
 - 9  exercise angina      category (binary)  exercise induced angina (1 = yes; 0 = no)
 - 10 ST depression        category           ST depression induced by exercise relative to rest 
                                                 (1 = present, 0 = not present)
 - 11 ST slope             category           the slope of the peak exercise ST segment, 3 Values
                                               (1 = up-sloping, 2 = flat or normal, 3 = down-sloping)
 - 12 hypertension         category           hypertension (1 = hypertensive, 0 = non-hypertensive)
 - 13 family history       category           family history of coronary artery disease (1 = yes; 0 = no)
 - 14 target               category           heart disease (1 = presence, 0 = absence)




## Key Findings
- 
-
- 


## Project Structure

3. Open heart_disease_prediction.ipynb` in Jupyter Notebook in VS Code IDE.
4. Run the notebook cells to follow the ETL workflow and view the visualizations.

## Key Steps

1. **Extract:** Load the CSV data using pandas.
2. **Transform:** Clean missing values, check data types, and preprocess as needed.
3. **Load:** Store the cleaned data in a DataFrame.
4. **Visualize:** Generate plots to explore relationships and trends in the data.

## Agile Methodothology
This is a collaborative and sustainable way of managing projects by breaking the work into small, manageable tasks, delivering results step by step, and improving tasks based on regular feedbacks (Beck, K., et al.(2001). Manifesto for Agile Software Development. [https://agilemanifesto.org]

## User Story
As a student Data Analyst, I want to build an ETL pipeline to extract, clean, transform, and load heart_disease_prediction data (including features such as age, sex, BMI, family size, smoking habits, and geographic region) from Kaggle, so that I can perform analysis, create and generate reports on how personal and geographic factors influence insurance costs.

## Tasks

1. **Extract Data**  
   - Download and extract healthcare insurance data from Kaggle (CSV format) [https://www.kaggle.com/datasets/willianoliveiragibin/healthcare-insurance]
2. **Clean Data**  
   - Handle missing values (impute or drop as appropriate).
   - Normalize data types and ensure correct formatting of all fields.
3. **Transform Data**  
   - Apply business logic to create derived columns (e.g., BMI category).
   - Encode categorical variables for analytics.
4. **Load Data**  
   - Load the cleaned and transformed data into a Pandas DataFrame.
5. **Validate & Visualize Data**  
   - Check data quality and consistency (duplicates, nulls, ranges).
   - Perform descriptive statistics and correlation analysis.
   - Visualize insights, predictive models, and the impact of geographic regions.

## Acceptance Criteria

### 1. Data Extr+=action
- 1 The pipeline shall extract raw data from Kaggle and UCI repository in CSV format, including features: age, sex, chest pain type, resting systolic bp, cholesterol, fasting blood sugar, resting ECG, maximum heart rate during exercise, exercise angina, ST depression, ST slope, hypertension, family history of coronary artery disease and the target variabe of heart disease presence or absence.
- 2 The extraction process must log missing or duplicate records and report extraction success/failure.

### 2. Data Transformation
- 1 The pipeline shall clean data by removing duplicates, handling missing values, and standardizing field formats (e.g., sex as ‘Male’/‘Female’).
- 2 Categorical variables must be encoded for downstream analytics..

### 3. Data Loading
- 1 The data shall be loaded into a Pandas DataFrame following a pre-defined schema.
- 2 The loading process must be IDE potent, preventing duplicate entries.
- 3 The pipeline must validate and log each load, including row counts and data checksums.

### 4. Data Quality & Integrity
- 1 The pipeline shall include automated data quality checks (e.g., null checks, referential integrity) and alert on anomalies.
- 2 All transformation steps must be documented and auditable.
- 
### 5. Security & Compliance
- 1 Sensitive data must be handled in compliance with data privacy regulations (e.g., HIPAA, GDPR).
- 2 Access to data must be restricted and audit-logged.

### 6. Documentation & Monitoring
- 1 The ETL process shall be documented with setup, configuration, and troubleshooting instructions.
- 2 The pipeline must include monitoring and alerting for failures or significant data anomalies.

## Additional Requirements for Analysis & Reporting

- The pipeline must enable:
- Descriptive statistics.
- Correlation and visualisation reports between clinical features and heart disease risk.
- Visualization.


## Visualizations
- Distribution of insurance charges
- Correlation heatmaps
- Age vs. charges scatter plots
- Categorical comparisons (e.g., smoker vs. non-smoker)
- Gegographic factors in relation to healthcare insurance cost [https://greggpeter234.github.io/Individual_Project-1/]
  
## Credits
- Hungarian Institute of Cardiology. Budapest: Andras Janosi, M.D.
- University Hospital, Zurich, Switzerland: William Steinbrunn, M.D.
- University Hospital, Basel, Switzerland: Matthias Pfisterer, M.D.
- V.A. Medical Center, Long Beach and Cleveland Clinic Foundation: Robert Detrano, M.D., Ph.D.
- GitHub copilot for code correction, review and explanation
- Chatgpt for code research and context.
- Professional definition for Agile methodology. Beck, K., et al.(2001). Manifesto for Agile Software Development. [https://agilemanifesto.org]
- UCI data repository


## Acknowledgements
- UCI Machine Learning Repository and authors and collectors of this datasets already credited for their remarkable and profound work
- Kaggle community and everyone in the community that i made research from on the use of this datasets
- My partner who provided support and understanding through out my journey through this project.
- My instructors and fellow bootcamp mates at code institute who have been very supportive and helpful through out my journey.


---

*Created as part of my Data Analytics bootcamp Capstone Project!*

- 
