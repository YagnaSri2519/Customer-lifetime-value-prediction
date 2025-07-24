#  Customer Lifetime Value (CLTV) Prediction

This project builds a machine learning model to predict **Customer Lifetime Value (CLTV)** based on historical purchase behavior. The goal is to identify high-value customers and enable targeted marketing strategies.

---

## Objective

Predict the **total value a customer will generate over their lifetime** using features like:

- Recency of purchase
- Frequency of orders
- Average Order Value (AOV)

---

##  Tools & Libraries

- Python 3.x
- Pandas, NumPy
- Scikit-learn (`sklearn`)
- Seaborn, Matplotlib
- Joblib (for saving the model)

---

## Dataset

The model uses **transaction-level purchase data**, which includes:

- `CustomerID`
- `InvoiceDate`
- `InvoiceNo`
- `Quantity`
- `UnitPrice`

From these, the following features are engineered:

| Feature     | Description                             |
|-------------|-----------------------------------------|
| Recency     | Days since the last purchase            |
| Frequency   | Total number of transactions            |
| AOV         | Average Order Value (total / frequency) |
| Monetary    | Total amount spent (target variable)    |

---

## 🧠 Model Details

- **Model Used**: Random Forest Regressor
- **Target Variable**: `Monetary` (proxy for LTV)
- **Metrics**:  
  - Mean Absolute Error (MAE)  
  - Root Mean Squared Error (RMSE)

---

