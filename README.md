# 🚲 Bike Sharing Demand Prediction using Machine Learning

This project aims to predict daily bike rental demand using machine learning regression techniques based on historical rental, seasonal, and weather-related data.

The analysis follows a structured machine learning workflow consisting of data preprocessing, visualization, model development, training, evaluation, and hyperparameter optimization to build an accurate demand prediction model.

---

## 📊 Dataset

* Source: Bike Sharing Dataset (UCI Machine Learning Repository)
* Type: Tabular data
* Target: `cnt` (Total Bike Rentals)

### Features

The dataset contains daily records of bike rental activity, including:

* Season
* Year
* Month
* Holiday
* Weekday
* Working Day
* Weather Situation
* Temperature
* Feeling Temperature
* Humidity
* Wind Speed
* Casual Rentals
* Registered Rentals

---

## ⚙️ Project Workflow

### 1. Import Dataset & Library

* Import required libraries for data analysis and machine learning
* Load the dataset into a Pandas DataFrame
* Inspect the dataset structure and basic information

### 2. Data Preprocessing

* Check missing values and data consistency
* Remove irrelevant feature (`instant`)
* Remove leakage features (`casual` and `registered`)
* Convert `dteday` into datetime format
* Set the date column as the dataframe index

### 3. Data Visualization

* Visualize weekly bike rental trends
* Analyze monthly and quarterly demand patterns
* Explore feature distributions using pair plots
* Analyze feature correlations using a heatmap

### 4. Build Model

* Apply One-Hot Encoding to categorical variables
* Combine encoded categorical and numerical features
* Separate features (X) and target variable (y)
* Split the dataset into training and testing sets

### 5. Training & Evaluation

* Train XGBoost regression models using different parameter configurations
* Compare model performance across different maximum tree depths
* Evaluate models using:

  * R² Score
  * RMSE
  * MSE
  * MAE

### 6. HyperParameter Tuning

* Optimize model performance using:

  * Grid Search
  * Random Search
  * Bayesian Optimization
* Compare optimization strategies to obtain the best-performing model

---

## 🧠 Key Concept

This project demonstrates:

* End-to-end **Machine Learning pipeline**
* **Regression modeling using XGBoost**
* **Demand prediction**
* **Hyperparameter optimization**
* **Performance evaluation using multiple regression metrics**

---

## 📈 Results

* Successfully developed an XGBoost regression model for predicting daily bike rental demand.
* Compared multiple XGBoost configurations to evaluate model performance.
* Applied multiple hyperparameter optimization techniques to improve prediction accuracy.

---

## 🛠️ Tech Stack

* Python
* NumPy
* Pandas
* Scikit-learn
* XGBoost
* Scikit-Optimize
* Matplotlib
* Seaborn

---

## 📌 Future Improvements

* Compare XGBoost with additional regression models (Linear Regression, Random Forest, LightGBM, etc.)
* Perform feature importance analysis
* Add model explainability using SHAP
* Deploy the model as an interactive web application
* Evaluate model performance on additional datasets

---

## 👤 Author

* GitHub: [husnindz](https://github.com/husnindz)
