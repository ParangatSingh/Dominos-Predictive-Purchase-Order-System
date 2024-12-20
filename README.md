# Dominos Predictive Purchase Order System

## **Overview**
This project focuses on forecasting the ingredients needed for pizzas using historical sales data and the ARIMA model. The goal is to enhance inventory management and reduce food wastage by predicting the ingredient requirements for the upcoming week.

---

## **Key Components**

### **1. Data Exploration and Cleaning**
- Perform an initial analysis of the datasets to assess their structure and quality.
- Handle missing ingredient quantities and identify outliers to ensure reliable model training.

### **2. Feature Engineering**
- Derive additional features from the existing data to provide better context for predictions.
- Create time-based features from `order_date`, such as:
  - Day of the week
  - Day of the year
  - Month  
  These features are intended to improve the predictive performance of the model.

### **3. Model Training**
- Train the ARIMA model using historical sales data to forecast future ingredient needs.
- Optimize model parameters to enhance prediction accuracy and reliability.

### **4. Model Evaluation**
- Evaluate the model's performance using **Mean Absolute Percentage Error (MAPE)** to ensure predictions align with business requirements.

---

## **Datasets**

### **1. Pizza Ingredients (`Pizza_ingredients.csv`)**
Contains information about the ingredient requirements for each type of pizza.

**Key Columns:**
- `pizza_name_id`
- `pizza_name`
- `pizza_ingredients`
- `Items_Qty_In_Grams`

### **2. Pizza Sales (`Pizza_Sale.csv`)**
Includes historical sales data for pizzas.

**Key Columns:**
- `pizza_id`
- `order_id`
- `pizza_name_id`
- `quantity`
- `order_date`
- `order_time`
- `unit_price`
- `total_price`
- `pizza_size`
- `pizza_category`
- `pizza_ingredients`
- `pizza_name`

---
