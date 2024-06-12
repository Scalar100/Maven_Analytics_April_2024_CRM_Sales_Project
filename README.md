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

### Data Extraction and Transformation
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

### Description of the Worksheets
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
5. **Data Dictionary**:
   - `The data dictionary provides detailed descriptions for each field across all worksheets to ensure clarity and consistency in understanding and using the data.

The CSV files used as well as the one containing all the data from the rest and the dashboard generated in this project have been included in the repository.

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

### Data Analysis & Visualization:
After the completion of the data cleaning and preparation, I proceeded to analysis and visualization. To ensure easy navigation and adequate understanding of the project, I divided the visualizations into 4 dashboards. These dashboards were used to effectively visualize key insights from this analysis.

Some Key Insights from the data visualization are summarized below:

1.	**Overview**: The overview section shows that a total of $10.01 million was generated in the sales of 7 (seven) products all made by 35 (thirty-five) sales agents. Darcel Schlecht from Central Regional office generated the most revenue ($1.15 million), 11.48% of the total revenue. GTX Pro also churned out a massive $3.5 million revenue, placing it as the top performing product with approximately 35% of the total revenue. Revenue generated at the sector level were well above $1.0 million as seen in Retail ($1.87 million), Technology ($1.52 million), Medical ($1.36 million), Software ($1.08 million). Other sectors generated a cumulative revenue less than $1.0 million. Kan Code also led the charts in the “Top Revenue by Clients”, Melvin Marxen also topped the Charts as the best Manager in terms of cumulative Revenue generated.
2.	**Time Analysis**: The Time Analysis shows that June and September generated the most sales with $1.02 million and $1.01 million respectively. The Quarterly Trend shows an increase in total revenue from Q1 to Q2, 36.86% increase was experienced. The Revenue dropped from $2.97 million in Q2 to $2.79 million in Q3 and further to $2.07 million in Q4. All Managers generated their most Revenues in Q2 except for Rocco Neubert and Summer Sewald who generated the most Revenue in Q3. Most Deals were won in Q2 and most were lost in Q3.
3.	**Location Analysis**: A total of 15 countries were explored across North America, Africa, Asia, Europe, and South America. United States came out on top with an outstanding ($8.4 million), amassing a whooping 84% of the total revenue generated. Korea, Jordan and Panama are second on the list with $0.2 million generated each. 

#### Recommendations:
1. **Refine Sales Strategies**: Utilize insights from the analysis to refine sales strategies, prioritizing high-performing products and target accounts. Direct resources towards strategies and products that yield the highest return on investment, as evidenced by the significant revenue generated by top-performing products such as GTX Pro. Rapt attention should be paid to geographic regions showing high revenue potential. Focus on markets like the United States, which emerged as the top revenue generator, while also considering opportunities in regions like Korea, Jordan, and Panama, where significant revenue was also observed.
3. **Optimize Sales Team Management**: Identify top-performing sales agents within each region like Darcel Schlecht and Melvin Marxen and provide them with additional training, support, and incentives to maintain and enhance their performance. Address underperforming areas by offering targeted coaching and support, informed by insights from the analysis.
5. **Enhance Customer Engagement**: Customize customer engagement approaches based on regional preferences and behaviors identified through the analysis. Develop localized marketing campaigns and promotions to resonate with customers in various countries, enhancing products visibility.
7. **Monitor Performance Metrics**: Implement region-specific performance metrics to track sales effectiveness and customer engagement across different geographical areas. Utilize dashboards and reports to gain real-time visibility into regional performance trends and adapt strategies accordingly.

#### Conclusion:
In conclusion, the analysis of the sales pipeline data has provided valuable insights into sales performance, customer behavior, and market trends. By leveraging these insights, the organization can make informed decisions to optimize sales strategies, improve team performance, and boost products’ visibility.
Moving forward, it is essential to continue refining and adapting sales strategies based on ongoing analysis and feedback. By maintaining a data-driven approach to sales management and customer engagement, the organization can position itself for continued success and growth in the competitive marketplace.
Overall, the project has demonstrated the power of data analytics in driving business outcomes and also stressed the importance of leveraging data to make strategic decisions that drive value and impact across the organization.

#### About:
This data analysis project aims to extract actionable insights from sales pipeline data to optimize sales strategies, enhance team performance, and improve customer satisfaction. By analyzing metrics such as deal stage progression, sales agent performance, and product sales, the project seeks to empower the organization with data-driven recommendations for strategic decision-making. Through a combination of data analysis techniques and visualization tools, this project aims to drive growth and efficiency within the sales process while maintaining a competitive edge in the market.
 
