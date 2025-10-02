# Amazon Delivery Time Prediction

## Project Overview
This project focuses on predicting delivery times for e-commerce orders using machine learning and data analytics. By analyzing factors such as product size, distance, traffic, weather, and agent performance, the project builds accurate regression models to estimate delivery times. A user-friendly **Streamlit application** allows users to input order details and receive predicted delivery times in real-time.

---

## Domain
**E-Commerce & Logistics**

---

## Problem Statement
Efficient delivery is critical for customer satisfaction in e-commerce. This project aims to:
- Predict delivery times for orders based on multiple factors.
- Provide actionable insights to optimize logistics and resource allocation.
- Evaluate the performance of delivery agents under different conditions.

---

## Business Use Cases
1. **Enhanced Delivery Logistics**: Predict delivery times to improve planning and customer satisfaction.  
2. **Dynamic Traffic & Weather Adjustments**: Adjust delivery estimates based on real-time conditions.  
3. **Agent Performance Evaluation**: Identify high-performing agents and areas for improvement.  
4. **Operational Efficiency**: Optimize resource allocation and delivery scheduling.

---

## Dataset
**File:** `amazon_delivery.csv`  
**Columns Include:**
- `Order_ID`: Unique order identifier  
- `Agent_Age`, `Agent_Rating`  
- `Store_Latitude/Longitude`, `Drop_Latitude/Longitude`  
- `Order_Date/Order_Time`, `Pickup_Time`  
- `Weather`, `Traffic`, `Vehicle`, `Area`  
- `Delivery_Time`: Target variable (hours)  
- `Category`: Product category  

---

## Approach

### 1. Data Preparation & Cleaning
- Load and preprocess dataset
- Handle missing values and duplicates
- Standardize categorical variables

### 2. Feature Engineering
- Calculate geospatial distance between store and delivery location
- Extract time-based features (hour, day of the week)
- Encode categorical variables

### 3. Exploratory Data Analysis (EDA)
- Analyze delivery time distributions
- Study impact of traffic, weather, and distance
- Visualize agent performance

### 4. Regression Modeling
- Train multiple regression models:
  - Linear Regression
  - Random Forest Regressor
  - Gradient Boosting Regressor
- Evaluate models using RMSE, MAE, and R²
- Track models with **MLflow**

### 5. Application Development
- Build **Streamlit app** for user-friendly delivery time prediction
- Input features: distance, traffic, weather, agent rating, etc.
- Output: predicted delivery time

### 6. Deployment
- Deploy models via Streamlit for real-time usage
- Ensure scalability and user interactivity

---

## Results & Insights
- Cleaned and preprocessed dataset ready for modeling  
- Multiple regression models trained and evaluated  
- Key factors affecting delivery time:
  - Distance between store and delivery location
  - Traffic and weather conditions
  - Agent performance metrics  
- Functional Streamlit app for prediction

---

## Evaluation Metrics
- **Data Quality**: Completeness and correctness of dataset  
- **Model Performance**: RMSE, MAE, R² scores  
- **Application Usability**: Ease of input and result interpretation  
- **Model Tracking**: MLflow logging and comparison of models  

---

## Technology Stack
- **Languages & Libraries**: Python, Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn, Plotly  
- **Deployment**: Streamlit  
- **Model Tracking**: MLflow  

---

## Folder Structure
