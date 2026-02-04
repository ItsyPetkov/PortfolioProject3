# Coffee Sales Intelligence Dashboard – Product, Market & Performance Optimization Study

This portfolio project is based on coffee sales data provided by a local retailer. Exploratory Data Analysis (EDA) is performed on transactional data to isolate and understand specific trends and patterns that support strategic decision-making, revenue optimisation, and sustainable business growth. This project is produced in its entirety solely using MS Excel.

## Target User: Business Owner/Potential Stakeholders

This analysis is designed for people looking to enter the coffee retail market or to expand their business by investigating sales data. It provides actionable insights such as buying behaviour, high-volume vs. high-value comparison, loyalty program effectiveness, price-volume tradeoffs, growth trends and seasonal coffee paterns.

## Understanding the Data

The data for this project consists of three sperate spreadsheets: Orders, Customers, Products

<table>
<tr>
<td valign="top">

**Orders Table**

| Column Name | Data Type |
|-------------|------------|
| Order ID    | Text       |
| Order Date  | Date       |
| Customer ID | Text       |
| Product ID  | Text       |
| Quantity    | Number     |

</td>
<td valign="top">

**Customers Table**

| Column Name   | Data Type |
|---------------|------------|
| Customer ID   | Text       |
| Customer Name | Text       |
| Email         | Text       |
| Phone Number  | Text       |
| Address Line 1| Text       |
| City          | Text       |
| Country       | Text       |
| Postcode      | Text       |
| Loyalty Card  | Text       |

</td>
<td valign="top">

**Products Table**

| Column Name   | Data Type |
|---------------|------------|
| Product ID    | Text       |
| Coffee Type   | Text       |
| Roast Type    | Text       |
| Size          | Number     |
| Unit Price    | Number     |
| Price per 100g| Number     |
| Profit        | Number     |

</td>
</tr>
</table>

The data obtained from the spreadsheets presented above is processed into a single spreadsheet called "Working Sheet". In fact, this is the sheet used for all of the visuals and the analysis conducted in this project. For additional details, please read the information provided in the Data Analysis Framework section.

## Data Analysis Framework

The contents of the "Working Sheet" were processed through the following set of cleaning and transformation steps:

* Data gathering using XLOOKUP for the Customer data and INDEX MATCH for the product data
* Column population with derived metics using regular formulas (e.g. Sales = Unit Price * Quantity)
* Transformation of coffee types and raost from their abreviations to entire words using multiple NESTED IF statements (e.g. Lib -> Liberica, D -> Dark)
* Formatting column contents using custom formats (e.g. 'dd-mmm-yyyy' for dates and 0.0 'kg' for units)
* Addition of currency labels ($) for the Unit Price and the Sales columns
* Duplicate checking and removal
* Converting the spreadsheet range into a table

Next stages involve data visualisation by producing dynamic, interactive dashboards in MS Excel and data storytelling by producing a comprehensive analysis report using MS PowerPoint. The output of the last step is available in the GitHub repo under 'Stakeholder report.pptx'.

## Analytical Focus & Key Business Questions

This section contains questions important to the business owner. According to them, they are worth exploring and may provide insights on how to improve strategic decision-making, revenue optimisation, and support sustainable business growth over significant periods of time.

List of business-related enquiries and their relevance:

* *Which coffee products generate the most revenue and volume? How does this vary across countries?* => Helps decide where to double down (best-selling Stock Keeping Units (SKU) by market) and whether certain coffee types should be promoted, expanded, or retired in specific countries.

* *Who are the most valuable customers, and what purchasing patterns distinguish them?* => Identifies high-value customers to target with retention, loyalty perks, or premium offerings.

* *Does the loyalty card program meaningfully increase customer spend or purchase frequency?* => Provides a direct evaluation of the Return Of Investment (ROI) metric associated with the loyalty program.

* *How do pricing, package size, and unit combinations influence sales performance?* => Supports decisions around pricing strategy, bundle sizing, and margin optimization.

* *What are the key sales trends over time, and are there any seasonal patterns?* => Enables better demand forecasting, inventory planning, and campaign timing.

<!-- This is a project aiming to develop a pipeline of data pre-processing and analysis within Excel. It consists of two different dataset and thus two different dashboards are created (one is begginer-friendly and the other demonstrates more advanced concepts)

Topics that are covered in this exploration include:

1.Pivot Tables

2.Functions and formulae -> MIN(), MAX(), SUM(), POW(), SQRT(), AVG(), IF(), IFS(), LEN(), LEFT(), RIGHT(), TEXT(), TRIM(),
CONCATENATE(), SUBSTITUTE(), SUMIF(), SUMIFS(), COUNT(), COUNTIF(), COUNTSIFS(), DAYS(), MONTHS(), YEARS(), NETWORKDAYS(),
UPPER(), LOWER(), PROPER(), INDEX()

3.XLOOKUP and VLOOKUP

4.Conditional Formatting

5.Charts

6.Data Cleaning in Excel

Excel Project Dataset.xlsx Dashboard:
![image](https://github.com/user-attachments/assets/2a178b71-4fad-41c9-955e-77e1f15ce7da)

coffeeOrdersData.xlsx Dashboard:
![image](https://github.com/user-attachments/assets/c1bc272e-d77f-440f-b68c-940f66be6eb1) -->
