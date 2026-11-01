# crop_yield_prediction
Project Overview
This project aims to build a robust machine learning pipeline to predict agricultural crop yields (hg/ha_yield) based on environmental and operational factors. By merging multiple datasets containing climate metrics, chemical usage, and historical records, we can analyze what drives crop productivity across different regions and crop types.

Dataset Origin & Components
The dataset is constructed by combining four primary data sources:
yield.csv: Historical crop production and yield records across various countries.
rainfall.csv: Annual average rainfall measurements (mm per year) by region.
temp.csv: Average annual temperature records by country/region.
pesticides.csv: Total pesticide tonnage used in agricultural production.

Feature Descriptions
Area: The country or region where the crop is grown (Categorical).
Item: The specific type of crop being cultivated, such as potatoes, maize, wheat, etc. (Categorical).
Year: The chronological year of the record (Numerical).
average_rain_fall_mm_per_year: Average annual rainfall in millimeters (Numerical).
avg_temp: Average recorded temperature in degrees Celsius (Numerical).
pesticides_tonnes: Total tonnes of pesticides applied (Numerical).
hg/ha_yield: Target Variable — Crop yield measured in hectograms per hectare.

Project Workflow
Data Preprocessing & Cleaning: Standardized column names, unified datasets through inner joins, removed duplicates, and handled missing values.
Exploratory Data Analysis (EDA): Visualized yield distributions, identified right-skewness, and analyzed feature relationships.
Feature Engineering & Transformation: Applied log transformation to fix target skewness and set up a ColumnTransformer for target encoding and feature scaling.
Model Training & Tuning: Trained and hyperparameter-tuned multiple regression models (Linear Regression, Decision Tree, Random Forest, and XGBoost) using GridSearchCV.
Evaluation: Compared models using  R2  Score, MAE, and RMSE on real-world scales, saving the best-performing pipeline.

Data Source & Files
You can download the raw data files (yield.csv, rainfall.csv, temp.csv, pesticides.csv) via this link https://www.kaggle.com/datasets/patelris/crop-yield-prediction-dataset
Evaluation: Compared models using R2 Score, MAE, and RMSE on real-world scales, saving the best-performing pipeline.
Data Source & Files
You can download the raw data files (yield.csv, rainfall.csv, temp.csv, pesticides.csv) via this link https://www.kaggle.com/datasets/patelris/crop-yield-prediction-dataset
