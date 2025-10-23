# Cafe Sales Analysis — Exploratory Data Analysis (EDA)

### Project Overview
This EDA project explores and analyzes sales data from a cafe to uncover patterns, customer preferences, and revenue-driving insights.
Through a structured EDA process, we clean, transform, and visualize transactional data using Python to support better business decisions in inventory, pricing, and operations.

---

### Dataset Overview
- **Source:** Kaggle
- **Total Records:** 10,000  
- **Columns:** 8 (Transaction ID, Item, Quantity, Price per Unit, Total Spent, Payment Method, Location, Transaction Date)  
- **Time Period:** January 2023 to December 2023 — a full year of cafe transactions.
- **Key Variables:**  
  - `Quantity` — Number of items sold  
  - `Price Per Unit` — Selling price of each item  
  - `Total Spent` — Total amount spent per transaction  
  - `Transaction Date` — Timestamp of purchase

---
    
### Project Objective
- Understand sales trends across days, weeks, and months.  
- Identify top-performing and low-performing items.  
- Compare weekday vs weekend sales performance.  
- Detect and handle missing values and outliers effectively.  
- Generate insights to support marketing and inventory strategies.

---

### Workflow Process

#### 1. Data Loading & Initial Overview
The dataset was loaded to understand its structure, shape (10,000 rows, 8 columns), and initial data types
#### 2. Data Cleaning & Preparation
- Missing values handled via imputation and column corrections.  
- Duplicate records verified — none found.  
- Data type conversions performed (`Transaction_Date` → datetime).  
- Outliers in **Revenue** detected using IQR and capped for stability.  
- New features engineered: `Year`, `Month`, `Day`, `Day_Name`, `Week`, `Is_Weekend`.
#### 3. Exploratory Analysis & Visualizations
- **Item-wise Sales:** Identified top items by revenue and quantity sold.  
- **Payment Insights:** Compared distribution of payment methods.  
- **Weekend vs Weekday Sales:** Quantified demand differences to highlight peak periods.  
- **Time Series Trends:** Analyzed daily fluctuations in transactions, revenue, and item quantity .  
- **Correlation Study:** Evaluated relationships among key metrics to uncover hidden patterns.
#### 4. Insight Generation
Findings were visualized to generate actionable business recommendations.

---

## Key Insights
1. **Juice & Salad** is the top-revenue-generating item, showing strong and consistent demand.  
2. **Cake and Smoothie** contribute high revenue despite lower sales volume — likely due to premium pricing.  
3. **Cookie and Tea** remain low-revenue, suggesting optional bundling or promotional potential.
4. **Digital Wallet** dominate payment methods
5. **Takeaway orders** slightly exceed **in-store orders**, suggesting a preference for off-premise dining
6. **weekdays sales outperform Weekend**, highlighting greater customer activity.
7. **June** recorded peak revenue, while **January and November** saw the lowest, indicating seasonal variation. 
8. Sales patterns are **volatile but stable overall** — no long-term decline or growth trend detected.

---

## Business Recommendations
- **Stock more high-performing items (Juice, Salad)** during weekends.  
- **Promote low-selling items** (Tea, Cookie) through combos or discounts.  
- **Plan staffing and inventory** around observed weekend spikes.  
- **Review pricing strategies** for premium items with high margins.  
- **Monitor time-based patterns** for seasonal marketing opportunities.

---

## Tech Stack
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Datetime  
- **Tools & Environment:** Jupyter Notebook, GitHub

---

## Repository Structure
```
cafe-sales-analysis/
│
├── README.md                 # Project overview, objectives, and insights
│
├── data/                     # Raw and cleaned datasets
│   ├── dirty_cafe_sales/     # Original CSV file
│   └── Cafe_Sales_Cleaned/   # Preprocessed datasets
│
├── notebooks/                # Jupyter notebooks for EDA and analysis
│   └── cafe.ipynb            # Final analysis notebook
│
├── visuals/                  # Plots, charts
```
---

## Future Scope
- Implement time-series forecasting (ARIMA, Prophet).  
- Analyze customer segmentation using clustering.  
- Build an interactive Power BI dashboard.

---

## About Me

Hi, I’m Simitha Ummer.

I’m a Data Science intern with a background in Botany, now focused on analytics and data-driven decision making. I specialize in Python, SQL, Power BI, and Excel, with experience in exploratory data analysis, dashboard development, and deriving actionable insights from complex datasets.

I’m passionate about building reproducible workflows, crafting clear visual narratives, and connecting insights across domains such as education, health, financial inclusion, and policy.

Feel free to connect with me on [LinkedIn](www.linkedin.com/in/simitha-ummer-69a848350) or explore more of my work on [GitHub](https://github.com/simitha2002).
