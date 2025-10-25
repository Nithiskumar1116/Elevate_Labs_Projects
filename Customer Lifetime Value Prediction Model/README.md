# Customer_Lifetime_Value_Prediction_Model
Project 1 || Data Analyst Intern || Elevate Labs

The Customer Lifetime Value (LTV) Prediction Model aims to estimate the total revenue a business can expect from a customer throughout their relationship. By analyzing historical transaction data, the project helps organizations identify high-value customers, optimize marketing spend, and improve customer retention strategies.

This model uses RFM analysis (Recency, Frequency, Monetary) and machine learning algorithms such as Random Forest and XGBoost to predict each customer's future spending potential. The dataset typically includes customer transaction records with attributes like CustomerID, InvoiceDate, Quantity, and UnitPrice.

The process involves several key stages:

Data Preprocessing 
    Cleaning missing values, removing negative quantities, and calculating total sales per transaction.

Feature Engineering 
    Creating RFM features (Recency, Frequency, Monetary) and additional metrics like Average Order Value (AOV).

Model Training 
    Splitting data into training and testing sets, then fitting regression models to predict LTV.

Model Evaluation 
    Assessing performance using metrics such as MAE (Mean Absolute Error) and RMSE (Root Mean Squared Error).

Customer Segmentation 
    Categorizing customers into value segments (Low, Medium, High, VIP) based on predicted LTV.

Visualization & Insights 
    Using histograms and boxplots to show LTV distribution and customer segment patterns.

The final output provides a CSV file containing each customer’s predicted LTV and segment label, enabling data-driven decisions for targeted promotions and personalized engagement.
