# Air Quality Index (AQI) Prediction

## 📌 Project Overview
This project aims to predict the Air Quality Index (AQI) using historical air pollution data. We use machine learning techniques in Python to analyze air quality data and build predictive models. The dataset includes various pollutants such as PM2.5, PM10, NO2, NOx, NH3, CO, SO2, O3, Benzene, and Toluene, collected from multiple cities.

## 📂 Dataset
The dataset used for this project is named **"air quality data.csv"** and contains information on air pollutants of a specific time period. Some key points about the dataset:
- Xylene has the highest percentage of missing values (61.86%)
- PM10 and NH3 have missing values around 28 and 26%
- The target variable is **AQI (Air Quality Index)**

## 🚀 Project Workflow
The project is structured into the following key steps:
1. **Data Preprocessing:**
   - Load dataset and analyze missing values.
   - Handle missing values by replacing them with the mean of the respective columns.
   - Remove irrelevant features such as `Date` and `City`.

2. **Exploratory Data Analysis (EDA):**
   - Univariate analysis: Distribution of individual features (Xylene, PM10, NH3, Benzene, NOx, etc.) using histograms.
   - Bivariate analysis:
     - Count plots for `City` and `AQI_Bucket`
     - Box plots to visualize the distribution of different pollutants across cities
     - Distribution of AQI over the time period

3. **Data Cleaning and Preprocessing:**
   - Handle missing values by replacing them with the mean of the respective feature.
   - Perform data scaling using **StandardScaler** to normalize feature values.
   - Outlier detection and removal using the **IQR method**.

4. **Model Training & Evaluation:**
   - Implemented different regression models:
     - **Linear Regression**
     - **K-Nearest Neighbors (KNN)**
     - **Decision Trees**
     - **Random Forest Regressor**
   - The models were evaluated using:
     - **Root Mean Squared Error (RMSE)**
     - **R-squared (R²) score**

## 🚀 Technologies Used
- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Scikit-Learn

