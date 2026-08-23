# Tourism Consumer Behavior Analytics

## Customer Segmentation & Spending Prediction

An end-to-end **Data Analytics, Machine Learning, and Business Intelligence** project focused on understanding tourism customer behavior, identifying meaningful customer segments, and predicting customer spending.

---

## 📌 Project Overview

Tourism businesses deal with customers who differ significantly in their travel preferences, spending behavior, income levels, and booking patterns.

This project analyzes **2,456 customer records** to uncover behavioral patterns, identify meaningful customer segments, predict customer spending, and transform analytical findings into actionable business insights.

The project combines:

- Exploratory Data Analysis
- Customer Segmentation
- Machine Learning
- Regression Analysis
- Data Visualization
- Power BI
- Business Intelligence
- Data-Driven Recommendations

---

## 🎯 Objectives

The main objectives of this project are to:

- Understand the factors associated with tourism customer spending.
- Identify meaningful customer segments.
- Predict customer spending using regression models.
- Compare multiple machine learning models.
- Build interactive Power BI dashboards.
- Translate analytical findings into actionable business recommendations.

---

## 📊 Dataset

The dataset contains:

- **2,456 customer records**
- **10 tracked features**
- **0 missing values**
- **0 duplicate records**

### Key Features

| Feature | Description |
|---|---|
| Age | Customer age |
| Gender | Customer gender |
| Income Level | Customer income category |
| Preferred Travel Type | Preferred type of travel |
| Avg Trip Duration | Average duration of trips |
| Spending Amount | Customer spending amount |
| Booking Channel | Booking method used |
| Repeat Visitor | Whether the customer is a repeat visitor |
| Customer Review Score | Customer satisfaction/review score |

---

## 🔍 Exploratory Data Analysis

The exploratory analysis was conducted to understand customer distributions and identify relationships between customer characteristics and spending.

### Key Findings

- Spending is centered around approximately **$2,500**.
- Average trip duration is approximately **11 days**.
- Most review scores fall between **3.5 and 4.5**.
- Medium-income travelers represent the largest income group.
- Travel preferences are distributed across Cultural, Leisure, Adventure, and Religious travel.
- Booking behavior is relatively balanced across Website, Agent, and App channels.

### 💰 Spending Drivers

Income level showed a clear relationship with spending:

- **High-income travelers:** ~$3,860 average spending
- **Low-income travelers:** ~$1,650 average spending

Adventure trips recorded the highest average spending at approximately **$3,100**.

### 📈 Correlation Analysis

Two notable relationships were identified:

| Relationship | Correlation |
|---|---:|
| Trip Duration vs. Spending | **r ≈ 0.67** |
| Age vs. Spending | **r ≈ 0.09** |

This indicates that trip duration has a substantially stronger relationship with spending than age.

---

## 👥 Customer Segmentation

Customer segmentation was performed using **K-Means Clustering**.

The following numeric features were scaled before clustering:

- Age
- Trip Duration
- Spending Amount
- Review Score

Different values of **K = 2 to 8** were evaluated using:

- Elbow Method
- Silhouette Score
- Davies-Bouldin Index

The final solution selected:

> **K = 4**

This provided the clearest balance between cluster cohesion and business interpretability.

### Customer Segments

| Segment | Customers | Share | Avg. Spending |
|---|---:|---:|---:|
| High-Value Adventure Travelers | 702 | 28.6% | $3,620 |
| Budget Occasional Travelers | 530 | 21.6% | $1,782 |
| Satisfied Leisure & Religious Travelers | 573 | 23.3% | $2,313 |
| Loyal Mature Travelers | 651 | 26.5% | $2,262 |

---

## 🤖 Spending Prediction

Six regression models were trained and evaluated:

1. Linear Regression
2. Ridge Regression
3. Lasso Regression
4. Gradient Boosting
5. Random Forest
6. Support Vector Regression (RBF)

The models were evaluated using held-out test data and **5-fold cross-validation**.

### 🏆 Best Model

**Linear Regression**

| Metric | Result |
|---|---:|
| R² | **0.904** |
| MAE | **$233.9** |
| RMSE | **$296.2** |

The model explains approximately **90% of the variance in customer spending**.

An important finding was that simpler linear models performed as well as or better than more complex models, suggesting that spending patterns in this dataset are largely driven by additive relationships.

---

## 🔑 Key Predictors of Spending

### 1. Income Level

Higher income levels are associated with substantially higher spending.

### 2. Average Trip Duration

Longer trips are consistently associated with higher total spending.

### 3. Booking Channel & Repeat Visitor

These variables showed smaller positive effects on spending patterns.

---

## 📊 Power BI Dashboard

The project includes an interactive **Power BI dashboard** designed to transform the analytical results into an easy-to-understand business reporting experience.

### Customer Overview

- Customer segment distribution
- Spending by segment
- Travel preferences
- Repeat visitors
- Interactive segment filters

### Spending & ML Insights

- Average spending by income level
- Average spending by booking channel
- Machine learning model comparison
- KPI summary cards

---

## 💡 Business Recommendations

### Extend Customer Stay

Since trip duration has a strong positive relationship with spending, tourism businesses can encourage longer stays through targeted offers and promotional packages.

### Target by Behavior, Not Age

Since age has almost no relationship with spending, premium offers should not rely heavily on age-based targeting.

Instead, customers can be targeted based on:

- Income
- Trip duration
- Travel preferences
- Spending behavior
- Customer segment

---

## 🔄 Project Workflow

‏```text
Raw Tourism Data
        ↓
Data Quality Assessment
        ↓
Exploratory Data Analysis
        ↓
Correlation & Spending Analysis
        ↓
Feature Preparation & Scaling
        ↓
K-Means Customer Segmentation
        ↓
Regression Model Training
        ↓
Model Evaluation & Comparison
        ↓
Power BI Dashboard
        ↓
Business Insights & Recommendations
---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook
- Power BI
- K-Means Clustering
- Regression Analysis
- Data Visualization
- Machine Learning
- Business Intelligence

---

## 📌 Results at a Glance

| Metric | Result |
|---|---:|
| Customer Records | **2,456** |
| Customer Segments | **4** |
| Best Model | **Linear Regression** |
| R² Score | **0.904** |
| MAE | **$233.9** |
| RMSE | **$296.2** |

---
