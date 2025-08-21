# SALES ANALYSIS PROJECT
### PROJECT OVERVIEW
To derive meaningful insights and patterns from sales data, that can inform strategic business decisions.
### DATA SOURCE
sales_data_csv [Download here](https://github.com/SomtooNkannebe/Data_Analysis_Projects/blob/main/Sales%20Data.csv))

### TOOLS
- Python - For Clearning and Analysis.
- Power BI - For viturialization. 

### DATA CLEANING / PREPARATION
In the initial data preparation Phase we prepared the following task. 
1. Data loading and inspection.
2. Handling missing values.
3. Data cleaning and formating.

### EXPLORATING DATA ANALYSIS QUESTIONS
-  What is the distribution of orders across different regions?
-  Identify the top 5 cities with the highest number of orders?
-  What are the most popular product categories based on sales?
-  Identify the top 5 selling products?
  
### DATA ANALYSIS
some python codes
- Identify the top 5 cities with the highest number of orders?
```python
 orders_across_different_cities=df.groupby('City')['Order ID'].count()
print(orders_across_different_cities.sort_values(ascending=False).head(5))
```
- What are the most popular product categories based on sales?
``` Python
 popular_product1=df.groupby('Product')['Sales'].sum()
 print(popular_product1.sort_values(ascending=False))
```
- Identify the top 5 selling products?
``` python
popular_product1=df.groupby('Product')['Quantity Ordered'].sum()
 print(popular_product1.sort_values(ascending=False).head(5))
```
### RESULTS / FINDINGS
- Top 5 cities with the highest number of orders:
  - San Francisco
  - Los Angeles
  - New York City
  - Boston

![Top Cities by Orders](https://github.com/SomtooNkannebe/Data_Analysis_Projects/blob/main/salesdata2025%20(4).jpg)

- Top 5 most Popular product
  - AAA Batteries (4-pack).
  - AA Batteries (4-pack).
  -  USB-C Charging Cable.
  -  Lightning Charging Cable.
  -  Wired Headphones.
    
- less indemands product include the following:
  - Lg Dryers.
  - Lg washing machines.
  - Thinkpad Laptops

### RECOMENDATIONS
- AAA Batteries (4-pack) should be avalible always.
- Pomotions and discounts should be done on months with lower sales and on less popular product to increase demand
- The product cost prices should be entered in to check if profit or loss is been after the year.
- Underperfoming product should be review and possibly phase out.
