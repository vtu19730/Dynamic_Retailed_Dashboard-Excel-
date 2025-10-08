🧾 Dynamic Retail Dashboard (Excel Data Science Project)
📖 Overview

The Dynamic Retail Dashboard is an interactive Excel-based analytical solution designed to visualize and analyze retail business performance.
This project demonstrates data science principles applied within Excel, including data ingestion, transformation, and dynamic visualization.
It provides actionable insights into sales, profit, and shipping performance across multiple regions and markets.

🎯 Objective

The primary goal of this project is to:

Analyze retail data efficiently using Excel’s data science tools.

Develop an interactive and automated dashboard to track sales trends, customer segments, and product performance.

Enable data-driven decision-making for business stakeholders through dynamic filters and KPIs.

🧩 Dataset Description

The dataset consists of three related tables — Orders, Returns, and People.
All datasets are ingested directly from GitHub, ensuring centralized version control and automatic refresh capability.

1️⃣ Orders Table

Contains details about each retail transaction.

Column Name	Description
Order ID	Unique identifier for each order
Order Date / Ship Date	Dates for order placement and shipping
Ship Mode	Type of delivery (e.g., Same Day, First Class, Second Class)
Customer ID / Name	Unique customer identifier and name
Segment	Business category (Consumer, Corporate, Home Office)
City / State / Country / Postal Code	Customer’s geographical details
Market / Region	Market classification (e.g., APAC, EU, US)
Product ID / Category / Sub-Category / Product Name	Product-related details
Sales	Revenue generated from the sale
Quantity	Number of units sold
Discount	Discount percentage applied
Profit	Net profit from the order
Shipping Cost	Cost incurred for shipping
Order Priority	Urgency level (e.g., Critical, Medium)
Sample Data:
Order ID	Order Date	Ship Date	Ship Mode	Customer Name	Segment	Country	Product Category	Sales	Profit	Shipping Cost
CA-2012-124891	31-07-2020	31-07-2020	Same Day	Rick Hansen	Consumer	United States	Technology	2309.65	762.18	933.57
IN-2013-77878	05-02-2021	07-02-2021	Second Class	Justin Ritter	Corporate	Australia	Furniture	3709.39	-288.76	923.63
2️⃣ Returns Table (To be added after data sample shared)

Contains information on returned orders and reasons for return.

Column Name	Description
Order ID	ID of the returned order
Returned	Indicates whether the order was returned (Yes/No)
Return Reason	Explanation or reason for the return
3️⃣ People Table (To be added after data sample shared)

Stores sales representative information by region.

Column Name	Description
Region	Regional sales zone
Person	Name of the person handling sales in that region
🔗 Data Ingestion

All data sources are hosted on GitHub.

The data is connected to Excel via Power Query, allowing:

Direct online refresh

Automatic schema updates when data changes

Version-controlled data management

⚙️ Workflow

Data Ingestion

Load all three tables (Orders, Returns, People) using Excel’s Get Data → From Web feature linked to GitHub.

Data Cleaning & Transformation

Standardize column names and formats (e.g., dates, numeric fields).

Merge datasets using common keys (Order ID and Region).

Handle missing values and filter invalid records.

Data Modeling

Define relationships among the three tables.

Create calculated columns (e.g., profit margin, sales per order).

Dashboard Creation

Build PivotTables and PivotCharts.

Add dynamic slicers for filters such as Region, Category, Segment, and Ship Mode.

Include KPIs like:

Total Sales

Total Profit

Average Shipping Cost

Return Rate

Visualization

Region-wise and Category-wise performance charts.

Trend analysis over time.

Top products and customers by revenue and profit.

📊 Dashboard Features

Dynamic Filters: Interactive slicers for market, region, and product category.

Automated Refresh: Updates automatically from GitHub data source.

Performance Metrics: KPIs for profit, sales, and shipping cost.

Visual Insights:

Profitability by segment

Return rates

Shipping performance

Product category analysis

🧠 Key Insights (Example)

The Technology category yields the highest sales across most regions.

Critical order priorities often incur higher shipping costs.

Corporate segment customers show greater bulk order volume but lower profit margins due to discounts.

Same Day shipping mode results in higher profit ratios despite increased shipping costs.

🧰 Tools & Technologies Used
Tool	Purpose
Microsoft Excel	Data analysis, Power Query, Dashboard creation
GitHub	Data source hosting and version control
Power Query	Data ingestion and transformation
Pivot Tables & Charts	Data summarization and visualization
Slicers & KPIs	Interactive analysis
🚀 How to Use

Clone or download this repository from GitHub.

Open the Excel workbook.

Go to Data → Refresh All to load the latest data from GitHub.

Use the slicers and filters to explore sales insights dynamically.

🔮 Future Enhancements

Integration with Power BI for advanced visualization.

Predictive analytics (e.g., sales forecasting using regression).

Automated email reports and alerts.

Add more performance metrics like profit per region or shipping efficiency.

🏁 Conclusion

The Dynamic Retail Dashboard demonstrates how Excel can be leveraged beyond traditional spreadsheets — acting as a powerful data analytics and visualization tool.
Through structured data ingestion, transformation, and modeling, this dashboard empowers business users to gain quick, actionable insights with minimal effort.
