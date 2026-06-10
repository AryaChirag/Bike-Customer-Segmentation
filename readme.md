# 🚴 Bike Customer Segmentation Analysis

![Python](https://img.shields.io/badge/Python-blue)
![Pandas](https://img.shields.io/badge/Pandas-black)
![Tableau](https://img.shields.io/badge/Tableau-blue)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

Customer segmentation using RFM analysis to identify high-value and at-risk customers for targeted marketing strategy optimization.

## 📊 Executive Summary

- Built an RFM-based segmentation model using multi-year customer transaction data
- Identified 11 behavioral customer segments
- Discovered that recent and high-value customers drive majority of revenue
- Highlighted significant churn risk in Lost and High-Risk segments
- Developed an interactive Tableau dashboard for business decision-making

## 📌 Project Overview

This analysis is based on multi-year customer transaction and demographic data. It applies RFM (Recency, Frequency, Monetary) analysis to segment customers into 11 behavioral groups, enabling identification of high-value, churn-risk, and inactive customers for targeted marketing strategies.

A Tableau dashboard has been developed to visualize customer behavior and segmentation insights.

---

## 🎯 Business Objective

The goal of this project is to:

- Identify high-value customer segments
- Understand purchasing behavior patterns
- Improve customer retention strategies
- Support data-driven marketing decisions
- Increase overall sales efficiency

---

## 🧠 Key Insights

- The majority of customers belong to the **40–49 age group**, indicating a strong mid-age customer base.
- Female customers account for approximately **51% of total bike purchases**, slightly higher than male customers.
- Customers from **Manufacturing and Financial Services** dominate the dataset.
- **Mass Customers** represent the largest wealth segment across all age groups.
- RFM analysis shows that **recent and high-frequency customers generate higher monetary value**, indicating strong engagement patterns.
- A significant portion of customers fall into **Lost and High-Risk segments**, highlighting churn risk opportunities.

---

## 📊 Tableau Dashboard

The Sales Dashboard for Customer Segmentation can be found [here](https://public.tableau.com/app/profile/chirag.arya4385/viz/Customersegmentationdashboard_16941047002960/SalesDashboard).

<p align="center">
  <a href="https://public.tableau.com/app/profile/chirag.arya4385/viz/Customersegmentationdashboard_16941047002960/SalesDashboard">
    <img src="visualizations/Customer%20Segmentation%20Dashboard.png" width="950"/>
  </a>
</p>

Click the dashboard to explore interactive insights

---

## 📊 Exploratory Data Analysis

### Customer Demographics

Analysis shows strong concentration in middle-aged groups, with minimal representation below 30 and above 70.

<p align="center">
  <img src="visualizations/Old%20Customers%20Age%20Distribution.png" width="500" style="margin-right:10px;"/>
  <img src="visualizations/New%20Customers%20Age%20Distribution.png" width="495"/>
</p>

---

### Gender-Based Bike Purchases

- Female customers slightly outperform male customers in bike purchases.

<p align="center">
  <img src="visualizations/Gender%20based%20Bike%20Purchases.png" width="500"/>
</p>

---

### Job Industry Distribution

- Highest customers: Manufacturing and Financial Services  
- Lowest customers: Agriculture and Telecom 

<p align="center">
  <img src="visualizations/Old%20Customers%20Job%20Industry.png" width="450" style="margin-right:10px;"/>
  <img src="visualizations/New%20Customers%20Job%20Industry.png" width="545"/>
</p>

---

### Wealth Segmentation

- Mass Customers dominate across all age groups  
- High Net Worth is the second largest segment

<p align="center">
  <img src="visualizations/Old%20Customers%20Wealth%20Segment.png" width="502" style="margin-right:10px;"/>
  <img src="visualizations/New%20Customers%20Wealth%20Segment.png" width="498"/>
</p>

---

### Cars Owned by State

- New South Wales shows the highest non-car ownership  
- Victoria and Queensland show a balanced distribution

<p align="center">
<img src="visualizations/Car%20Owners%20by%20State.png" width="480"/>
</p>

---

## 🧩 Customer Segmentation (RFM Model)

Customers were segmented into 11 behavioral groups based on Recency, Frequency, and Monetary value to identify customer value and churn risk patterns.

- Platinum Customers  
- Very Loyal Customers  
- Recent Customers  
- Potential Customers  
- Lost Customers  
- Losing Customers  
- High Risk Customers  
- Evasive Customers  
- Becoming Loyal Customers  
- Almost Lost Customers  
- Late Bloomers  

---

## 📈 RFM Analysis Insights

- **Platinum and Very Loyal customers** contribute the highest revenue share
- **Recent customers** show strong conversion potential
- **High-frequency customers** generate higher monetary value
- **Lost customers** represent a significant churn segment

<p align="center">
  <img src="visualizations/Recency%20vs%20Monetary.png" width="500" style="margin-right:10px;"/>
  <img src="visualizations/Frequency%20vs%20Monetary.png" width="500"/>
</p>

---

## 🧹 Data Preparation Summary

The dataset underwent the following preprocessing steps:

- Handling missing values using imputation and removal
- Standardization of categorical variables (Gender, State, Industry)
- Feature engineering (Age, Age Group, Profit calculation)
- Removal of inconsistent and duplicate records
- Conversion of date fields to proper datetime formats

---

## 📂 Dataset Information

The dataset includes:

- Customer Demographics
- Transactions Data
- New Customer List
- Customer Address Data

---

## 🛠️ Tools & Technologies

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Tableau
- Jupyter Notebook
- Excel

---

## 📁 Repository Structure

```text
Bike-Customer-Segmentation/
│
├── clean_data/
│
├── raw_data/
│
├── notebooks/
│
├── visualizations/
│
├── python_files/
│
├── README.md
```

---

## 📂 Data Source

The dataset contains retail customer transaction and demographic data used for RFM-based segmentation analysis.

---

## 🚀 Business Impact

This analysis helps the business to:

- Improve customer targeting and segmentation strategies
- Reduce customer churn
- Increase marketing efficiency
- Optimize segmentation strategy
- Enhance revenue through personalized campaigns

---

## 💡 Business Recommendations

- Focus marketing efforts on Platinum and Very Loyal customers to maximize ROI
- Re-engage Lost and High-Risk customers using targeted campaigns
- Convert Recent Customers into long-term loyal customers
- Personalize offers for Mass Customer segment to improve retention

---

## 🚀 Future Improvements

- Automate the RFM segmentation pipeline using Python scripts
- Deploy an interactive dashboard using Tableau Public refresh automation
- Integrate clustering algorithms (K-Means) for comparison with RFM segmentation
- Build a customer lifetime value (CLV) model

---

## 👤 Author

**Chirag Arya**  
GitHub: [AryaChirag](https://github.com/AryaChirag)
