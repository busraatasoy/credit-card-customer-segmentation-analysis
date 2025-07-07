# 💳 Credit Card Customer Segmentation

This project focuses on segmenting credit card customers based on their demographics and transactional behavior using the **K-Means clustering algorithm**. The goal is to help the company identify key customer segments and apply tailored business strategies to improve engagement and revenue.

---

## 📌 Objective

- Understand customer patterns through EDA
- Segment customers into **5 groups**
- Explain each group’s behavioral and demographic traits
- Support business decisions with data-driven insights

---

## 🗃 Dataset Overview

- **Records**: 10,127 customers
- **Features**: 14 demographic and transactional attributes

### Key Features:
1. `customer_id:` unique identifier for each customer.
2. `age:` customer age in years.
3. `gender:` customer gender (M or F).
4. `dependent_count:` number of dependents of each customer.
5. `education_level:` level of education ("High School", "Graduate", etc.).
6.`marital_status:` marital status ("Single", "Married", etc.).
7. `estimated_income:` the estimated income for the customer projected by the data science team.
8. `months_on_book:` time as a customer in months.
9. `total_relationship_count:` number of times the customer contacted the company.
10. `months_inactive_12_mon:` number of months the customer did not use the credit card in the last 12 months.
11. `credit_limit:` customer's credit limit.
12. `total_trans_amount:` the overall amount of money spent on the card by the customer.
13. `total_trans_count:` the overall number of times the customer used the card.
14. `avg_utilization_ratio:` daily average utilization ratio.

ℹ️ No missing values detected. Categorical variables were encoded and numerical variables were scaled using **StandardScaler**.

---

## 🔍 EDA Highlights

- Distribution of age, income, and credit usage visualized
- Strong relationships found between transaction frequency, credit limit, and utilization
- High variance observed in `total_trans_amount` and `avg_utilization_ratio`

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Encoding (`OneHotEncoder` for categorical vars)
- Scaling (`StandardScaler` for numeric vars)
- Outlier review and feature engineering

### 2. Clustering
- Applied **K-Means algorithm**
- Evaluated cluster range from **1 to 10**
- Based on the **Elbow Curve**, K=5 was selected as the optimal number:
  - Inertia decreased sharply between 1 and 4 clusters.
  - After **K=5**, the decrease slowed, forming a visible “elbow”.

### 3. Cluster Profiling
- Mean values by cluster were used to describe customer types
- Cluster insights support marketing and retention strategies

---

## 📊 Cluster Descriptions

- **Cluster 1**: Mixed Marital Status, High Income, Male-Dominant  
- **Cluster 2**: Entirely Married, Moderate Income, Female-Dominant
- **Cluster 3**: Entirely Single, Moderate Income, Female-Dominant
- **Cluster 4**: Unknown Marital Status, Moderate Income, Balanced Gender Ratio
- **Cluster 5**: Entirely Divorced, Moderate Income, Balanced Gender Ratio

---

## 🧰 Tools & Technologies

- Python  
- Libraries: pandas, numpy, seaborn, matplotlib, scikit-learn  
- Jupyter Notebook (Kaggle environment)

---

## 🔮 Future Enhancements

- Test with **Hierarchical Clustering**, **DBSCAN**, or **GMM**
- Use **PCA** for dimensionality reduction and visualizations
- Connect results to churn prediction or upsell models
- Create a **Power BI or Tableau dashboard** for business teams

---

## 🔗 Resources

- 📘 [Kaggle Notebook](https://www.kaggle.com/code/busraatasoy/credit-card-customer-segmentation-analysis)
- 📊 [Dataset](https://www.kaggle.com/datasets/busraatasoy/credit-card-customer-segmentation-data)

---

## 👩‍💻 Author

**Büşra Atasoy**  
Data Analyst & Senior OPEX Expert  
📫 [LinkedIn](https://www.linkedin.com/in/busraatasoy)

---


