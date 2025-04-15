# **GRAPH SUMMARIES & OBSERVATIONS**

---


 **Summary:-**

 
1. **Internet Service vs Churn (Count Plot)**
   
- Graph Type: Countplot with hue = Churn
- Columns used: InternetService, Churn

- This plot compares churn behavior across different internet services.

- Fiber Optic users have a significantly higher churn rate compared to other services.

- DSL users show moderate churn behavior.

- Customers who have No Internet Service rarely churn.

# Business Insight:
Customers using fiber optic services may be facing issues such as cost dissatisfaction, technical problems, or competition — indicating a need to assess quality, pricing, or support.


**Observation:-**

- Customers using Fiber Optic internet have the highest churn rate.

- Those using DSL have a moderate churn rate.

- No internet service customers barely churn, indicating basic service users tend to stay longer.

![image](https://github.com/user-attachments/assets/2e21e33f-39b2-4cd2-ab03-678348645b3f)

---

2.**Churn by Senior Citizen (Count Plot)**

- Graph Type: Countplot
- Columns used: SeniorCitizen, Churn

- This plot shows the distribution of churn between senior and non-senior customers.

- Senior citizens (label 1) churn more often compared to non-seniors.

- Although fewer in number, their churn rate is disproportionately high.

# Business Insight:
Senior citizens might need better guidance or personalized service plans. Targeted customer support could help reduce churn in this segment.

**Observation:-**

- Senior citizens (1) show a higher churn percentage than non-seniors.

- While the number of non-seniors is higher overall, relative churn rate is significantly more in the senior group.

![image](https://github.com/user-attachments/assets/e3e317a1-fcb5-4558-a002-77c9c47d3383)

---

3.**Correlation (Heatmap)**

- Graph Type: Heatmap
- Columns used: Numerical features (tenure, MonthlyCharges, TotalCharges)

- This heatmap visualizes correlation between numeric features.

- Tenure and TotalCharges have a strong positive correlation, as expected (more time = higher total bill).

- MonthlyCharges has a moderate correlation with TotalCharges.

- No numeric feature shows a direct strong correlation with Churn.

 # Business Insight:
Although Churn doesn’t correlate directly, combinations like low tenure + high MonthlyCharges might indicate churn risk. It highlights the need for multivariate analysis.

**Observation:-**

- Strong positive correlation between TotalCharges and tenure (makes sense: more tenure = higher total bill).

- MonthlyCharges and TotalCharges also show moderate positive correlation.

- Churn does not correlate highly with any numeric field directly but is visually associated with tenure and charges when combined.

  ![image](https://github.com/user-attachments/assets/9566437f-ae8d-4842-990f-c8c9ca6fe688)

  ---

  4.**Monthly Charges Distribution (Histogram)**

- Graph Type: Histogram
- Column used: MonthlyCharges

- This plot shows how monthly charges are distributed across the customer base.

- Most customers pay between $20 to $90, with a peak near $70-$80.

- A few customers are in the premium price bracket above $100.

# Business Insight:
Churn mitigation strategies should focus on customers in higher charge brackets, especially new ones. These customers are more sensitive to value and service quality.

**Observation:-**

- Distribution is right-skewed — majority of customers pay between 20 to 90 USD/month.

- A noticeable spike is visible around 70–80, indicating a common pricing bracket.

- Few customers pay higher than 100, and very few below 20.

  ![image](https://github.com/user-attachments/assets/d3ba94e1-c32f-41c6-9bc9-1de33d1d34ee)

  ---

  5.**Tenure vs Monthly Charges (Scatter Plot)**

- Graph Type: Scatter plot with hue = Churn
- Columns used: tenure, MonthlyCharges, Churn

- This plot maps customer lifetime (tenure) against their billing amount.

- Churned customers are concentrated in low tenure and high charges — suggesting new customers are leaving due to high costs or unmet expectations.

- Long-tenured customers rarely churn, regardless of cost.

# Business Insight:
Early churn is critical. Offer welcome plans, onboarding help, or discounts to new customers — especially if they are high spenders.

**Observation:-**

- Customers with low tenure and high monthly charges are mostly churned (red dots).

- Long-term customers tend to stay, even if monthly charges are high.

- Clustered churn happens in bottom-left and top-middle zones (new + expensive customers).

![image](https://github.com/user-attachments/assets/608550f3-f95a-49de-954f-1bc8f367344a)

---

6.**Monthly Charges by Churn (Box Plot)**

- Graph Type: Boxplot
- Columns used: MonthlyCharges, Churn

- This shows how monthly billing varies between churned and retained customers.

- Churned customers have higher average and median monthly charges.

- There are some churned outliers with extremely high monthly charges.

 # Business Insight:
Price sensitivity plays a major role. Consider repackaging expensive plans, or offering incentives and loyalty bonuses to high-paying users.

**Observation:-**

- Churned customers have higher median monthly charges.

- There are several high-paying churners (visible through boxplot whiskers).

- Customers who did not churn mostly have lower monthly bills.

  ![image](https://github.com/user-attachments/assets/3943b233-fa88-4f04-8086-5358e8e99b19)

  ---

  7.**MonthlyCharges, TotalCharges, Tenure by Churn(Pair Plot)**

- Graph Type: Pairplot (scatter matrix)
- Columns used: MonthlyCharges, TotalCharges, tenure, Churn

- This multivariate view shows patterns and clusters across three important features.

- Clear cluster of churned customers with low tenure and moderate TotalCharges.

- TotalCharges increases linearly with tenure, but high MonthlyCharges with low tenure appears risky.

# Business Insight:
Supports earlier findings: high bills and short relationships lead to churn. Monitoring this segment can predict early exits and guide intervention.

**Observation:-**

- Clear clustering: churned customers often have low tenure + moderate total charges.

- TotalCharges vs tenure is highly linear — expected due to cumulative billing.

- The scatter patterns confirm that tenure is a key churn predictor, especially when combined with charges.

  ![image](https://github.com/user-attachments/assets/df7c5549-cfbb-44db-a1dd-3351297a9a00)

  ---

  





