# 🍔 Food Delivery Time Prediction

## 📌 Project Overview

This project focuses on analyzing and predicting food delivery times using real-world features such as distance, traffic conditions, weather, and courier experience.

The objective is to:

* Perform **data cleaning & preprocessing**
* Conduct **Exploratory Data Analysis (EDA)**
* Extract insights using **SQL queries**
* Prepare data for **Machine Learning models**

---

## 🔗 Dataset Source

Dataset used in this project is from Kaggle:

👉 https://www.kaggle.com/datasets/denkuznetz/food-delivery-time-prediction/data

---

## 📂 Features in Dataset

* `Distance_km` → Distance between restaurant and delivery location
* `Weather` → Weather conditions
* `Traffic_Level` → Traffic intensity
* `Time_of_Day` → Morning / Afternoon / Evening / Night
* `Courier_Experience_yrs` → Experience of delivery agent
* `Vehicle_Type` → Scooter / Bike / Car
* `Preparation_Time_min` → Time taken to prepare food
* `Delivery_Time_min` → Target variable

---

## 🧹 Data Cleaning

* Checked and removed duplicate records
* Handled missing values:

  * Categorical columns → Filled with **mode**
  * Numerical columns → Filled with **median**
* Ensured dataset consistency

---

## 📊 Exploratory Data Analysis (EDA)

### Analysis Performed:

* Distribution of delivery time
* Distance vs delivery time relationship
* Traffic impact on delivery
* Time of day influence
* Courier experience effect
* Vehicle type comparison

### 📈 Key Insights:

* Longer distances increase delivery time
* High traffic significantly delays orders
* Experienced couriers deliver faster
* Peak hours (evening/night) show higher delays

---

## 🔥 Correlation Analysis

* Used **Spearman correlation matrix**
* Observed strong relationships:

  * Distance ↔ Delivery Time
  * Traffic ↔ Delivery Time

---

## 🗄️ SQL Analysis

Performed analysis using in-memory SQLite:

* Average delivery time per traffic level
* Peak delay times based on time of day
* Distance category impact (Short / Medium / Long)

---

## ⚙️ Tech Stack

* Python 🐍
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SQLite

---

## 🚀 How to Run

```bash
# Clone the repository
git clone <your-repo-link>

# Install dependencies
pip install pandas numpy matplotlib seaborn

# Run the notebook
jupyter notebook Food_Delivery_.ipynb
```

---

## 📌 Future Improvements

* Build Machine Learning models (Regression)
* Improve prediction accuracy
* Deploy as a web application
* Add real-time delivery prediction system

---

## 💡 Conclusion

This project demonstrates how data analysis can uncover patterns affecting delivery performance and help optimize logistics systems.

---

## ⭐ Support

If you found this project useful, give it a ⭐ on GitHub!
