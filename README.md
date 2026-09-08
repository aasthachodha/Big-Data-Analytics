# Big Data Analytics and Machine Learning for Road Accident Severity Prediction

## 📌 Project Overview

This project presents an end-to-end Big Data Analytics and Machine Learning system for analyzing road accident data and predicting accident severity.

The project integrates multiple road accident datasets containing collision, vehicle, and casualty information. PySpark is used for large-scale data processing, cleaning, integration, and feature engineering. A Random Forest Classifier is then used to predict accident severity.

The analytical and machine learning results are presented through an interactive Power BI dashboard.

### Project Pipeline

Raw Accident Data
↓
Data Loading using PySpark
↓
Data Cleaning
↓
Dataset Integration
↓
Feature Engineering
↓
Exploratory Data Analysis
↓
Random Forest Classification
↓
Model Evaluation
↓
Power BI Visualization


---

## 🎯 Objectives

The main objectives of this project are:

- Process large-scale road accident datasets using PySpark.
- Clean and integrate collision, vehicle, and casualty datasets.
- Perform exploratory analysis of accident patterns.
- Engineer meaningful temporal, vehicle, driver, road, and environmental features.
- Predict accident severity using a Random Forest Classifier.
- Evaluate the machine learning model using Accuracy and F1 Score.
- Identify important factors influencing accident severity.
- Develop an interactive Power BI dashboard for data exploration and result presentation.


---

## 📂 Datasets

The project uses three related road accident datasets:

### 1. Collision Dataset

Contains accident-level information such as:

- Accident date and time
- Accident severity
- Location
- Road type
- Speed limit
- Junction information
- Light conditions
- Weather conditions
- Road surface conditions
- Urban/Rural area

### 2. Vehicle Dataset

Contains vehicle and driver-related information such as:

- Vehicle type
- Vehicle manoeuvre
- Skidding and overturning
- Driver age
- Driver age band
- Driver sex
- Journey purpose
- Propulsion code

### 3. Casualty Dataset

Contains information related to casualties involved in accidents.

The datasets were integrated to provide a broader representation of accident events for analysis and machine learning.


---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming and data processing |
| Jupyter Notebook | Development environment |
| PySpark | Big Data processing |
| Spark MLlib | Machine Learning |
| Random Forest | Accident severity classification |
| Power BI | Interactive visualization |
| CSV | Dataset and prediction-result storage |


---

## 🔄 Data Processing

PySpark was used to process the accident datasets through the following stages:

### Data Loading

The raw CSV datasets were loaded into Spark DataFrames.

### Data Cleaning

The preprocessing stage included:

- Schema inspection
- Data type conversion
- Handling invalid values
- Handling missing values
- Coordinate validation
- Removal of problematic records

### Data Integration

Collision, vehicle, and casualty information was combined to create a dataset suitable for analytical processing and machine learning.


---

## ⚙️ Feature Engineering

Several additional features were created to improve analysis and model performance.

### Temporal Features

- Accident date
- Accident month
- Accident day
- Accident hour
- Day of week
- Time period
- Hour category
- Weekend flag

### Vehicle Features

- Vehicle type
- Vehicle manoeuvre
- Skidding and overturning
- Propulsion code

### Driver Features

- Age of driver
- Driver age group
- Age band of driver
- Sex of driver
- Journey purpose

### Road & Environmental Features

- Road type
- Speed limit
- Speed category
- Junction detail
- Junction control
- Light conditions
- Weather conditions
- Road surface conditions
- Urban/Rural area
- Trunk road flag

### Aggregate Features

- Number of vehicles
- Number of casualties

The target variable used for classification was accident severity.


---

## 🤖 Machine Learning

### Random Forest Classifier

A Random Forest Classifier was selected for accident severity prediction.

Random Forest was chosen because:

- It is suitable for classification problems.
- It can capture non-linear relationships between variables.
- It combines multiple decision trees to produce a more robust prediction.
- It works well with a mixture of accident, vehicle, driver, road, and environmental features.
- It provides feature-importance information that helps interpret the model.

### Machine Learning Workflow

```text
Engineered Features
        ↓
Feature Preparation
        ↓
Training / Testing Split
        ↓
Random Forest Classifier
        ↓
Severity Prediction
        ↓
Model Evaluation
