# Leveraging Predictive Analytics to Revolutionize Inventory Management in Online Retail

### Prashant Chikhalia (Final Project)

## Objective
To develop machine learning models that optimize inventory management by accurately forecasting demand, calculating safety stock, and minimizing stockouts and overstock scenarios.

## Motivation
This project addresses key challenges in online retail inventory management, such as stockouts and overstocking, by leveraging predictive analytics. Advanced models like XGBoost, ARIMA, and Exponential Smoothing were applied to forecast demand, ensuring optimized stock levels and operational efficiency.

## Research Questions
1. What drives purchasing behavior across product categories in online retail?
2. Can historical transaction data predict future sales and optimize stock levels?
3. How do seasonal variations and holidays affect purchasing patterns, and how can this improve stock management?
4. What data-driven strategies can mitigate overstock and stockouts through accurate forecasting?

## Literature Review
1. Literature emphasizes the importance of demand forecasting for inventory optimization. Advanced methods like XGBoost and hybrid models significantly enhance prediction accuracy, especially in e-commerce.  
2. This project leverages time-series models (ARIMA, Exponential Smoothing) and machine learning (XGBoost) to address challenges in stock management, combining accuracy with practical inventory planning techniques.

## Dataset Overview
The dataset comprises approximately 540,000 rows and 8 columns, covering various aspects of sales transactions for an online retail business primarily operating in the United Kingdom. Key features include:

**Invoice**: Unique transaction identifier.
**StockCode**: Product code.
**Description**: Details of the product.
**Quantity**: Number of units sold per transaction.
**InvoiceDate**: Date and time of the transaction.
**Price**: Price per unit of the product.
**Customer ID**: Unique customer identifier.
**Country**: Customer’s country of residence.

**This dataset is suitable for exploring demand forecasting, customer purchasing patterns, and inventory management strategies.**

**Dataset Link**: [Online Retail Data UCI Machine Learning](https://doi.org/10.24432/C5CG6D)

## EDA & Methodology

**Data Preprocessing**: Addressed missing values, removed duplicates, and converted data types. Created new features like revenue per transaction, `IsWeekend`, and rolling averages.

**Analysis Approach**:
1. **Transaction Analysis**: Explored trends in quantity, price, and revenue, identifying seasonal spikes and demand variability.
2. **Country Insights**: Highlighted the UK as the dominant market, with smaller contributions from other countries.
3. **Feature Engineering**: Incorporated `Day of Week`, `7-Day Avg Sales`, and lag features for demand forecasting.

**Modeling**: Applied Exponential Smoothing, ARIMA, and XGBoost for demand prediction. Evaluated models based on RMSE and feature importance analysis.

## Model Results & Evaluation

**Inventory Demand Prediction:**
- **Models Used**: Exponential Smoothing, ARIMA, XGBoost.  
- **Evaluation Metrics**: RMSE, Mean Squared Error (MSE).  
- **Results**:
  - **XGBoost**: RMSE = 9,423 (Best Performance).  
  - **ARIMA**: MSE = 12,304.  
  - **Exponential Smoothing**: MSE = 15,840.

**Key Insights**:
- XGBoost outperformed other models due to its ability to handle complex patterns.
- Important predictors: `IsWeekend`, `7-Day Avg Sales`.

## Conclusion

This project successfully demonstrated the power of predictive analytics in optimizing inventory management for online retail. By leveraging machine learning models such as XGBoost, ARIMA, and Exponential Smoothing, we achieved accurate demand forecasting and actionable insights to improve stock management.

Key outcomes include:
- XGBoost emerged as the best-performing model with an RMSE of 9,423, highlighting its ability to handle complex patterns in demand.
- Feature importance analysis revealed `IsWeekend` and `7-Day Avg Sales` as the most significant predictors, providing valuable insights for inventory planning.
- Safety stock calculations using lead time variability ensured optimal buffer levels, reducing risks of stockouts and overstocking.

This project highlights the importance of combining advanced analytics with feature engineering to solve real-world challenges in e-commerce inventory management.

