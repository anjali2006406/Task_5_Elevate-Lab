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


**Observation**

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

**Observation**

- Senior citizens (1) show a higher churn percentage than non-seniors.

- While the number of non-seniors is higher overall, relative churn rate is significantly more in the senior group.

![image](https://github.com/user-attachments/assets/e3e317a1-fcb5-4558-a002-77c9c47d3383)

---

3.**Correlation Heatmap**

- Graph Type: Heatmap
- Columns used: Numerical features (tenure, MonthlyCharges, TotalCharges)

- This heatmap visualizes correlation between numeric features.

- Tenure and TotalCharges have a strong positive correlation, as expected (more time = higher total bill).

- MonthlyCharges has a moderate correlation with TotalCharges.

- No numeric feature shows a direct strong correlation with Churn.

 # Business Insight:
Although Churn doesn’t correlate directly, combinations like low tenure + high MonthlyCharges might indicate churn risk. It highlights the need for multivariate analysis.

**Observation**

- Strong positive correlation between TotalCharges and tenure (makes sense: more tenure = higher total bill).

- MonthlyCharges and TotalCharges also show moderate positive correlation.

- Churn does not correlate highly with any numeric field directly but is visually associated with tenure and charges when combined.

  ![image](https://github.com/user-attachments/assets/9566437f-ae8d-4842-990f-c8c9ca6fe688)

  ---

  



