# 🍔 Food Business Intelligence  
### Data Cleaning, Feature Engineering, and Exploratory Analysis Using Python

## 📌 Overview
Food delivery businesses generate large volumes of transactional data that are often incomplete, inconsistent, and difficult to analyze. Poor data quality leads to inaccurate reporting, weak insights, and poor business decisions.

This project focuses on transforming a **raw, messy food delivery dataset** into a **clean, analysis-ready dataset** and extracting **key business insights** to support decision-making in pricing, operations, customer satisfaction, and revenue optimization.

---

## ❗ Problem Statement
The original dataset contained several data quality issues, including:

- Missing values across multiple columns  
- Inconsistent text formatting  
- Incorrect data types (dates and ratings stored as text)  
- Duplicate records  
- Lack of business-ready metrics (e.g., final price, fast delivery indicator)

Without proper cleaning and transformation, the dataset could not be reliably used for business intelligence or analytics.

---

## 🎯 Project Objectives
The objectives of this project were to:

- Clean and standardize a raw food delivery dataset  
- Handle missing values using appropriate statistical methods  
- Engineer new features to support business analysis  
- Perform exploratory data analysis (EDA) to generate actionable insights  
- Produce a final, clean dataset suitable for dashboards and reporting  

---

## 🛠 Tools & Technologies
- **Python**
- **Pandas** – data manipulation and cleaning  
- **Matplotlib** – visual exploration  
- **Jupyter Notebook**

---

## 📂 Dataset Description
- **Initial size:** 1,050 rows × 12 columns  
- **Final size:** 1,000 rows × 14 columns  

### Key Fields
- Food  
- Category  
- Restaurant  
- Location  
- Price  
- Discount  
- Final_Price  
- Delivery_Time  
- Rating  
- Date  

---

## 🔍 Methodology

### Phase 1: Data Cleaning
The following steps were carried out:

- Imported required libraries  
- Loaded raw CSV data into Pandas  
- Inspected dataset size, structure, and data types  
- Identified missing values in numeric and categorical columns  
- Removed extra spaces from column names  
- Converted `Date` to datetime format  
- Converted `Rating` to numeric values  
- Filled missing numeric values using **median imputation**  
- Filled missing categorical values using **mode imputation**  
- Standardized text formatting (capitalization and spacing)  
- Removed duplicate records  

---

### Phase 2: Feature Engineering
New business-relevant features were created:

- **Fast_Delivery:** Indicates whether delivery time ≤ 30 minutes  
- **Final_Price:** Actual price paid after discount  

These features enable deeper operational and financial analysis.

---

### Phase 3: Exploratory Data Analysis (EDA)
Key business metrics and insights were computed, including:

- Total revenue generated  
- Total number of orders  
- Average order value  
- Average customer rating  
- Revenue breakdown by restaurant  
- Revenue breakdown by food category  

---

## 📊 Key Findings & Insights
- **Total Revenue:** ₦454,245  
- **Top Revenue Category:** Fast Food  
- **Top Restaurant by Revenue:** McDonald’s  
- **Average Order Value:** ~₦454  
- Faster deliveries were associated with **higher customer ratings**

---

## ✅ Conclusion
This project demonstrates how raw operational data can be transformed into valuable business intelligence using Python. Through proper data cleaning, feature engineering, and exploratory analysis, the dataset was converted into a reliable foundation for dashboards, forecasting, and strategic decision-making in the food delivery industry.

---

## 💡 Recommendations
- Businesses should closely track delivery speed to improve customer satisfaction  
- Discounts should be optimized based on category performance  
- Further analysis can be extended to customer segmentation and time-based trends  

---

## 📁 Project Structure
```text
├── data/
│   ├── raw_food_data.csv
│   └── cleaned_food_data.csv
├── notebook/
│   └── food_business_intelligence.ipynb
├── README.md
