# Financial-Fraud-Detection-Project

## 🔗 Project Links

- 💻 [Source Code](YOUR_GITHUB_REPOSITORY_URL)
- 🚀 [Live Streamlit Dashboard](https://drive.google.com/file/d/1JgMYBc044AA92r_iW0lq0A_G5pO6y4vp/view?usp=sharing)
- 📊 [Power BI Dashboard](https://drive.google.com/file/d/1h0--yu-GabvDgcDM0rBZDOyi9mi5gld9/view?usp=sharing)
- 📄 [Project Documentation](https://drive.google.com/file/d/1WnvcxTzioD6N5mmI-CBzCET8WgT9Jf1A/view?usp=sharing)


# 📌 **INTRODUCTION**

Financial Fraud Detection is a data analytics and machine learning project designed to identify suspicious financial transactions and reduce fraudulent activities. The project uses transaction data, risk indicators, and machine learning model performance metrics to analyze fraud patterns and support data-driven decision-making. Also  analyzed financial transactions to identify suspicious activities and potential fraud and  monitored transaction trends, payment methods, and geographic fraud patterns and identified important features that contribute to fraud prediction.

# 🎯 **OBJECTIVES**

- **Identify Fraudulent Transactions:** Detect suspicious financial activities and potential fraud patterns.
- **Analyze Transaction Trends:** Examine transaction amounts, frequencies, and historical patterns.
- **Evaluate Payment Methods:** Analyze fraud risks across different payment methods.
- **Monitor Geographic Risks:** Identify locations associated with suspicious transaction activity.
- **Analyze Feature Importance:** Determine the key factors influencing fraud predictions.
- **Evaluate Model Performance:** Assess machine learning models using appropriate evaluation metrics.
- **Develop Interactive Dashboards:** Create Power BI dashboards for effective fraud analysis and visualization.
- **Support Risk Management:** Provide actionable insights to improve fraud prevention strategies.



# 🚀 Project Resources

## 📊 Dashboards

- 🔗 [Power BI Dashboard](https://drive.google.com/file/d/1h0--yu-GabvDgcDM0rBZDOyi9mi5gld9/view?usp=sharing)
- 🌐 [Streamlit Dashboard](https://drive.google.com/file/d/1JgMYBc044AA92r_iW0lq0A_G5pO6y4vp/view?usp=sharing)

## 📄 Project Documentation

- 📑 [View Project Documentation PDF](https://drive.google.com/file/d/1WnvcxTzioD6N5mmI-CBzCET8WgT9Jf1A/view?usp=sharing)

## 📂 Datasets

- 📁 [Fraud Prediction Feature Dataset](https://docs.google.com/spreadsheets/d/1Ry-LfgLMQedO8JxT5bR05PBVfCxKJpIs/edit?usp=sharing&ouid=116913806936212812012&rtpof=true&sd=true)
- 📁 [Payment Method Transaction Dataset](https://docs.google.com/spreadsheets/d/1YpmUJUssS2LRC3c2s7CTzp4-G2zmpIv9/edit?usp=sharing&ouid=116913806936212812012&rtpof=true&sd=true)
- 📁 [ML Model Perfomance  Dataset](https://docs.google.com/spreadsheets/d/1yVHBsCXZfJbnIu3Ah2cEN91lNlwEhYAi/edit?usp=sharing&ouid=116913806936212812012&rtpof=true&sd=true)
- 📁 [Transaction Risk Dataset](https://docs.google.com/spreadsheets/d/1oIivdQzwzeoBqQfnqh-IV9DOcMH-AEQa/edit?usp=sharing&ouid=116913806936212812012&rtpof=true&sd=true)
- 📁 [Fraud Analysis Dataset](https://docs.google.com/spreadsheets/d/1UiYlw3ejGL3YilGkbKrqC_xKg63cxe-5/edit?usp=sharing&ouid=116913806936212812012&rtpof=true&sd=true)
- 📁 [Executive Risk Summary Dataset](https://docs.google.com/spreadsheets/d/1iB3yg65lX3IlWF5RipaaxGm10jtVN4ai/edit?usp=sharing&ouid=116913806936212812012&rtpof=true&sd=true)

  
## 🛠️ Tools & Technologies

- Python
- Pandas
- NumPy
- Scikit-learn
- Machine Learning
- Microsoft Excel
- Power BI
- Power Query
- DAX
- Streamlit
- Matplotlib
- Seaborn
- Jupyter Notebook
- GitHub



## 📊 Key KPIs

- Total Transactions
- Total Fraud Transactions
- Total Legitimate Transactions
- Fraud Detection Rate
- Fraud Loss Amount
- Total Transaction Amount
- Average Transaction Amount
- Fraud Rate (%)
- Fraud by Payment Method
- Geographic Fraud Distribution
- High-Risk Transactions
- Fraud Trends Over Time
- Model Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC Score
- Feature Importance


## 📊 DAX Measures Used:

- Total Transactions = DISTINCTCOUNT('Fraud Data'[Transaction ID])
- Total Fraud Transactions = CALCULATE(DISTINCTCOUNT('Fraud Data'[Transaction ID]), 'Fraud Data'[Is Fraud] = 1)
- Total Legitimate Transactions = CALCULATE(DISTINCTCOUNT('Fraud Data'[Transaction ID]), 'Fraud Data'[Is Fraud] = 0)
- Total Transaction Amount = SUM('Fraud Data'[Transaction Amount])
- Average Transaction Amount = AVERAGE('Fraud Data'[Transaction Amount])
- Fraud Loss Amount = CALCULATE(SUM('Fraud Data'[Transaction Amount]), 'Fraud Data'[Is Fraud] = 1)
- Fraud Rate (%) = DIVIDE([Total Fraud Transactions], [Total Transactions], 0) * 100
- Legitimate Transaction Rate (%) = DIVIDE([Total Legitimate Transactions], [Total Transactions], 0) * 100
- Average Fraud Amount = CALCULATE(AVERAGE('Fraud Data'[Transaction Amount]), 'Fraud Data'[Is Fraud] = 1)
- High-Risk Transactions = CALCULATE(DISTINCTCOUNT('Fraud Data'[Transaction ID]), 'Fraud Data'[Risk Level] = "High")
- Fraud Transactions by Payment Method = CALCULATE(DISTINCTCOUNT('Fraud Data'[Transaction ID]), 'Fraud Data'[Is Fraud] = 1)
- Fraud Transactions by Location = CALCULATE(DISTINCTCOUNT('Fraud Data'[Transaction ID]), 'Fraud Data'[Is Fraud] = 1)
- Total Predicted Fraud = CALCULATE(DISTINCTCOUNT('Fraud Data'[Transaction ID]), 'Fraud Data'[Predicted Fraud] = 1)
- True Positive = CALCULATE(DISTINCTCOUNT('Fraud Data'[Transaction ID]), 'Fraud Data'[Is Fraud] = 1, 'Fraud Data'[Predicted Fraud] = 1)
- False Positive = CALCULATE(DISTINCTCOUNT('Fraud Data'[Transaction ID]), 'Fraud Data'[Is Fraud] = 0, 'Fraud Data'[Predicted Fraud] = 1)
- False Negative = CALCULATE(DISTINCTCOUNT('Fraud Data'[Transaction ID]), 'Fraud Data'[Is Fraud] = 1, 'Fraud Data'[Predicted Fraud] = 0)
- Precision (%) = DIVIDE([True Positive], [True Positive] + [False Positive], 0) * 100
- Recall (%) = DIVIDE([True Positive], [True Positive] + [False Negative], 0) * 100
- F1-Score (%) = DIVIDE(2 * [Precision (%) ] * [Recall (%) ], [Precision (%) ] + [Recall (%) ], 0)


  

## 📂 Repository Structure

```text
Financial-Fraud-Detection/
│
├── 📂 Dataset/
│   ├── Fraud_Analysis_Dashboard_Dataset.xlsx
│   ├── Payment_Method_Risk_Dashboard_Dataset.xlsx
│   ├── Geographic_Fraud_Dashboard_Dataset.xlsx
│   ├── Transaction_Trend_Dashboard_Dataset.xlsx
│   ├── ML_Model_Performance_Dashboard_Dataset.xlsx
│   ├── Fraud_Prediction_Feature_Importance_Dashboard_Dataset.xlsx
│   ├── Executive_Risk_Summary_Dashboard_Dataset.xlsx
│   └── ...
│
├── 📂 Machine_Learning/
│   └── Fraud_Detection_Model.ipynb
│
├── 📂 PowerBI/
│   └── Financial_Fraud_Detection_Dashboard.pbix
│
├── 📂 Streamlit/
│   └── app.py
│
├── 📂 Screenshots/
│   ├── Fraud_Analysis_Dashboard.png
│   ├── Payment_Method_Risk_Dashboard.png
│   ├── Geographic_Fraud_Dashboard.png
│   ├── Transaction_Trend_Dashboard.png
│   ├── ML_Model_Performance_Dashboard.png
│   ├── Feature_Importance_Dashboard.png
│   └── Executive_Risk_Summary_Dashboard.png
│
├── 📂 Documentation/
│   └── Financial_Fraud_Detection_Documentation.pdf
│
└── 📄 README.md
```



## 📌 Conclusion

- The Financial Fraud Detection project integrates Data Analytics, Machine Learning, Power BI, DAX, and Streamlit to support fraud identification and financial risk analysis.
- The project transforms raw transaction data into meaningful business insights through data preprocessing, exploratory data analysis (EDA), and fraud pattern analysis.
- The machine learning component helps identify potentially fraudulent transactions and evaluate fraud prediction performance.
- Payment method and geographic analysis help identify fraud patterns across different transaction categories and locations.
- Feature importance analysis highlights the factors that contribute to fraud predictions.
- Power BI provides interactive dashboards with KPIs, transaction trends, fraud distribution, and risk indicators.
- Streamlit provides a user-friendly interface for exploring fraud insights and analytical results.
- The project demonstrates how data analytics and machine learning can support fraud monitoring, risk assessment, and informed financial decision-making.

## 🎯 Key Learnings

- **Data Preprocessing:** Learned to clean, transform, and prepare transaction datasets for analysis.
- **Exploratory Data Analysis:** Gained insights into transaction patterns, fraud distribution, and risk indicators.
- **Machine Learning:** Understood how classification models can be used to identify potentially fraudulent transactions.
- **Feature Importance:** Learned to identify important variables influencing fraud predictions.
- **Model Evaluation:** Gained experience evaluating model performance using accuracy, precision, recall, F1-score, and ROC-AUC.
- **DAX Measures:** Developed measures to calculate fraud rates, transaction counts, and financial risk KPIs.
- **Power BI Visualization:** Learned to build interactive dashboards for monitoring fraud trends and risk patterns.
- **Streamlit Development:** Gained experience presenting analytical results through an interactive web application.
- **Business Intelligence:** Improved the ability to translate analytical findings into actionable business insights.
- **End-to-End Project Development:** Gained practical experience combining data analytics, machine learning, visualization, and reporting in one project.




  

  


