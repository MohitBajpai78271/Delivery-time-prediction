# 🚚 Delivery Time Prediction Model

Predict estimated delivery times for food orders using real-world inspired features like distance, traffic, time-of-day, and restaurant prep time. Built for operational efficiency in last-mile logistics systems such as Zomato or Swiggy.

---

## 🔍 Problem Statement

Timely delivery is crucial for customer satisfaction in the food delivery industry. This project aims to predict the Estimated Time of Arrival (ETA) for orders using machine learning regression models based on historical order data and real-time features.

---

## 🧠 Features Engineered

- **Geodesic Distance**: Haversine formula between restaurant and customer location  
- **Order Time Attributes**: Hour of day, day of week, rush-hour flags  
- **Weather Conditions**: Simulated weather (rainy, sunny, etc.)  
- **Restaurant Prep Time**: Based on order size/type  
- **Traffic Level**: Simulated or fetched via placeholder APIs  

---

## 🛠️ Tech Stack

- `Python`, `Pandas`, `NumPy`
- `Scikit-learn`, `XGBoost`, `RandomForestRegressor`
- `Streamlit` for interactive UI

---

## 📊 Model Performance

| Model               | MAE   | R² Score |
|--------------------|-------|----------|
| Linear Regression   | 7.8 min | 0.62     |
| Random Forest       | 5.1 min | 0.81     |
| XGBoost             | 4.3 min | 0.86     |

*XGBoost showed the best performance on unseen test data.*

---

## 💻 Streamlit Dashboard

Interactive dashboard for:
- Inputting order details (location, time, traffic, etc.)
- Viewing real-time ETA prediction
- Visualizing model performance with MAE, residuals, and feature importance

Launch with:
```bash
streamlit run app.py
