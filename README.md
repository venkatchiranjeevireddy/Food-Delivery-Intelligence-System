# 🍔 Food Delivery Time Prediction System

## 📌 Project Overview

This project focuses on analyzing and predicting food delivery time using real-world factors such as distance, traffic conditions, weather, and courier experience.

The goal of this project is to:

* Perform **data cleaning and preprocessing**
* Conduct **Exploratory Data Analysis (EDA)**
* Extract insights using **SQL queries**
* Build and evaluate **Machine Learning models**
* Derive **business insights for delivery optimization**

---

## 🔗 Dataset Source

Dataset used in this project:

👉 https://www.kaggle.com/datasets/denkuznetz/food-delivery-time-prediction/data

---

## 📂 Features in Dataset

* `Distance_km` → Distance between restaurant and delivery location
* `Weather` → Weather conditions
* `Traffic_Level` → Traffic intensity
* `Time_of_Day` → Morning / Afternoon / Evening / Night
* `Courier_Experience_yrs` → Experience of delivery agent
* `Vehicle_Type` → Scooter / Bike / Car
* `Preparation_Time_min` → Food preparation time
* `Delivery_Time_min` → 🎯 Target variable

---

## 🧹 Data Cleaning & Preprocessing

* Checked and removed duplicate records
* Handled missing values:

  * Categorical features → filled using **mode**
  * Numerical features → filled using **median**
* Converted categorical variables using **one-hot encoding**
* Prepared dataset for machine learning pipeline

---

## 📊 Exploratory Data Analysis (EDA)

### Analysis Performed:

* Distribution of delivery time
* Distance vs delivery time relationship
* Impact of traffic levels
* Effect of time of day (peak hours)
* Courier experience vs delivery performance
* Vehicle type comparison

### 📈 Key Insights:

* Delivery time increases with **distance**
* **High traffic** significantly increases delays
* **Peak hours (evening/night)** show maximum delivery time
* More experienced couriers reduce delivery variability

---

## 🔥 Correlation Analysis

* Used **Spearman correlation matrix**
* Observed strong relationships:

  * Distance ↔ Delivery Time
  * Traffic Level ↔ Delivery Time

---

## 🗄️ SQL-Based Analysis

Performed analysis using in-memory SQLite:

* Average delivery time by traffic level
* Peak delay analysis based on time of day
* Distance-based categorization (Short / Medium / Long)

These insights were later validated using machine learning models.

---

## 🤖 Machine Learning Modeling

### Models Used:

* Linear Regression (**Baseline Model**)
* XGBoost Regressor (with hyperparameter tuning)
* LightGBM Regressor (with hyperparameter tuning)

### 📊 Evaluation Metrics:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)

### 📈 Results:

| Model             | MAE  | RMSE |
| ----------------- | ---- | ---- |
| Linear Regression | 6.13 | 9.05 |
| XGBoost           | 6.75 | 9.55 |
| LightGBM          | 6.75 | 9.74 |

### 🧠 Key Observation:

* Linear Regression outperformed advanced models, indicating **strong linear relationships** between features and delivery time
* Tree-based models did not provide additional improvement for this dataset

---

## 📌 Feature Importance & Insights

* Most important features influencing delivery time:

  * Distance
  * Traffic Level
  * Time of Day

### 💡 Business Insights:

* Reducing delivery distance and optimizing routes can improve efficiency
* Managing peak-hour traffic is critical for reducing delays
* Assigning experienced couriers can improve delivery performance

---

## ⚙️ Tech Stack

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* LightGBM
* SQLite

---

## 🚀 How to Run

```bash
# Clone the repository
git clone <your-repo-link>

# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn xgboost lightgbm

# Run the notebook
jupyter notebook Food_Delivery_.ipynb
```

---

## 🔮 Future Improvements

* Perform advanced feature engineering
* Try ensemble models (stacking/blending)
* Build real-time prediction API using FastAPI
* Deploy as a web application
* Integrate live traffic APIs for real-world usage

---

## 💡 Conclusion

This project demonstrates how data analysis and machine learning can be used to understand and optimize delivery operations.

It highlights that:

* Simpler models can outperform complex models when relationships are linear
* Data-driven insights can significantly improve business decisions

---

## ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub!
