# Project: Domino's Pizza Sales Dashboard Analysis
![Pizza1](https://github.com/user-attachments/assets/b684345b-3b9b-4b31-afcf-e09bc5c7dd19)
![Pizza 2](https://github.com/user-attachments/assets/31f00d65-6e15-4239-8064-3ebb673daddd)

Project Overview
This project involves the analysis of a Domino's Pizza sales dataset to uncover key business insights and performance metrics. The goal was to translate raw sales data into an interactive dashboard (represented in this PDF) that highlights sales trends, customer ordering behavior, and product performance. This analysis aids in strategic decision-making for inventory management, marketing, and menu optimization.

Key Performance Indicators (KPIs)
The dashboard tracks several high-level KPIs that provide a snapshot of overall business health:

• Total Revenue: $873,803.20

• Average Order Value: $40.93

• Total Pizzas Sold: 52,979

• Total Orders: 21,350

• Average Pizzas Per Order: 2.48

Tools & Methods
• Data Analysis & Processing: Likely performed using SQL for data extraction and aggregation, or Excel/Power Query for data cleaning and transformation.

• Data Visualization: The final dashboard was created using a BI tool like Tableau, Power BI, or Looker Studio to create interactive charts and graphs.

• Business Intelligence: The project follows a standard BI workflow: Data Sourcing -> Cleaning -> Analysis -> Visualization -> Insight Generation.

Key Insights & Analysis
1. Sales & Order Trends

• Peak Business Days: Orders are highest on Fridays and Saturdays, indicating strong weekend demand. Evenings are the busiest time.

• Seasonal Trends: The months of May and July show the highest number of orders, suggesting potential seasonal promotions or factors influencing demand.

2. Product Performance

• Top Category: The "Classic" pizza category is the highest contributor to both total sales and total orders.

• Preferred Size: Large-sized pizzas generate the maximum revenue, aligning with the high average number of pizzas per order (2.48).

3. Best & Worst Sellers

• Revenue Champion: The Thai Chicken Pizza is the top-performing pizza in terms of revenue generation.

• Quantity & Orders Champion: The Classic Deluxe Pizza is the most frequently ordered pizza, leading in both total quantity sold and total number of orders.

• Consistent Underperformer: The Brie Carre Pizza is the poorest performer across all key metrics: revenue, quantity sold, and total orders.

Business Implications & Recommendations
Based on the insights from this dashboard, the following strategic actions can be recommended:

• Inventory & Supply Chain: Focus inventory planning for "Classic" category ingredients and large-size pizza bases, especially on weekends and during May/July.

• Marketing & Promotions:

Create featured deals or "Meal of the Day" offers around top-selling pizzas like the Thai Chicken and Classic Deluxe.

Consider bundling or discounting low-performing pizzas (like the Brie Carre) to clear inventory or introduce them to a wider audience.

• Menu Optimization:

Highlight best-selling pizzas on the menu and in promotional materials.

Evaluate whether the worst-performing pizzas should be retained, re-branded, or removed from the menu to simplify operations.

• Staffing: Schedule more staff during weekend evenings and the peak summer months (May, July) to handle the increased order volume efficiently.

SQL Analysis Structure
A. Key Performance Indicators (KPIs)
sql
-- Total Revenue, Average Order Value, Total Pizzas Sold
-- Total Orders, Average Pizzas Per Order
B. Trend Analysis
Daily Trends: Order patterns by day of week

Monthly Trends: Seasonal performance analysis

C. Product Performance
Sales by Category: Revenue distribution across pizza types

Sales by Size: Performance analysis by pizza size

Quantity by Category: Volume analysis per category

D. Best & Worst Performers
Top/Bottom 5 by Revenue

Top/Bottom 5 by Quantity

Top/Bottom 5 by Total Orders

🔍 Key SQL Insights
Business Metrics
Total Revenue: $873,803.20

Average Order Value: $40.93

Total Pizzas Sold: 52,979

Total Orders: 21,350

Average Pizzas Per Order: 2.48

Performance Trends
Peak Days: Friday/Saturday evenings

Peak Months: May and July

Top Category: Classic pizzas (45.9% of revenue)

Top Size: Large pizzas

Product Analysis
Revenue Leader: Thai Chicken Pizza

Volume Leader: Classic Deluxe Pizza (quantity & orders)

Underperformer: Brie Carre Pizza (across all metrics)

📈 Business Impact
Operational Insights
Inventory Management: Focus on Classic category and Large size ingredients

Staff Scheduling: Increase capacity during weekends and summer months

Menu Optimization: Identify underperforming products for review

Strategic Decisions Supported
Product performance tracking

Seasonal demand forecasting

Menu optimization and pricing strategies

Marketing campaign targeting

🚀 Technical Achievements
SQL Expertise Demonstrated
Complex aggregations and calculations

Date/time manipulation functions

Advanced filtering and sorting

Subqueries for percentage calculations

Data type conversions and formatting

Data Processing Capabilities
sql
-- Example of complex calculation:
CAST(CAST(SUM(quantity) AS DECIMAL(10,2)) / 
CAST(COUNT(DISTINCT order_id) AS DECIMAL(10,2)) AS DECIMAL(10,2))
AS Avg_Pizzas_per_order
