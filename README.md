🧾 Dynamic Retail Dashboard in Excel
📘 Overview

The Dynamic Retail Dashboard is an interactive and data-driven analytical tool built in Microsoft Excel to visualize and interpret retail business data.
It connects to datasets hosted on GitHub, utilizes Power Query for data ingestion and transformation, and provides actionable insights through dynamic charts, KPIs, and slicers.

This project helps businesses monitor sales performance, profitability, product trends, and regional insights, enabling smarter decision-making with visual clarity.

📊 Datasets Used

The dashboard is based on three key datasets — Orders, Returns, and People — all connected through Power Query for dynamic data refresh.

1️⃣ Orders Table

The Orders table contains comprehensive information about customer transactions, including product, shipment, and financial details.

Sample Data
Order ID	Order Date	Ship Date	Ship Mode	Customer ID	Customer Name	Segment	City	State	Country	Postal Code	Market	Region	Product ID	Category	Sub-Category	Product Name	Sales	Quantity	Discount	Profit	Shipping Cost	Order Priority
CA-2012-124891	31-07-2020	31-07-2020	Same Day	RH-19495	Rick Hansen	Consumer	New York City	New York	United States	10024	US	East	TEC-AC-10003033	Technology	Accessories	Plantronics CS510 - Over-the-Head monaural Wireless Headset System	2309.65	7	0	762.18	933.57	Critical
IN-2013-77878	05-02-2021	07-02-2021	Second Class	JR-16210	Justin Ritter	Corporate	Wollongong	New South Wales	Australia		APAC	Oceania	FUR-CH-10003950	Furniture	Chairs	Novimex Executive Leather Armchair, Black	3709.40	9	0.1	-288.77	923.63	Critical
IN-2013-71249	17-10-2021	18-10-2021	First Class	CR-12730	Craig Reiter	Consumer	Brisbane	Queensland	Australia		APAC	Oceania	TEC-PH-10004664	Technology	Phones	Nokia Smart Phone, with Caller ID	5175.17	9	0.1	919.97	915.49	Medium
ES-2013-1579342	28-01-2021	30-01-2021	First Class	KM-16375	Katherine Murray	Home Office	Berlin	Berlin	Germany		EU	Central	TEC-PH-10004583	Technology	Phones	Motorola Smart Phone, Cordless	2892.51	5	0.1	-96.54	910.16	Medium
2️⃣ Returns Table

Tracks orders that have been returned, along with the corresponding market details.

Sample Data
Returned	Order ID	Market
Yes	MX-2013-168137	LATAM
Yes	US-2011-165316	LATAM
Yes	ES-2013-1525878	EU
Yes	CA-2013-118311	United States
3️⃣ People Table

Contains sales representative details and the regions they manage.

Sample Data
Person	Region
Anna Andreadi	Central
Chuck Magee	South
Kelly Williams	East
Matt Collister	West
Deborah Brumfield	Africa
🧩 Problem Statements Solved with Steps
1️⃣ Key Performance Indicators (KPIs)

Objective: Calculate and display core business metrics like Total Sales, Total Profit, Total Quantity, Number of Orders, and Profit Margin dynamically.

Steps:

Import the Orders dataset via Power Query.

Create calculated columns:

Profit Margin = Profit / Sales

Total Orders = COUNT(Order ID)

Use Excel formulas to calculate key metrics:

Total Sales = SUM(Sales)

Total Profit = SUM(Profit)

Total Quantity = SUM(Quantity)

Build a KPI table using cell references and conditional formatting icons to highlight trends.

2️⃣ Sales and Profit Trend Analysis

Objective: Identify sales and profit performance patterns over time.

Steps:

Create a Pivot Table with Order Date grouped by Year and Month.

Add Sales and Profit as values.

Insert a Line Chart to visualize trends.

Apply Slicers for filtering by Category, Region, and Market.

3️⃣ Category-Wise Profit Analysis

Objective: Compare profit contributions from different product categories.

Steps:

Create a Pivot Table with Category as rows and Profit as values.

Sort results in descending order.

Insert a Bar Chart to visualize performance.

Add slicers for Market and Year filters.

4️⃣ Segment-Wise Sales Share (%)

Objective: Display the percentage share of sales from each customer segment.

Steps:

Create a Pivot Table with Segment as rows and Sales as values.

Show values as % of Grand Total.

Insert a Pie Chart or Donut Chart for visual representation.

Add data labels showing percentages.

5️⃣ Sales by Country

Objective: Analyze and compare sales performance across countries.

Steps:

Create a Pivot Table with Country as rows and Sales as values.

Sort data by descending order of Sales.

Use Conditional Formatting or Color Scales to highlight top countries.

Optionally, use a Map Chart for regional representation.

6️⃣ Top 5 Subcategories

Objective: Identify the top-performing subcategories in terms of sales.

Steps:

Create a Pivot Table using Sub-Category as rows and Sales as values.

Sort by Sales (Descending).

Apply a Top 5 Filter.

Visualize with a Column Chart.

⚙️ Dynamic Features

Power Query Integration: Automatically fetches and refreshes data from GitHub.

Interactive Slicers: Allow users to filter by Region, Market, Category, or Segment.

Dynamic Charts: Update in real-time as filters change.

KPI Indicators: Provide quick performance summaries for decision-makers.

Automated Calculations: Ensures consistency and reduces manual intervention.

🚀 Next Steps / Future Enhancements

Return Rate Analysis: Evaluate product returns by category or market.

Customer Profitability Study: Identify top and bottom customers.

Market Comparison Dashboard: Compare KPIs across regions.

Product-Level Deep Dive: Visualize sales and profit for individual products.

Integration with Power BI: For advanced analytics and storytelling dashboards.

📈 Business Significance

The Dynamic Retail Dashboard enables business teams to:

Track real-time performance across regions and segments.

Understand sales trends and profitability drivers.

Identify high-value markets and low-performing areas.

Make data-backed decisions for marketing, logistics, and inventory planning.

🧰 Tools & Technologies Used
Tool	Purpose
Microsoft Excel	Dashboard design, data analysis, KPIs, and visualization
Power Query	Data ingestion and transformation from GitHub
GitHub	Centralized data storage and version control
Pivot Tables & Charts	Summarization and visual analysis
Slicers & Conditional Formatting	Interactive exploration and highlighting trends
🧭 Project Workflow
graph TD
A[GitHub Dataset] --> B[Power Query in Excel]
B --> C[Data Cleaning & Transformation]
C --> D[Data Modeling & Relationship Building]
D --> E[Pivot Tables & KPIs]
E --> F[Interactive Dashboard & Insights]

🖼️ Visuals

This repository includes:

Screenshots of the final dashboard.

KPI visualization examples.

Chart views for category-wise profit, regional sales, and top subcategories.

Power Query transformation snapshots.

🏁 Conclusion

The Dynamic Retail Dashboard showcases the powerful combination of Excel + Power Query for real-world data analytics.
It demonstrates how even without coding, one can build automated, scalable, and insightful dashboards that empower retail businesses to make informed decisions and optimize performance.
