# 🚴 Bike Customer Segmentation Analysis

## 📌 Project Overview

This project focuses on analyzing customer purchasing behavior for an automobile bike company to identify valuable customer segments and improve targeted marketing strategies.

Customer segmentation is performed using RFM (Recency, Frequency, Monetary) analysis, a behavior-based approach that groups customers based on their past purchase activity.

The final segmentation divides customers into 11 behavioral groups, enabling the business to identify high-value customers, at-risk customers, and inactive customers for targeted engagement.

A Tableau dashboard was built to visualize customer behavior and segmentation insights.

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

- Platinum and Very Loyal customers generate the highest revenue contribution despite being a smaller segment.
- A significant portion of customers fall into Lost and High-Risk categories, indicating churn risk.
- Customers with recent purchases show higher monetary value, indicating strong engagement.
- The 40–49 age group dominates both new and existing customer segments.
- Female customers account for slightly higher bike purchases (~51%).

---

## 📊 Tableau Dashboard

The Sales Dashboard for Customer Segmentation can be found here:  
https://public.tableau.com/app/profile/chirag.arya4385/viz/Customersegmentationdashboard_16941047002960/SalesDashboard

![Tableau Dashboard](media_files/Customer%20Segmentation%20Dashboard.png)

---

## 📊 Exploratory Data Analysis

### Customer Demographics
- Age distribution across new and existing customers
- Gender-based purchase behavior
- Wealth segmentation across age groups

### Customer Behavior
- Job industry distribution
- Car ownership patterns by state
- Purchase behavior trends

### Revenue Insights
- Relationship between Recency, Frequency, and Monetary value
- Identification of high-value customer clusters

---

## 🧩 Customer Segmentation (RFM Model)

Customers were segmented into 11 groups:

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

## 📈 Segmentation Insights

- Platinum and Very Loyal customers contribute the highest revenue share.
- Lost customers form a significant inactive segment.
- Recent customers show strong potential for conversion.
- Higher engagement leads to higher monetary value.

---

## 📊 Visualizations

| Age Distribution | Gender Analysis |
|------------------|----------------|
| ![](media_files/Old%20Customers%20Age%20Distribution.png) | ![](media_files/Gender%20based%20Bike%20Purchases.png) |

| Customer Segments | RFM Analysis |
|------------------|----------------|
| ![](media_files/Customer%20Segment%20Distribution.png) | ![](media_files/Recency%20vs%20Monetary.png) |

---

## 🛠️ Tools & Technologies

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Tableau
- Jupyter Notebook
- Excel

---

## 📂 Dataset Information

The dataset includes:

- Customer Demographics
- Transactions Data
- New Customer List
- Customer Address Data

---

## 🚀 Business Impact

This analysis helps the business to:

- Improve customer targeting
- Reduce customer churn
- Increase marketing efficiency
- Optimize customer segmentation strategy
- Enhance revenue through personalized campaigns

---

## 👤 Author

Chirag Arya  
GitHub: [AryaChirag](https://github.com/AryaChirag)




# Data Analytics Customer Segmentation

## Goal of the project
The goal of this project is to conduct a Customer Segmentation Analysis for an Automobile bike Company. Customer segmentation is performed by developing an RFM Model. RFM (Recency, Frequency, Monetary) analysis is a behavior-based approach grouping customers into segments. It groups the customers on the basis of their previous purchase transactions. In this analysis, the customer segment was divided into 11 groups. The analysis will help in determining which customer segments should be targeted in order to enhance sales revenue for the company. A **Sales Dashboard for Customer Segmentation** is developed using **Tableau** and the data quality assessment and analysis is done using **Python**.

## Tableau Dashboard
The Sales Dashboard for Customer Segmentation can be found [here](https://public.tableau.com/app/profile/chirag.arya4385/viz/Customersegmentationdashboard_16941047002960/SalesDashboard).

![Tableau Dashboard](media_files/Customer%20Segmentation%20Dashboard.png)

**In case of failure of loading Jupyter Notebooks on Github, the following notebooks can be found in the nb viewer. Click on the respective hyperlinks to view:**

+ [Data_cleaning_customer_address.ipynb](https://nbviewer.org/github/AryaChirag/Data-Analytics-Bike-Customer-Segmentation/blob/master/Data_cleaning_customer_address.ipynb)
+ [Data_cleaning_customer_demographic.ipynb](https://nbviewer.org/github/AryaChirag/Data-Analytics-Bike-Customer-Segmentation/blob/master/Data_cleaning_customer_demographic.ipynb)
+ [Data_cleaning_new_customer_list.ipynb](https://nbviewer.org/github/AryaChirag/Data-Analytics-Bike-Customer-Segmentation/blob/master/Data_cleaning_new_customer_list.ipynb)
+ [Data_cleaning_transactions.ipynb](https://nbviewer.org/github/AryaChirag/Data-Analytics-Bike-Customer-Segmentation/blob/master/Data_cleaning_transactions.ipynb)
+ [RFM_analysis.ipynb](https://nbviewer.org/github/AryaChirag/Data-Analytics-Bike-Customer-Segmentation/blob/master/RFM_analysis.ipynb)

## Analysis Approach

### 1. Data Quality Assessment and Data Cleaning
The first step towards generating useful insights from the data was the data preparation, quality assessment, and data cleaning step. After the cleaning process, exploratory data analysis on the dataset and identification of customer purchasing behaviors to generate insights can be performed.

In the data cleaning step, the data quality of the following datasets was first assessed. After a data quality assessment, the following data quality issues were observed and the necessary process to mitigate the issue was followed :

+ **CustomerDemographics.xlsx :**
  + 1 Irrelevant column was present and such columns were dropped from the dataset.
  + There were 5 columns where Missing values were present. For such columns based on the volume of the missing values either the records were dropped or appropriate values were imputed at places of missing values.
  + For the gender column, there was no standardization of data. Based on the values available the column data was standardized to remove data inconsistency.
  + The Date of Birth column was transformed to create a new feature column 'Age' and 'Age Group' to check for discrepancies in age distribution. An outlier was observed and the record was removed.
  + Checked whether there are duplicate records present in the dataset. In this dataset, there were no duplicate records.
  
+ **NewCustomerList.xlsx :**
  + 5 Irrelevant column was present and such columns were dropped from the dataset.
  + There were 4 columns where Missing values were present. For such columns based on the volume of the missing values either the records were dropped or appropriate values were imputed at places of missing values.
  + The Date of Birth column was transformed to create a new feature column 'Age' and 'Age Group' to check for discrepancies in age distribution.
  + There was no data inconsistency.
  + Checked whether there are duplicate records present in the dataset. In this dataset, there were no duplicate records.
  
+ **Transaction_data.xlsx :**
  + The product_first_sold_date column is not in datetime format. The data type of this column was changed from int64 to datetime format.
  + There were 7 columns where Missing values were present. For such columns based on the volume of the missing values either the records were dropped or appropriate values were imputed at places of missing values.
  + A new feature column 'Profit' was created which is basically the difference between the list price and the standard price.
  + There was no data inconsistency.
  + Checked whether there are duplicate records present in the dataset. In this dataset, there were no duplicate records.

+ **CustomerAddress.xlsx :**
  + For the states column, there was no standardization of data. Based on the values available the column data was standardized to remove data inconsistency.
  + There were certain customer IDs from the Customer Demographics table that were getting dropped in the Address table.
  
### 2. Exploratory Data Analysis on Customer Segments
After the data cleaning process, exploratory analysis of the dataset is performed and the following insights are obtained :
+ New vs. Old Customers Age Distribution
  + Most New customers are aged between 40-49 also for Old Customers most of them are aged between 40-49.
  + The lowest number of customers for both types of customers is present in the age bracket under 30 and above 70 age groups.
  + The automobile company is popular among New Customers between the age of 40-70.
  + A steep drop in customers is observed in the 30-39 age group among the New Customers.

| Old Customers by Age Distribution | New Customers by Age Distribution |
| :------------- | :------------- |
|![](media_files/Old%20Customers%20Age%20Distribution.png)|![](media_files/New%20Customers%20Age%20Distribution.png)|

+ Bike purchases over the last 3 years by Gender
  + Most bike purchases have been done by Females over the last 3 years. Approximately 51% of the bike purchases are done by Females compared to 49% of the purchases being done by Males.
  + The Female purchases are 10,000 more than that of Male purchases (numerically).
  
![](media_files/Gender%20based%20Bike%20Purchases.png)

+ New vs. Old Customers Job Industry Distribution
  + Most New customers are from the Manufacturing and Financial Services sector (approx 20% of the New Customers).
  + The lowest number of customers are from the Agriculture and Telecom sector approx 3%.
  + A similar trend is observed among Old Customers as well.

| Old Customers by Job Industry | New Customers by Job Industry |
| :------------- | :------------- |
|![](media_files/Old%20Customers%20Job%20Industry.png)|![](media_files/New%20Customers%20Job%20Industry.png)|

+ Wealth Segmentation by Age Category
  + Across all age categories, the largest number of customers are from the 'Mass Customer' Segment.
  + The next category comes from the 'High Net Worth' customers.
  + In the age group 40-49, the Affluent segment outperforms the high-worth customers in terms of number of customers despite old or new customers.

| Old Customers Wealth by Age Group | New Customers Wealth by Age Group |
| :------------- | :------------- |
|![](media_files/Old%20Customers%20Wealth%20Segment.png)|![](media_files/New%20Customers%20Wealth%20Segment.png)|

+ Cars owned by States
  + New South Wales has the largest number of people who don't own a car.
  + In Victoria and Queensland the proportion is quite even.
  + In New South Wales the number of people owning a car is significantly lesser than those who do not have a car.

![](media_files/Car%20Owners%20by%20State.png)

### 1. Customer Segmentation and RFM Analysis
In this stage of analysis, the customer segmentation was done by developing an RFM Model. The RFM (Recency, Frequency, Monetary) analysis is a behavior-based approach grouping customers into segments. It groups the customers on the basis of their previous purchase transactions.

In this analysis, the customer segment was divided into 11 groups. The groups are:

+ Platinum Customers
+ Very Loyal Customers
+ Recent Customers
+ Potential Customers
+ Lost Customers
+ Losing Customers
+ Late Bloomer
+ High Risk Customers
+ Evasive Customers
+ Becoming Loyal
+ Almost lost Customers

As of the current state of the Automobile business the distribution of customer segments is depicted below:
![](media_files/Customer%20Segment%20Distribution.png)

+ Recency and Frequency vs. Monetary Distribution
  + Customers who purchased recently generated more revenue than customers who visited a long time ago.
  + Customers classified as "Platinum Custoers", "Very Loyal" and "Becoming Loyal" visit frequently.

| Recency vs Monetary | Frequency vs Monetary |
| :------------- | :------------- |
| ![](media_files/Recency%20vs%20Monetary.png) | ![](media_files/Frequency%20vs%20Monetary.png) |


## Datasets Used
The datasets used include:
+ **Raw_data.xlsx:** This Excel file dataset included the following sheets of data:
  + **Transactions_data.xlsx:** This dataset included the transaction data of the customers across all the different states in Australia.
  + **NewCustomerList.xlsx:** This dataset included the new customers who visited the automobile bike company recently.
  + **CustomerDemographic.xlsx:** This dataset included entire details of the Customer Demographics.
  + **CustomerAddress.xlsx:** This dataset included the address of the Customers.
  
## Tools and Technologies Used
The tools used in this project include:
+ **Python** - This was needed to conduct Data Quality Assessment and also for Data Cleaning processes. With Python libraries **pandas, numpy, matplotlib, seaborn, math** exploratory data analysis of the datasets and gaining useful insights from the data was possible.
+ **Tableau**- A Business Intelligence tool was required to explore data and visualize the data by creating charts, and graphs to come up with a Sales Dashboard for Customer segmentation for a bike company.

## Built With
+ Python 3.10.11
+ Google Colab
+ Tableau

## Authors
+ Chirag Arya - [Github Profile](https://github.com/AryaChirag)
