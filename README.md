# Leveraging Predictive Analytics to Revolutionize Inventory Management in Online Retail

### Prashant Chikhalia

## Objective
To develop predictive models that optimize inventory management by accurately forecasting stock levels, thereby reducing costs and preventing stockouts.

## Motivation
This project aims to improve inventory management in online retail by using a forecasting model to tackle common issues like overstock and stockouts, leveraging data-driven insights and machine learning.

## Research Questions
1. What drives purchasing behavior across product categories in online retail?
2. Can historical transaction data predict future sales and optimize stock levels?
3. How do seasonal variations and holidays affect purchasing patterns, and how can this improve stock management?
4. What data-driven strategies can mitigate overstock and stockouts through accurate forecasting?

## Literature Review
The literature highlights the need for accurate demand forecasting and efficient inventory management. Advanced models like ensemble learning and hybrid approaches improve prediction accuracy but require significant computational power. This project uses machine learning to optimize demand forecasting and stock adjustments, with tools like SHAP for interpretability and Streamlit for real-time updates, aiming to make inventory management more data-driven and transparent.

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

**Data Preprocessing**: Addressed missing values, removed duplicates, and ensured accurate data types. Engineered new features, such as revenue per transaction.

**Analysis Approach**:
1. **Transaction Analysis**: Explored key patterns in quantity, unit price, and revenue distributions, identifying right-skewed trends.
2. **Country Insights**: Analyzed transaction counts by country, highlighting the UK as the primary market.
3. **Future Steps**: Plan to conduct further time-based analysis (e.g., trends by month, day) and customer segmentation for targeted insights.

## Model Results & Evaluation

**Inventory Demand Prediction:**
- **Model Used**: Linear Regression (with potential to test other models if needed).
- **Evaluation Metrics**: Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² Score.
- **Results:**
    - **Linear Regression**: MAE = 320.45, RMSE = 950.32, R² = 0.92

## Next Steps
1. **Advanced EDA:** Analyze trends and segment customers.
2. **Feature Engineering:** Create and normalize new features.
3. **Modeling:** Use clustering and time series forecasting.
4. **Evaluation:** Assess model with metrics.
5. **Visualization:** Create visuals and finalize insights.
6. **Documentation:** Summarize in a report.
7. **Model Tuning:** Experiment with advanced models.
