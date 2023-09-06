# Product-Sales-Dashboard-using-Excel

## Project Overview
This Excel dashboard project was crafted to dissect data from a fictional coffee company. The initial data is segregated into three worksheets: Orders, Customers, and Products, each holding key insights into the company's operations.
![Dashboard png](https://github.com/AImmanuel/Product-Sales-Dashboard-using-Excel/assets/141285116/1577412e-40cb-4ca9-b2e7-e2ec304bac52)

## Features
- **Data Analysis:** Gain insights into customer behavior, product profitability, and order trends.
- **Interactive Dashboard:** Easily navigate through data and customize your analysis.
- **Visualizations:** Visualize data using charts and graphs to make informed decisions.

## Data Sources
- **Orders:** Contains information about orders, including Order ID, Order date, Customer ID, and Product ID.
- **Customers:** Provides details about customers, such as Customer ID, Customer Name, Email, Phone Number, and more.
- **Products:** Includes information on coffee products, including coffee type, Roast type, size, unit price, and profit.

## Data Transformations
In the process of preparing the data for analysis, the following transformations were applied:

- **Customer Data Integration:** Customer Name, Email, and Country were added to the Orders worksheet using the XLOOKUP function, matching on the Customer ID column.
- **Product Data Integration:** Coffee Type, Roast Type, Size, and Unit price were filled in from the Products worksheet using the INDEX and MATCH functions.
- **Sales Calculation:** The Sales column was calculated by multiplying the Unit Price and Quantity from the Orders worksheet.
- **Coffee Type and Roast Type Abbreviations:** Abbreviations in the Coffee Type and Roast Type columns were expanded using the IF function. 

## Pivot Tables
To create meaningful graphs and filters for the dashboard, the following Pivot Tables were built:

**Total Sales Pivot Table**
- Rows: Years and months from the Order Date column in the Orders table.
- Columns: Coffee type names from the Coffee Type Names column in the Orders table.
- Values: Sales from the Orders table.

**Country Bar Chart Pivot Table**
- Rows: Country names from the Country column in the Orders table.
- Values: The sum of sales for the three countries (United States, Ireland, and United Kingdom).

**Top 5 Customers Pivot Table**
- Rows: Customer Names.
- Values: Sum of Sales for each customer from the Orders table.
- Sorting: Customers are sorted by the largest sales first, and only the top five are displayed.

## Graphs and Filters
The Excel dashboard includes the following graphs and filters:

- **Total Sales Line Chart:** Represents Total Sales (in USD) over Time, with four lines for the four different coffee types. 
A timeline allows users to select specific months or years to display on the graph. Additional filters include Size, Loyalty Card (Yes/No), and Roast Type Name.

- **Sales by Country Bar Graph:** Shows the total sales by country, influenced by the filters and timeline.

- **Top 5 Customers Bar Graph:** Displays the top 5 customers based on sales, and it is affected by the filters and timeline.

## Technologies and Functions Used
- **Microsoft Excel:** Used for data processing, analysis, visualization, and dashboard creation.
- **XLOOKUP:** Used to search for specific information (such as Customer Name, Email, and Country) based on the Customer ID and populate these details in the respective columns, enhancing the dataset for analysis.

## Usage
Navigate through the different worksheets (Orders, Customers, and Products) to explore the data.
Utilize the Pivot Tables to create graphs and apply filters for deeper insights.
Interact with the dashboard to analyze sales data, customer behavior, and product performance.
Refer to the visualizations and data to make informed decisions.

## Results/Insights
- Identify sales trends for different coffee types over time.
- Analyze the impact of loyalty cards on customer spending.
- Discover the top-performing countries and customers.
- Gain insights into product preferences and profitability.
- Use filters to customize your analysis and uncover actionable insights.


