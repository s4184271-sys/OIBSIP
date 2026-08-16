# OASIS INFOBYTE – Data Analytics Internship

## Task 1: Exploratory Data Analysis on Retail Sales Data

### Project Overview

This project was completed as part of my **Data Analytics Internship at OASIS INFOBYTE**.

The objective of this task was to perform Exploratory Data Analysis (EDA) on a retail sales dataset and identify meaningful patterns related to sales, profit, discounts, categories, regions, sub-categories, and customers.

### Dataset

The project uses a Superstore-style retail sales dataset containing **2,008 retail order records** covering the period **2022–2024**.

The dataset includes information such as:

- Order and customer details
- Order dates
- Customer demographics
- Product categories and sub-categories
- Regions
- Quantity
- Unit price
- Discount
- Sales
- Profit

### Tools & Technologies

- **Python**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **Jupyter Notebook / VS Code**

### EDA Performed

The analysis included:

1. **Data Understanding**
   - Dataset shape and structure
   - Data types
   - Missing-value analysis
   - Duplicate-value analysis
   - Descriptive statistics

2. **Statistical Analysis**
   - Mean and median comparison
   - Distribution and skewness observations
   - Correlation analysis

3. **Time-Series Analysis**
   - Monthly sales trends
   - Year-wise performance

4. **Category Analysis**
   - Order volume
   - Total sales
   - Total profit
   - Profit margin
   - Loss-making orders

5. **Regional Analysis**
   - Orders by region
   - Total sales by region
   - Average sales per order
   - Year-wise regional sales trends

6. **Sub-Category Analysis**
   - Order volume
   - Total sales
   - Average sales per order
   - Total profit
   - Profit margin
   - Loss rate

7. **Customer Analysis**
   - Unique customer count
   - Customer order frequency
   - Customer sales
   - Customer profit

8. **Demographic Analysis**
   - Gender distribution
   - Age-group analysis
   - Average order value by age group

9. **Discount & Profit Analysis**
   - Discount vs. profit correlation
   - Profit comparison across discount levels

### Key Findings

- **Office Supplies** generated the highest total sales and total profit among the three main categories.
- **Furniture** had the highest category-level profit margin.
- At the sub-category level, **Chairs** had the highest profit margin at approximately **16.71%** and the lowest loss rate at approximately **14.73%**.
- **Bookcases** also performed strongly, with a profit margin of approximately **14.07%** and a loss rate of approximately **15.32%**.
- **Art** combined relatively high sales and total profit with a strong profit margin of approximately **13.65%**.
- **Storage** generated the highest sales and total profit among the sub-categories.
- **Paper** had the lowest sub-category profit margin, at approximately **9.58%**.
- **Accessories** had the highest loss-making order rate, at approximately **28.14%**.
- The correlation between **Discount and Profit was approximately -0.06**, indicating a very weak negative linear relationship.
- **Unit Price and Sales** showed a stronger positive relationship, while **Quantity and Sales** also showed a positive relationship.
- **CUST-420** was one of the strongest customers in the analysis, combining high order frequency with the highest total sales among the customers examined.

### Data Quality Notes

The initial dataset inspection identified:

- **25 missing values** in `Customer_Age`
- **8 duplicate rows**

The missing age values were retained as missing for age-based analysis rather than being artificially imputed.

The duplicate rows were identified and documented while retaining the original records so that the analysis and accompanying project presentation remained consistent with the completed work.

### Conclusion

This EDA demonstrated how retail data can be explored from multiple business perspectives rather than relying only on descriptive statistics.

The analysis showed that **high sales volume does not always translate into high profitability**. Examining profit margins and loss rates alongside sales helped identify sub-categories that were more efficient and those that may require further investigation.

### Project Files

- `Retail_Sales_EDA.ipynb` – Complete Python EDA notebook
- `Retail_Sales_Dataset.csv` – Dataset used for the analysis

### Internship

**OASIS INFOBYTE – Data Analytics Internship**

**Task:** Task 1 – Exploratory Data Analysis on Retail Sales Data
