

# 🚗 Car Price Prediction — Machine Learning Project

## 📌 Overview

The price of a car depends on various factors such as brand value, fuel type, car age, transmission, and mileage. Predicting car prices accurately can help both buyers and sellers make better financial decisions.

This project demonstrates how to **build and evaluate machine learning models** for predicting car prices using **Python, Scikit-learn, and Plotly** in Google Colab.

---

## 📂 Dataset

* Source: `car data.csv`
* Features:

  * `Present_Price`: Current showroom price (in lakhs)
  * `Driven_Kms`: Total kilometers driven
  * `Owner`: Number of previous owners
  * `Car_Age`: Derived from year of purchase (newer cars have lower age)
  * `Fuel_Type`: Petrol / Diesel / CNG
  * `Selling_Type`: Dealer / Individual
  * `Transmission`: Manual / Automatic
* Target:

  * `Selling_Price`: Resale value of the car (in lakhs)

---

## 🔎 Exploratory Data Analysis (EDA)

* Distribution of Selling Price
* Relationship between Present Price & Selling Price
* Selling Price vs Fuel Type
* Driven Kms vs Selling Price by Transmission

Interactive **Plotly visualizations** were used for better insights.

---

## 🛠️ Modeling

* **Preprocessing**:

  * StandardScaler for numeric features
  * OneHotEncoding for categorical features
* **Models trained**:

  * Linear Regression
  * Random Forest Regressor

---

## 📊 Model Evaluation

### Linear Regression

* MAE: **1.216**
* RMSE: **1.866**
* R² Score: **0.849 (84.89%)**
* MAPE: **80.30%**
* Accuracy: **19.70%**

### Random Forest Regressor

* MAE: **0.619**
* RMSE: **0.948**
* R² Score: **0.961 (96.10%)**
* MAPE: **16.80%**
* Accuracy: **83.20%**

✅ **Random Forest outperformed Linear Regression significantly**.

---

## 🔑 Feature Importance (Random Forest)

* **Present Price**: 88.6% (most influential)
* **Car Age**: 5.7%
* **Driven Kms**: 3.3%
* Transmission, Fuel Type, and Selling Type had minor contributions.

---

## 📈 Insights

* Petrol cars generally have lower resale value than diesel.
* Older cars show a sharp decline in selling price.
* Present Price is the most dominant factor in predicting resale value.

---

## 🚀 Tech Stack

* Python 🐍
* Pandas, NumPy
* Scikit-learn
* Plotly (interactive visualizations)

---

## 📌 Conclusion

* **Random Forest** achieved **83.2% accuracy** and is the preferred model for predicting car prices.
* Feature importance reveals that **Present Price** is the key driver of resale value.



