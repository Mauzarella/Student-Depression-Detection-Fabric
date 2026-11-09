🧠 Student Depression Detection - End-to-End Microsoft Fabric Project

📌 Project Overview

This project leverages Microsoft Fabric to build an end-to-end data pipeline predicting student depression based on academic, social, and demographic factors. Utilizing a Medallion Lakehouse architecture, the data is ingested, cleansed, and modeled to train a classification algorithm, ultimately feeding into a Power BI dashboard for business insights.

Dataset: Kaggle Student Depression Detection Dataset

🏗️ Architecture & Tech Stack

Platform: Microsoft Fabric

Data Engineering: PySpark, Delta Lake (Bronze ➔ Silver ➔ Gold)

Machine Learning: Scikit-Learn / PySpark MLlib, MLflow (Experiment tracking)

Visualization: Power BI

🚀 Project Workflow

1. Ingestion (Bronze Layer)

Uploaded raw CSV data into a Fabric Lakehouse.

Stored as raw Delta Parquet tables for immutable history.

2. Transformation (Silver Layer)

Created Spark Notebooks to clean the data.

Standardized categorical variables (e.g., One-Hot Encoding for Family_background, Living_style).

Imputed missing values and binned numerical features like CGPA.

3. Machine Learning & Modeling (Gold Layer)

Utilized Fabric's Data Science workspace.

Trained a classification model (Random Forest/Logistic Regression) to predict the Depression target variable.

Tracked model performance metrics (Accuracy, F1-Score) using MLflow.

Outputted a final aggregated Gold table for reporting.

4. Power BI Dashboard

Connected Power BI directly to the Lakehouse SQL Analytics Endpoint.

Built interactive visuals to identify key influencers of depression, such as Health_condition, Current_semester, and CGPA.

📁 Repository Contents

/notebooks: Contains the PySpark notebooks used for data transformation and model training.

/reports: Screenshots and PDF exports of the Power BI Dashboard.

/data: Data dictionary and dataset link.

💡 Key Insights

(Add 2-3 bullet points here once you finish your Power BI dashboard. E.g., "Students with 'Critical' health conditions and a CGPA below 3.0 showed a 40% higher likelihood of depression.")

Step 5: Commit and Push

If you are doing this via the GitHub website:

Click Add file > Upload files.

Drag and drop your downloaded .ipynb notebooks and dashboard screenshots into the correct folders.

Write a commit message (e.g., "Initial commit: Added data cleaning notebook and README template") and click Commit changes.
