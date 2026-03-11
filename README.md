# Customer-Churn-Prediction
📉 Customer Churn Prediction with Machine Learning

This project focuses on forecasting customer churn using a telecommunications dataset. The primary aim is to identify customers who are likely to discontinue their services and uncover the business factors contributing to churn. By doing so, organizations can take preventive actions and improve customer retention strategies.

🧠 Project Objective

The purpose of this project is to:

Examine customer data to identify patterns and key drivers of churn

Develop machine learning models capable of predicting churn behavior

Evaluate multiple models to determine the most effective one

Convert analytical findings into practical business insights and strategies

📊 Dataset Overview

Source: Telco Customer Churn Dataset (IBM Sample Dataset / Kaggle)

Total Records: 7,043 customers

Features: 21 columns including demographics, subscribed services, and payment details

Target Variable: Churn (Yes / No)

🔍 Exploratory Data Analysis (EDA)

Data exploration was conducted using Seaborn and Matplotlib to understand patterns within the dataset.

Key visualizations included:

📌 Pie chart illustrating the overall churn distribution

📌 Histograms comparing tenure and monthly charges between churned and retained customers

📌 Count plots analyzing contract type and payment methods against churn behavior

📌 Correlation heatmaps highlighting relationships between numerical variables

These visual analyses revealed several insights:

Customers with shorter tenure are more likely to churn

Month-to-month contracts are strongly associated with higher churn rates

Customers paying via electronic check show higher churn tendencies

Higher monthly charges increase churn probability

🤖 Machine Learning Models

Several machine learning algorithms were trained and evaluated to predict customer churn.

Model	Accuracy
Logistic Regression	~80%
Random Forest	~82% ✅ Best
Support Vector Machine (SVM)	~78%
K-Nearest Neighbors	~75%
Naive Bayes	~72%

Preprocessing steps included:

Label Encoding for categorical variables

Feature Scaling

Train–Test Split for model evaluation

Performance was assessed using accuracy score, confusion matrix, and classification reports.
Among all models, the Random Forest Classifier delivered the best performance.

📈 Visual Outputs

All visualizations created during EDA and model comparison are stored in the visuals/ directory, including:

Churn Distribution Pie Chart

Tenure Distribution by Churn

Monthly Charges Density Plot by Churn

Contract Type vs Churn Visualization

Model Accuracy Comparison Bar Chart

🧠 Key Business Insights

This project goes beyond predictive modeling by extracting valuable business insights:

Approximately 27% of customers leave the service, indicating a major revenue loss

Customers with month-to-month contracts show a 42% churn rate, compared to only 11% for long-term contracts

Users with less than 12 months of tenure are the most vulnerable segment

Electronic check payments are strongly correlated with churn behavior

These insights allow companies to identify high-risk customers early and implement targeted retention programs.

💼 Business Recommendations
Strategy	Description
🎯 Focus on new customers	Provide onboarding support, discounts, or loyalty incentives
📄 Promote long-term contracts	Encourage customers to switch from monthly plans through discounts
💳 Promote stable payment methods	Encourage credit card or auto-pay instead of electronic checks
📢 Use churn prediction model	Share churn risk scores with marketing and support teams for proactive engagement
🛠️ Tools & Technologies

Python

Pandas & NumPy – Data preprocessing and manipulation

Seaborn & Matplotlib – Data visualization

Scikit-learn – Machine learning modeling

Jupyter Notebook – Development environment

📌 Future Enhancements

Possible improvements for this project include:

Applying SMOTE to address class imbalance

Deploying the model using a Streamlit web application for non-technical users

Integrating customer feedback or sentiment data for richer features

Monitoring model performance with live churn data over time
