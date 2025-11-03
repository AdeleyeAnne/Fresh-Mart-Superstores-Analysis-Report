 ## 📊 Excel Fresh-Mart-Superstores-Analysis-Report
 
#### Focus Areas: 

 Sales performance, profit margin, customer segmentation, and payment trends — all analyzed to support data-driven decision-making.

## 📋Project Topic:Fresh-Mart-Superstores

## Business Problem

The supermarket chain operates multiple branches across different cities and manages a wide range of product lines, payment methods, and customer categories. However, management faces challenges in understanding key sales drivers and identifying performance gaps across locations and customer groups.

Despite having consistent transaction records, the organization lacks a comprehensive analytical view that connects sales trends, customer behavior, and payment preferences. Decisions are often made based on intuition rather than data-backed insights.
- The company needs to answer critical business questions such as:
- Which city or branch generates the highest sales and gross income?
- How do sales vary between customer types (Members vs Normal) and gender groups?
- What are the most profitable product lines and most preferred payment methods?
- At what time of the day and on which days are sales highest?
- Without clear insights into these questions, the business risks:
- Missing revenue opportunities due to poor timing or inventory planning
- Inefficient marketing strategies that fail to target high-value customer groups
- Low operational efficiency across branches
- Inability to track profitability trends and adapt to customer preferences

To address these challenges, a data-driven analysis using Power BI was conducted on a dataset comprising five dimension tables and one fact table (1,000 rows). The report focuses on revenue trend analysis, customer segmentation, and order/time-series analysis to uncover actionable insights that will support better decision-making and improve overall business performance.

## 📉Business Objective Summary

- The main objective of this analysis is to gain insights into sales performance, customer segmentation, payment preferences, and time-based purchasing behavior across multiple supermarket branches.
- The goal is to help management make informed, data-driven decisions to improve sales, enhance customer experience, and optimize operations.
- To visualize overall business performance in terms of total revenue, total gross income, and branch comparison over time.
- To understand customer demographics, membership behavior, and product preferences that drive sales

  ### Setting Clear Metrics
* A dedicated Measure Table was created in Power BI using DAX to compute KPIs such as:
   - Total Revenue
   - Total Gross Income
   - Total Orders
   - Average Rating
   - City performance indicator
### 💻Tools Used
- Power Query(for Cleaning)
- PowerBi( For analysis and visualization)
- Power point (For reporting)
 
  ### Gathering the Data
* The dataset was extracted from a ZIP folder and renamed as Assignment Project.
The files were imported into Power BI using Get Data from Excel.
They were transformed into Queries for further cleaning and preparation.

### Cleaning the Data
* Data preparation involved the following steps:
* Set the first row as headers in Sales, Customer, and Product tables.
* Removed duplicate transactions based on Invoice ID.
* Checked filters to confirm data consistency and uniformity.
* Validated the Quantity column for missing values or errors (none found; 100% accuracy).
* Created a Payment Dimension Table from the Sales Table.
* Renamed queries following a Fact-Dimension model structure.
* Added a conditional column for order time to support time-based analysis (morning, afternoon, evening).
* Established relationships in the Power BI Model View before proceeding to Report View for visualization.
  
### Dataset Overview
The dataset consists of one fact table and five dimension tables, with a total of 1,000 rows.
* Tables:
- Fact Table – Supermarket Sales (12 columns)
Contains key transactional data including sales, quantity, gross income, and ratings.
* Dimension Tables:
- City (3 columns) – holds information on branch location and city identifiers.
- Product (2 columns) – contains product line and category details.
- Payment (2 columns) – captures payment method and related details.
- Customer (3 columns) – holds customer type, gender, and ID information.
- Calendar (5 columns) – includes date, day, month, quarter, and year fields for time-based analysis.
* This star-schema data model allows efficient analysis of sales trends, customer behavior, and revenue performance through different dimensions.

  
### 📋Analysis Tasks
1. What is the total revenue, total gross income, total orders, and average rating across all branches?
2.Which branch or city recorded the highest total sales and gross income, and how do they compare monthly?
3.How do sales and gross income differ between Member vs Normal customers, and does gender influence buying behavior?
4.Which product line generates the most revenue and has the highest customer ratings?
5.What are the most preferred payment methods among customers, and how do they relate to total sales and branch location?
6.Analyze daily and monthly sales trends — identify peak sales hours and top-performing months.
7.How many orders do we have each day? Are there any peak hours?
8.What time of the day do we get most orders? How much did we make in these times?
morning is 9am – 12noon
afternoon is 12 noon – 4pm
evening is 4pm – 9pm

###  Data Analysis and Key Insights
✅ Overall Performance
* Total Revenue: 323,000
* Total Gross Income: 15,000
* Total Orders: 5,510
* Average Rating: 6.97
✅ Branch / City Performance
* City with highest total sales: Naypyitaw (111,000)
* Followed by Yangon (106,000) and Mandalay (196)
* All cities show increased performance in January and March
✅ Customer Segmentation
* Member customers generated 164,223 in sales
* Normal customers generated 158,743
* Female customers made 2,869 purchases, slightly higher than Male with 2,641
*  → Female Members appear to be the most valuable customer group.
✅ Product Line Performance
* Food & Beverages had the highest revenue: 56,145
* Fashion Accessories received the highest customer rating: 1,251
✅ Payment Method Trends
* Most preferred: E-wallet with 345 customers
* Followed closely by Cash (344) and Credit Card (311)
* → Digital payments are rising across all branches.
✅ Sales Trends
* Best performing month: March – 25,771
* Peak sales hour: 2 PM – 3 PM
* Busiest day: Saturday
✅ Daily Orders
* Highest: Saturday (919 orders)
* Busy across weekdays, but slower on Monday (638 orders)
* Evening and afternoon hours show most transactions
✅ Time of Day Sales
* Morning (9am–12noon): 61,799
* Afternoon (12noon–4pm): 122,797
* Evening (4pm–9pm): 138,371
→ Evening is the strongest shopping period.

## Summary

This supermarket successfully generated 323k revenue with 15k gross income from 5510 orders.
Sales are strongest in:
- Evenings
- Weekends
- March
  
Naypyitaw is the top-performing city, with members and female customers contributing the highest revenue.
Food & Beverages are the most profitable products, and E-wallet is the most preferred payment method.
Evening hours and Saturdays experienced the highest sales activity

### Recommendation

Increase Staff During Peak Hours:
The analysis shows that evening hours (4 PM–9 PM) and weekends, especially Saturdays, record the highest customer traffic. Increasing staff during these periods will help reduce overcrowding, improve customer experience, and minimize waiting time.

Enhance Inventory Planning:
Maintain higher stock levels during peak sales periods and special occasions to prevent shortages and ensure smooth operations across branches.

Encourage Digital Payments:
Since E-wallet is the most preferred payment method, offering small discounts or loyalty points for digital transactions can increase adoption and speed up checkout time.

Target Key Customer Segments:
Develop marketing campaigns focused on members and female customers, as they represent the most consistent and profitable customer groups.

Replicate High-Performing Branch Strategies:
Analyze the operational strategies of the Naypyitaw branch and replicate its successful sales and customer engagement methods across other locations.

Introduce Festive and Occasional Incentives:
Offer special discounts, promotional bundles, or loyalty rewards during festive seasons and public holidays. This will attract more customers, boost sales, and enhance brand loyalty during high-traffic periods.

Automate Sales Reporting:
Implement real-time Power BI dashboards for ongoing monitoring of revenue, orders, and customer behavior to support timely, data-driven decisions.

Continuous Staff Training:
Provide regular training for staff on customer service, sales, and technology tools to maintain efficiency, improve customer relations, and ensure smooth service delivery.

### Conclusion

The supermarket sales report provides valuable insights into revenue trends, customer profiles, and time-based order patterns.
The data model of five dimension tables and one fact table enables flexible analysis across multiple perspectives.
Overall, the findings help management make smarter decisions on branch performance, product focus, and customer engagement strategies.


  
