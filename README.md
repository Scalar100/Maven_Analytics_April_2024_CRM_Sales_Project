# Maven_Analytics_April_2024_CRM_Sales_Project

### Executive Summary
This project utilizes a dataset from the April 2024 [Maven Analytics Sales Challenge](https://mavenanalytics.io/challenges/maven-sales-challenge/8f59bcfa-d310-4947-b3d8-917b3cce270e). It presents an interactive Power BI dashboard tailored for sales managers to monitor their team's quarterly performance. The dashboard offers detailed tracking of performance metrics for managers and sales agents, segmented by sector, product, and location.

### Project Background
The B2B sales of computer hardware play a crucial role within the technology industry. To maintain a competitive edge, it's essential for businesses to understand sales trends, product performance, and client preferences. Utilizing data-driven insights is key to making informed decisions about inventory management, sales strategies, and targeted marketing.

As Data Analysts from **MavenTech**, a company dedicated to providing computer hardware to large enterprises. We fully recognize the power of Data Analytics to drive success in our business. Recently, we implemented a new CRM system, which has allowed us to accumulate extensive data on our sales opportunities. However, this data has been largely inaccessible outside the CRM platform.

In the Maven Sales Challenge, I have been tasked with the role of BI Developer. My objective is to assist **MavenTech** in becoming a truly data-driven organization. To achieve this, I will create an interactive dashboard designed to give our sales managers clear and actionable insights into their teams' quarterly performance. This tool will enable them to optimize their sales strategies, make better-informed decisions, and ultimately drive better business outcomes.

[Click to interact with the Power BI report](https://app.powerbi.com/view?r=eyJrIjoiNzQ1N2E0NjMtZTQ3My00MjRjLWI1YmUtM2JhYzJkOTNlNDZkIiwidCI6IjFkZDZlZmUxLTk4MDctNGM1Yy04NzJiLWJmZDExZDIyNGEzMSJ9)

### Overview of the Data
The data provided comprises several interconnected worksheets, each contributing essential information for analyzing a sales pipeline. The main worksheets include:
1. **Sales Pipeline**
2. **Sales Team**
3. **Products**
4. **Accounts**

#### Data Extraction and Transformation
The data was cleaned and transformed using both the Microsoft Excel and the Power Query Editor in Power BI. Key transformations included:
- **Removal of Duplicates**: Ensured the uniqueness of entries, especially in the `opportunity_id` column in the Sales Pipeline worksheet.
- **Column Trimming**: Unnecessary columns were removed to streamline the analysis. This ensured the focus was on relevant data.
- **Blank Rows Removal**: Blank rows were removed to maintain data integrity.
- **Text Formatting**: Columns such as `product` and `account` were cleaned, trimmed, and capitalized to ensure consistency.
- **Header Promotion**: Ensured that the first row of each column was promoted to header status for clarity.
- **Column Renaming**: Columns were renamed for better readability.
- **Creating Tables**: Data on each worksheet was transformed into table by using the Cntr-A then Cntr-T functions.
- **Creating Id**: Account ID,	Product ID, and	Sales Agent ID were created and linked to the other tables for easy generation of relationship on Power BI.
- **Merging all data**: Data from the different worksheets were transferred into a single worksheet for easy usage.

#### Description of the Worksheets
1. **Sales Pipeline Worksheet**
   **Fields**:
     - `opportunity_id`: Unique identifier for each sales opportunity.
     - `sales_agent`: The sales agent handling the opportunity.
     - `product`: The product involved in the sale.
     - `account`: The company or client the sale is directed towards.
     - `deal_stage`: Current stage in the sales pipeline (e.g., Prospecting, Engaging, Won, Lost).
     - `engage_date`: Date when the engagement stage began.
     - `close_date`: Date when the deal was closed.
     - `close_value`: Revenue generated from the deal.
2. **Sales Team Worksheet**
3. **Products Worksheet**
4. **Accounts Worksheet**
   
#### Data Dictionary
The data dictionary provides detailed descriptions for each field across all worksheets to ensure clarity and consistency in understanding and using the data.

The CSV files used as well as the one containing all the data from the rest and the dashboard generted in this project have been included in the repository.

### Tools and Technologies Used
1. **Power BI**: The primary tool used in this project was Power BI, which facilitated the creation of visualizations and dashboards to extract and display insights from the data. I also utilized the Power BI service, enabling the generation of an interactive web link for seamless navigation and interaction with the report.
2. **Power Query Editor**: An advanced feature of Power BI, Power Query Editor was employed for data transformation and cleaning. This tool was used to perform various operations such as removing duplicates, eliminating blank rows, formatting columns, and replacing values across different columns.
4. **Microsoft Excel**: Microsoft Excel played a crucial role at the beginning of the project. It helped in the understanding of the data structure as well as some light data cleaning. It also served as a guide for subsequent data transformations using the Power Query Editor.

#### Project Workflow
1.	Data Understanding and Preparation: Initial exploration and light cleaning of the data using Microsoft Excel to understand its structure.
2.	Data Transformation and Cleaning: Further data cleaning and transformation using Power Query Editor in Power BI to prepare the dataset for analysis.
3.	Dashboard Development: Creation of the interactive dashboard in Power BI, incorporating various visualizations to represent sales performance metrics.
4.	Analysis and Insights: Analysis of the visualized data to derive insights into sales trends, product performance, and sector-specific performance metrics.
5.	Deployment: Publishing the dashboard to the Power BI service, making it accessible via an interactive web link.

#### Project Objective:
The objective of this project is to analyze the sales pipeline data and provide actionable insights to optimize sales strategies, enhance team performance, and improve business outcomes. By leveraging data from various sources including the sales pipeline worksheet, sales team worksheet, products worksheet, and accounts worksheet, the project aims to:
1.	Identify key trends and patterns in sales activities, such as top-performing products, high-value accounts, and effective sales agents.
2.	Analyze the effectiveness of different sales strategies and stages in the sales pipeline to streamline the sales process and maximize conversion rates.
3.	Provide recommendations for resource allocation, sales team management, and product pricing based on data-driven insights.
4.	Enable informed decision-making by stakeholders at various levels of the organization, from sales managers to executives, through intuitive visualizations and clear presentations of findings.
Ultimately, the goal is to empower the organization to make data-driven decisions that drive growth, increase revenue, and strengthen competitiveness in the market.

### Data Collection
The data for this project was obtained from the official [**Maven Analytics** website](https://mavenanalytics.io/challenges/maven-sales-challenge/8f59bcfa-d310-4947-b3d8-917b3cce270e). It includes sales opportunities from various accounts, encompassing multiple regions and industries. The dataset provides key metrics such as account details, product information, sales team data, and the status of each sales opportunity, as outlined in the data overview above.

### Data Model
The data model was automatically generated in Power BI. It automatically detected the relationships and cardinality between the various tables used in this project.


