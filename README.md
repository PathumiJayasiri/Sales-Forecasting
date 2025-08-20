

# 📊 Sales Forecasting with Linear Regression

## 📌 Overview

Dataset: train.csv (contains store, item, sales, and date)

Objective: Forecast monthly customer sales

Models Used:

Linear Regression (LR)

(Future scope: Random Forest, XGBoost, LSTM)

Metrics:

Root Mean Squared Error (RMSE)

Mean Absolute Error (MAE)

R² Score
---

## 🛠️ Technologies Used

* **Python 3**
* **Pandas** – Data handling
* **NumPy** – Numerical operations
* **Scikit-learn** – Machine Learning (Linear Regression & metrics)
* **Matplotlib / Seaborn** – Data visualization

---

## 📂 Project Structure

```
Sales-Forecasting/
│-- train.csv                 # Dataset (CSV or Excel file)
│-- sales_forecasting.ipynb  # Jupyter Notebook with implementation
│-- README.md             # Project documentation
```

---

## 🚀 Steps in the Project

1. **Import Libraries**
   Load necessary Python libraries for data handling, visualization, and modeling.

2. **Load Dataset**
   Use Pandas to read sales data (e.g., monthly or daily sales).

3. **Exploratory Data Analysis (EDA)**

   * Check missing values
   * Plot sales trends
   * Identify correlations

4. **Preprocessing**

   * Select features (X) and target (y)
   * Train-test split

5. **Model Training (Linear Regression)**

   * Train the Linear Regression model on training data.

6. **Prediction & Evaluation**

   * Predict sales on test data.
   * Evaluate model performance using:

     * ✅ Mean Squared Error (MSE)
     * ✅ Mean Absolute Error (MAE)
     * ✅ R² Score

7. **Visualization**

   * Plot **Actual vs. Predicted Sales** to visually analyze performance.

---

## 📈 Example Evaluation Metrics

* **Mean Squared Error (MSE):** Measures average squared difference between actual and predicted values.
* **Mean Absolute Error (MAE):** Measures average absolute difference.
* **R² Score:** Explains how well the model fits the data (closer to 1 is better).

---

## 📊 Sample Output (Visualization)

plt.figure(figsize=(15, 5))
plt.plot(monthly_sales['date'],monthly_sales['sales'])
plt.plot(predict_df['date'], predict_df['Linear Prediction'])
plt.title('Customer sales forecast using LR model')
plt.xlabel('Date')
plt.ylabel('Sales')
plt.legend(['Actual Sales','Predicted Sales'])
plt.show()

<img width="1233" height="470" alt="Customer sales forecast using LR model" src="https://github.com/user-attachments/assets/85df95b1-79b8-4771-807a-0c6523e57218" />


## ✅ Results

The Linear Regression model provides a baseline approach to sales forecasting.

* **Strengths:** Simple, interpretable, fast.
* **Limitations:** Assumes linearity; may not capture seasonal patterns or complex trends.

---

## 🔮 Future Improvements

* Add **Polynomial Regression** or **Random Forest** for better accuracy.
* Use **Time Series Models** (ARIMA, Prophet, LSTM).
* Apply **Feature Engineering** (holidays, promotions, seasonality).

---

## 📜 License

This project is open-source and free to use for educational purposes.

