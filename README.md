# 🚗 Determining Car Specifications and Prices

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=for-the-badge&logo=plotly&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)

---

## 📌 Project Overview

This project develops a **Linear Regression** model to predict car prices by analyzing the correlation between physical specifications and engine performance. The project covers the full data science pipeline — from data cleaning and outlier handling to model evaluation — using **R² Score** and **Root Mean Squared Error (RMSE)** to ensure reliable and credible price estimates.

---

## 📂 Dataset

- **Source**: [Kaggle - Car Sales Dataset](https://www.kaggle.com/datasets/gagandeep16/car-sales)
- **File**: `Car_sales.csv`
- **Size**: 157 rows × 16 columns
- **Target Variable**: `Price_in_thousands` (Continuous numerical value in $1,000s)

### Features Description

| Feature | Type | Description |
|---|---|---|
| `Manufacturer` | categorical | Car brand/manufacturer name |
| `Model` | categorical | Car model name |
| `Sales_in_thousands` | float | Number of units sold (in thousands) |
| `__year_resale_value` | float | Estimated resale value after one year |
| `Vehicle_type` | categorical | Type of vehicle (Passenger / Car) |
| `Price_in_thousands` | float | **Target** — car price in $1,000s |
| `Engine_size` | float | Engine displacement in liters |
| `Horsepower` | float | Engine horsepower output |
| `Wheelbase` | float | Distance between front and rear axles (inches) |
| `Width` | float | Vehicle width (inches) |
| `Length` | float | Vehicle length (inches) |
| `Curb_weight` | float | Vehicle weight without passengers/cargo (tons) |
| `Fuel_capacity` | float | Fuel tank capacity (gallons) |
| `Fuel_efficiency` | float | Fuel efficiency (MPG) |
| `Power_perf_factor` | float | Combined power performance factor |

---

## 🔧 Project Workflow

```
Data Understanding → Data Preparation → EDA → Modelling (Linear Regression) → Evaluation → Price Prediction
```

### 1. 📊 Data Understanding
Exploring the structure and characteristics of the dataset, checking data types, and identifying missing values.

### 2. 🔧 Data Preparation
- Handling missing values in relevant columns
- Selecting features with the strongest correlation to price
- Preparing data for modelling

### 3. 📈 Exploratory Data Analysis (EDA)
Visualizing patterns and extracting insights from the data, including:
- Top 10 best-selling car models
- Price comparison of best-selling cars
- Horsepower ratings across models
- Identifying specifications of the target car to be produced

### 4. 🤖 Modelling — Linear Regression
- Separating features and target variable
- Splitting data into **training** and **testing** sets
- Building a Linear Regression model using Scikit-learn

### 5. 📏 Evaluation
Measuring model performance using:
- **R² Score** — measures how well the model explains variance in car prices
- **RMSE (Root Mean Squared Error)** — measures average prediction error in price units

### 6. 🔮 Price Prediction
Predicting the price of a car based on user-defined specifications (Engine size, Horsepower, Wheelbase, etc.)

---

## 📊 Key Findings from EDA

- **Ford dominates** the best-selling models, placing 5 cars (F-Series, Explorer, Taurus, Ranger, Focus) in the top 10
- **F-Series** leads overall sales with over 500,000 units, followed by Explorer and Camry
- **Explorer** tops the pricing chart among best-sellers at $31,930, while **Ranger** offers the most affordable option at $12,050
- Engine size and horsepower show strong positive correlation with price

---

## ✅ Model Performance

| Metric | Value |
|---|---|
| **R² Score** | 0.9711 |
| **RMSE** | 1.7115 |

> 📝 The model achieves a very high R² Score of **0.97**, indicating that ~97% of the variance in car prices is explained by the selected features. The RMSE of **~1.71** means predictions are off by approximately $1,710 on average.

---

## 🛠️ Tools & Libraries

| Library | Purpose |
|---|---|
| `pandas` | Data manipulation and analysis |
| `numpy` | Numerical computation |
| `plotly.express` | Interactive data visualization |
| `scikit-learn` | Machine learning (Linear Regression, train-test split, evaluation metrics) |

---

## 🚀 How to Run

1. **Clone this repository**
   ```bash
   git clone https://github.com/your-username/determining-car-specifications-and-prices.git
   cd determining-car-specifications-and-prices
   ```

2. **Install required libraries**
   ```bash
   pip install pandas numpy plotly scikit-learn
   ```

3. **Download the dataset** from [Kaggle](https://www.kaggle.com/datasets/gagandeep16/car-sales) and place `Car_sales.csv` in the project directory

4. **Open and run the notebook**
   ```bash
   jupyter notebook Determining_Car_Specifications_and_Prices.ipynb
   ```

---

## 📁 Project Structure

```
determining-car-specifications-and-prices/
│
├── Determining_Car_Specifications_and_Prices.ipynb   # Main notebook
├── Car_sales.csv                                      # Dataset (download from Kaggle)
└── README.md                                          # Project documentation
```

---

## 👤 Author

**Fathan Alfariel Adhyaksa**
- GitHub: [@fathan-alf](https://github.com/fathan-alf)
- LinkedIn: [fathan-alfariel](https://www.linkedin.com/in/fathan-alfariel)
