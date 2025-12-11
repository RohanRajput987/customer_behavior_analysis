# customer_behavior_analysis
An end-to-end customer analytics solution performing data cleaning, exploratory analysis, segmentation, and visualization using Python, SQL, and Power BI to derive meaningful behavioral insights.

# 🛒 Customer Shopping Behavior Analysis

This project presents an end-to-end data analytics workflow using Python, SQL (PostgreSQL/MySQL/SQL Server), and Power BI to analyze customer shopping behavior.  
The analysis is based on 3,900 transactions and reveals actionable business insights related to demographics, spending patterns, product performance, segmentation, and subscription behavior.

Insights, visuals, and workflow stages are directly derived from the project assets provided. :contentReference[oaicite:0]{index=0}

---

## 📌 Overview

The goal of this project is to transform raw transactional data into meaningful business intelligence.  
The workflow includes:

- Loading and preprocessing data in **Python**
- Performing **EDA** and handling missing values
- Cleaning and feature engineering (age groups, purchase frequency, etc.)
- Loading the cleaned dataset into **PostgreSQL** for SQL analysis
- Running 10+ SQL queries to extract business insights :contentReference[oaicite:1]{index=1}
- Building an interactive **Power BI dashboard**
- Developing a business insights **Report & PPT** using **Gamma**

This project simulates a real-world retail analytics scenario.

---

## 📂 Dataset

The dataset contains **3,900 customer purchases** with **18 variables**, including:  
- Demographics: gender, age, location  
- Shopping behavior: discount applied, previous purchases, subscription status  
- Transaction details: item purchased, category, purchase amount, shipping type, review rating  
- Product attributes: size, color, season  

37 missing values were found only in the *review_rating* column and imputed by median category rating. :contentReference[oaicite:2]{index=2}

---

## 🛠️ Tools Used

- **Python** → pandas, numpy, seaborn/matplotlib  
- **PostgreSQL / MySQL / SQL Server** → analytics queries  
- **Power BI** → interactive dashboard  
- **Gamma** → automated PPT generation  
- **Jupyter Notebook** → EDA and transformation  
- **GitHub** → version control

---

## 🔧 Steps Performed

### **1️⃣ Load & Explore Data in Python**
- Imported the dataset using pandas  
- Explored structure using `.info()` and `.describe()`  
- Identified missing values and inconsistencies  
- Standardized column names

### **2️⃣ Data Cleaning**
- Imputed missing review ratings using category-level medians  
- Removed redundant columns (e.g., promo_code_used) :contentReference[oaicite:3]{index=3}  
- Verified consistency of discount and purchase data  
- Created engineered features:
  - `age_group`
  - `purchase_frequency_days`

### **3️⃣ Load Data into SQL Database**
- Connected Python to PostgreSQL  
- Inserted cleaned dataset into SQL tables  
- Ran analytical SQL queries across:
  - Revenue analysis  
  - Discount behavior  
  - Product ratings  
  - Customer segmentation  
  - Subscription insights  
  - Category and age-group performance

### **4️⃣ SQL Business Questions Answered**
Some examples (full script in `customer_behavior_sql_queries.sql`):

- Revenue by gender  
- High-spending discount users  
- Top 5 products by review rating  
- Shipping type comparison  
- Subscription vs non-subscription spending  
- Top 3 items per category  
- Customer segmentation (New, Returning, Loyal)  
- Revenue by age group  
All queries and results match the SQL output shown in the project PDF. :contentReference[oaicite:4]{index=4}

### **5️⃣ Power BI Dashboard Development**
Created an interactive dashboard highlighting:

- Total customers  
- Average purchase amount  
- Average review rating  
- Revenue by category & age group  
- Subscription share (27% vs 73%)  
- Sales by category  
- Customer segmentation KPIs (Loyal, New, Returning)  

Dashboard visuals match those shown in the project files. :contentReference[oaicite:5]{index=5}

### **6️⃣ Report & Presentation (Gamma)**
- Summarized key insights  
- Visual storytelling using charts, KPIs, and category breakdowns  
- Strategic business recommendations such as:
  - Boost subscription conversions
  - Strengthen loyalty programs
  - Highlight top-rated products in campaigns  
Based on the report PDF and PPT. :contentReference[oaicite:6]{index=6}

---

## 📊 Key Results & Insights

### **• Revenue by Gender**
Male customers generate ~68% of total revenue, indicating an opportunity to grow female engagement. :contentReference[oaicite:7]{index=7}

### **• Product Ratings**
Top-rated products include Gloves, Sandals, Boots, Hat, and Skirt. :contentReference[oaicite:8]{index=8}

### **• Shipping Influence**
Express users spend **$2–$7 more** per order than standard shipping customers. :contentReference[oaicite:9]{index=9}

### **• Subscription Behavior**
- 27% subscribers  
- Subscribers contribute $62K in revenue  
- Non-subscribers contribute $170K  
Average spend nearly identical (~$59.5). :contentReference[oaicite:10]{index=10}

### **• Customer Segmentation**
Based on purchase history:
- Loyal customers: 3,116  
- Returning: 701  
- New: 83  
Loyal buyers make up **80% of customer base**. :contentReference[oaicite:11]{index=11}

### **• Age Group Revenue**
Young adults contribute the highest revenue (~$62K). :contentReference[oaicite:12]{index=12}

---

## 📈 Power BI Dashboard

The dashboard includes:

- KPIs (customers, revenue, avg purchase amount)
- Subscription breakdown
- Revenue by category
- Sales by age group
- Revenue by shipping type
- Product ratings and discount dependency

Screenshots and visuals match the uploaded PBIX report.

---

## 🚀 How to Run This Project

### **1. Clone the Repo**
```bash
git clone https://github.com/RohanRajput987/customer_behavior_analysis
