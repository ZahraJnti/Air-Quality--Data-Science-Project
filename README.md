# Air-Quality--Data-Science-Project
A code for data analyzing and visualizing data and some prediction models with airquality/AirQualityUCI.csv dataset.


---

## 📌 Author

**Zahra Jannati**  
*Data Science Enthusiast | 2024*

---

# 🌫️ Air Quality Analysis Project

This project focuses on analyzing and cleaning a dataset related to **air quality measurements**. The original data was sourced from the UCI Machine Learning Repository and contains various sensor readings (e.g., CO, NOx, NMHC) collected over time.

---

## 📁 Dataset
- **Name:** AirQualityUCI.csv
- **Source:** UCI Machine Learning Repository
- **Description:** Contains hourly averaged responses from an array of chemical sensors embedded in an air quality monitoring device.

---

## 📌 Objectives

- Load and explore the structure of the air quality dataset.
- Handle inconsistent or missing data (e.g., placeholders like `-200`).
- Preprocess, clean, and prepare the data for analysis or modeling.
- Identify and handle missing values using imputation and row removal.
- Detect and remove duplicates.
- (Optional future steps: Visualization and modeling.)

---

## 🔧 Key Steps Performed

### 1. Data Loading & Exploration
- Used `pandas` and `numpy` to load and inspect the dataset.
- Investigated missing values, summary statistics, and initial anomalies.

### 2. Data Cleaning
- Dropped irrelevant columns (`Unnamed: 15`, `Unnamed: 16`).
- Combined `Date` and `Time` into a new `DateTime` column.
- Replaced commas in numeric columns with periods for conversion.

### 3. Handling Missing & Invalid Data
- Replaced placeholder values (`-200`) with `NaN`.
- Visualized missing data using `matplotlib`.
- Used:
  - `SimpleImputer` (mean strategy) for numeric imputation.
  - `KNNImputer` for more accurate filling of sensor gaps.
- Dropped rows with too many nulls when necessary.

### 4. Data Type Corrections
- Converted appropriate columns to `float` or `datetime64`.

### 5. Duplicate Management
- Identified and removed duplicate rows to ensure data quality.

---

## 📦 Technologies Used

- Python
- Jupyter Notebook
- pandas, numpy
- matplotlib
- scikit-learn (`KNNImputer`, `SimpleImputer`)

---

## 📊 Results

By the end of preprocessing:
- All invalid and missing values were either handled or removed.
- Dataset is clean and ready for:
  - Visualization of air quality trends over time.
  - Predictive modeling (e.g., forecasting pollution levels).
  - Correlation analysis between chemical components.

---

## 🚀 Future Work

- Create detailed visualizations of pollution trends.
- Build a machine learning model to predict air quality index (AQI).
- Deploy as an interactive dashboard or API.

---

## 📁 Repository Structure

