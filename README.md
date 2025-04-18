**Task_5_Elevate-Lab**

# **Customer Churn Analysis**

---

 ## **Overview**

- This project involves performing Exploratory Data Analysis (EDA) on a Customer Churn dataset using Python libraries: Pandas, Seaborn, and Matplotlib. The goal is to uncover insights into why customers churn by examining trends, patterns, and correlations within the data.


 **Dataset Information**

- Total Rows: 7043-- Total Columns: 21-- Target Column: Churn

- Contains a mix of numerical and categorical variables related to customer profiles, service usage, and account info.

- Key Columns:

tenure, MonthlyCharges, TotalCharges

gender, SeniorCitizen, Partner, Dependents

InternetService, TechSupport, Contract, PaymentMethod

### **Libraries Used**

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

---

# **Data Cleaning**

 - Loaded the dataset: Customer Churn.csv-- Replaced blank values in TotalCharges with 0 and converted it to float.-- Confirmed:

No null values ✅

No duplicate rows ✅

**Data Overview & Descriptive Statistics**

- Used .info() and .describe() to understand data types and distributions.-- Descriptive insights:

- Mean tenure: 32.3 months

- Average Monthly Charges: 64.76

- Average Total Charges: 2279.73

- Churn Rate: 1869 (Yes), 5174 (No)

---

# **Graphical Analysis with Insights**

 **Internet Service vs Churn**

sns.countplot(x='InternetService', hue='Churn', data=df, palette={'No':'lightgreen','Yes':'salmon'})

  **Insight: Customers with Fiber Optic internet have a higher churn rate.**
  

# **Senior Citizens and Churn**

sns.countplot(x='SeniorCitizen', hue='Churn', data=df, palette='Set2')

**Insight: Senior citizens churn more than non-senior customers.**


# **Correlation Heatmap**

sns.heatmap(df.corr(numeric_only=True), annot=True, cmap='coolwarm')

 **Insight: Tenure and TotalCharges are highly correlated. MonthlyCharges is weakly correlated with tenure.**
 

# **Distribution of Monthly Charges**

df['MonthlyCharges'].plot(kind='hist', bins=20, color='skyblue', edgecolor='black')

 **Insight: Charges are right-skewed. Most customers are charged between 20–90.**
 

# **Scatter Plot: Tenure vs Monthly Charges**

sns.scatterplot(x='tenure', y='MonthlyCharges', hue='Churn', data=df)

 **Insight: High churn is observed in customers with low tenure and high charges.**
 

# **Box Plot: Monthly Charges by Churn**

sns.boxplot(x='Churn', y='MonthlyCharges', data=df)

 **Insight: Customers who churn generally have higher monthly charges.**
 

# **Pair Plot: MonthlyCharges, TotalCharges, Tenure**

sns.pairplot(df[['MonthlyCharges', 'TotalCharges', 'tenure', 'Churn']], hue='Churn')

 **Insight: Churned customers cluster in low tenure and medium total charges.**

 ---

# **Key Findings**

- Customers with Fiber Optic internet and high monthly charges are more likely to churn.-- Short tenure and senior citizens are churn-prone.-- Contract type, payment method, and tech support play a significant role in retention.

 **Recommended GitHub Repo Structure**

 Customer-Churn-EDA
│
├──  Customer Churn.csv
├──  Customer Churn Analysis.ipynb
├──  Customer Churn Analysis.pdf
├──  README.md


---


 **Interview Questions & Prep**

-  What is EDA and why is it important?

It is the process of visually and statistically analyzing data to find patterns, anomalies, and trends.

- Which plots are used to check correlation?

Heatmap, Pairplot

-  How do you handle skewed data?

Use log/sqrt transformation or detect via boxplots.

- How to detect multicollinearity?

Use correlation matrix or VIF scores.

- What are univariate, bivariate, and multivariate analyses?

Univariate = 1 variable; Bivariate = 2 variables; Multivariate = 2+ variables

- Difference between heatmap and pairplot?

Heatmap shows correlations; pairplot shows scatter plots + histograms.

- How do you summarize your insights?

Through visuals + bullet points highlighting key trends.

---


### **Author**

**Anjali Singh**  

_Aspiring Business and Data Analyst_ 

🔗 [LinkedIn] :-www.linkedin.com/in/anjalissingh 

