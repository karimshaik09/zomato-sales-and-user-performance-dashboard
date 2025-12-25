
# Zomato Sales & User Performance Dashboard - Power BI Project
## Brief One-Line Summary

A Power BI dashboard analyzing Zomato’s sales, user behavior, food trends, and city-level performance for data-driven decision-making.

---
## Table of Contents
- [Overview](#overview)
- [Problem Statement](#problem-statement)
- [Dataset](#dataset)
- [Tools and Technologies](#tools-and-technologies)
- [Project Structure](#project-structure)
- [Data Modeling](#data-modeling)
- [DAX Measures](#dax-measures)
- [Key Insights](#key-insights)
- [Dashboard Output](#dashboard-output)
- [How to Run This Project](#how-to-run-this-project)
- [Results and Conclusion](#results-and-conclusion)
- [Future Work](#future-work)
- [Author and Contact](#author-and-contact)

---

## Overview
This project presents a Power BI dashboard that analyzes Zomato’s business performance across multiple cities, food categories, and user demographics.

The dashboard delivers insights on:
- Total Sales, Orders, Quantity, Ratings  
- User Gain vs User Loss  
- Food Category Performance (Veg, Non-Veg, Others)  
- City-level Sales Ranking  
- Year-over-Year Sales Trends  
- User Demographics (Age Distribution)

The goal is to convert raw datasets into meaningful insights to support marketing, operations, and strategic decision-making.

---

## Problem Statement
Zomato works across many cities and needs a clear way to understand platform performance.  
This dashboard answers the following business questions:

1. **Which cities are performing well and which are underperforming?**  
2. **How many users are joining vs leaving the platform?**  
3. **Which food categories contribute the most revenue?**  
4. **How are sales trending across multiple years?**  
5. **Which age groups form the largest user segments?**

This solves the problem of manually analyzing multiple datasets by bringing everything into a unified analytical dashboard.

---

## Dataset

| File Name        | Description |
|------------------|-------------|
| restaurant.xlsx  | Restaurant details and locations |
| users.xlsx       | User demographic details |
| orders.xlsx      | Order-level transaction data |
| orders_type.xlsx | Food type/category information |
| food.xlsx        | Food ratings and sales data |

Dataset totals:  
- 150K+ Orders  
- 148K+ Ratings  
- 78K+ Active Users  
- 987M+ Total Sales  

---

## Tools and Technologies
- Power BI Desktop  
- Power Query  
- DAX  
- Excel  
- GitHub  

---

## Project Structure

```
zomato-powerbi-dashboard/
│
├── README.md
├── datasets/
│   ├── restaurant.xlsx
│   ├── users.xlsx
│   ├── orders.xlsx
│   ├── orders_type.xlsx
│   └── food.xlsx
│
├── dashboard/
│   └── zomato_dashboard.pbix
│
└── images/
    ├── overview.png
    ├── user_performance.png
    └── city_performance.png
```
---

## Data Cleaning
- Removed duplicates and null values

- Standardized city names 

- Ensured numeric columns had the correct data types 

---

## Data Modeling

Relationships in the model:

- **orders(r_id)** → **restaurant(id)**  
  

- **orders(r_id)** → **menu(r_id)**  
  

- **orders(user_id)** → **users(user_id)**  
  

This model enables analysis across restaurants, users, and food categories.

---

## DAX Measures

The following measures were created to support KPIs and charts:

- ActiveUser  
- UserCount  
- GainCustomers  
- LostCustomers  
- CurYear  
- CurYearSale  
- PrevYear  
- PrevYearSale  
- Sale_Value  
- Dynamic_Top_Title  
- Top_Sales  
- Order count  
- Rating count  

---

## Key Insights

### Business Insights
- Tirupati recorded the highest sales (42M+).  
- Non-Veg items have the highest revenue contribution (325M+).  
- User churn (33K lost) is significantly higher than user gain (12K added).  
- Users aged **20–30** are the most active demographic group.  
- Sales peaked in **2018**, followed by a slight decline.

### Operational Insights
- Sultanpur and Navrangpura show potential for improvement.  
- Highest restaurant ratings were observed in BTM Bangalore and Rohini Delhi.  

---

## Dashboard Output

This dashboard includes:
- Sales KPIs  
- City Performance Charts  
- User Gain vs Loss Cards  
- Food Category Sales Visuals  
- Annual Sales Trend Line Chart  
- Age-Based User Distribution  

To include screenshots, use:
![Dashboard Screenshot 1](https://github.com/karimshaik09/zomato-sales-and-user-analytics-dashboard-powerbi-project/blob/f3d182ceed7699e08fa66e21189e11a0bc6f4169/Image/Screenshot%202025-10-18%20215827.png)
![Dashboard Screenshot 2](https://github.com/karimshaik09/zomato-sales-and-user-analytics-dashboard-powerbi-project/blob/ed4018ef7567fd18c321b3adba564b0a05304b85/Image/Screenshot%202025-10-18%20215848.png)
![Dashboard Screenshot 3](https://github.com/karimshaik09/zomato-sales-and-user-analytics-dashboard-powerbi-project/blob/15cdc72be7f426216512d0c33d3007aec225d45a/Image/Screenshot%202025-10-18%20215916.png)

---

## How to Run This Project

1. Clone the repository:
```
git clone https://github.com/yourusername/zomato-powerbi-dashboard.git
```

2. Open **Power BI Desktop**  
3. Load the file `zomato_dashboard.pbix`  
4. Ensure the datasets are inside the `datasets/` folder  
5. Refresh the Power BI model  
6. Explore the visuals  

---

## Results and Conclusion

This project successfully highlights:
- High-vs-low performing cities  
- User growth and churn behavior  
- Sales contribution by food category  
- Long-term sales trends  
- User demographic patterns  

The dashboard makes decision-making easier for business teams.

---

## Future Work
- Add machine-learning based sales forecasting  
- Build user churn prediction model  
- Implement geospatial heatmaps  
- Integrate Zomato API for real-time data  
- Add restaurant-level profitability metrics  

---

## Author and Contact
Name: Shane Karimulla Shaik  
Email: karimshaik1905@gmail.com  
LinkedIn: [Karimulla Shaik
](https://www.linkedin.com/in/karimshaik17/)
 
