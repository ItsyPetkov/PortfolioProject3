# Coffee Sales Intelligence Dashboard – Product, Market & Performance Optimization Study

This portfolio project is based on coffee sales data provided by a local retailer. Exploratory Data Analysis (EDA) is performed on transactional data to isolate and understand specific trends and patterns that support strategic decision-making, revenue optimisation, and sustainable business growth. This project is produced in its entirety solely using MS Excel.

## Table of Contents
- [Target User](#target-user-business-ownerpotential-stakeholders)
- [Understanding the Data](#understanding-the-data)
- [Data Analysis Framework](#data-analysis-framework)
- [Analytical Focus & Key Business Questions](#analytical-focus--key-business-questions)
- [Key Insights & Strategic Action Recommendations](#key-insights--strategic-action-recommendations)
  	- [Question 1 Analysis Output](#question-1-analysis-output)
  	- [Question 2 Analysis Output](#question-2-analysis-output)
  	- [Question 3 Analysis Output](#question-3-analysis-output)
  	- [Question 4 Analysis Output](#question-4-analysis-output)
  	- [Question 5 Analysis Output](#question-5-analysis-output)


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

Next stages involve: 1) data visualisation by producing dynamic, interactive dashboards in MS Excel using PIVOT TABLES/CHARTS, SLICERS, TIMELINES and CONDITIONAL FORMATTING; and 2) data storytelling by delivering a comprehensive analysis report using MS PowerPoint. The output of both steps is available in the GitHub repository under 'coffeeOrdersData.xlsx' and 'Stakeholder report.pptx', respectively.

## Analytical Focus & Key Business Questions

This section contains questions important to the business owner. According to them, they are worth exploring and may provide insights on how to improve strategic decision-making, revenue optimisation, and support sustainable business growth over significant periods of time.

List of business-related enquiries and their relevance:

1. *Which coffee products generate the most revenue and volume? How does this vary across countries?* => Helps decide where to double down (best-selling Stock Keeping Units (SKU) by market) and whether certain coffee types should be promoted, expanded, or retired in specific countries.

2. *Who are the most valuable customers, and what purchasing patterns distinguish them?* => Identifies high-value customers to target with retention, loyalty perks, or premium offerings.

3. *Does the loyalty card program meaningfully increase customer spend or purchase frequency?* => Provides a direct evaluation of the Return Of Investment (ROI) metric associated with the loyalty program.

4. *How do pricing, package size, and unit combinations influence sales performance?* => Supports decisions around pricing strategy, bundle sizing, and margin optimization.

5. *What are the key sales trends over time, and are there any seasonal patterns?* => Enables better demand forecasting, inventory planning, and campaign timing.

## Key Insights & Strategic Action Recommendations

This section presents a concise overview of the patterns and trends revealed through Exploratory Data Analysis (EDA) in relation to each of the questions posed above, followed by recommendations derived from the findings. 

#### Question 1 Analysis Output					
																		
<img width="1240" height="681" alt="image" src="https://github.com/user-attachments/assets/d39d1ed3-c413-4f8d-ba92-6ba72242ed09" />

Key Insights:

* Mainstream coffees drive the highest unit volumes but generate 30–40% lower revenue per unit compared to premium and specialty ones. In contrast, premium coffee types deliver 1.3–1.6× higher revenue per unit, confirming that volume leadership does not translate directly into revenue leadership.

* A small subset of products accounts for most of the revenue, with leading products contributing ~30–40% of category revenue in several markets. This indicates a moderate reliance on a narrow product mix, increasing exposure to demand or supply-side volatility.

* High-volume, low-revenue products represent the largest opportunity for margin expansion, as selectively shifting customers toward premium coffee or higher-value pack sizes could lift revenue per unit by 30–60% without requiring incremental volume growth.

* Country-level patterns show up to 50%+ volume concentration in a single coffee type in some markets, while others display more balanced product distribution across categories. This confirms that localized product, pricing, and marketing strategies can improve performance versus standardised global approaches.

Based on this analysis, I recommend the following actions:

* Reassess pricing strategy for high-volume Stock Keeping Units (SKU)
* Promote higher-margin products
* Introduce bundle offers or upsell strategies
* Localise product mix by country to reflect regional demand patterns

#### Question 2 Analysis Output
														
<img width="1469" height="934" alt="image" src="https://github.com/user-attachments/assets/8cf97800-44d4-4166-baee-858536f48970" />

Key Insights: 

* Customer value is highly concentrated: A small segment of high-value customers contributes a disproportionate share of total revenue, with ~25–45% higher average order values than other segments.

* Low purchase frequency dominates: Over 90% of customers purchase fewer than two times, indicating weak retention and limited repeat purchasing behaviour.

* High-value customers prefer premium products: Strong preference for larger pack sizes (2.5 kg) and dark roasts, especially Liberica, which generates the highest revenue per product-customer combination.

* Mid-value customers show upsell potential: Medium-value customers exhibit moderate order sizes, suggesting a clear opportunity to trade them up into higher-value baskets.

Based on this analysis, I recommend the following actions:

* Launch targeted retention campaigns for low-frequency customers (e.g., loyalty rewards, reorder reminders, personalised discounts).
* Develop premium bundles centred on dark roast and large pack sizes to appeal to high-value customers.
* Implement upsell strategies for medium-value customers, such as volume discounts or subscription plans.
* Personalise marketing and offers using customer segmentation based on order value and purchase frequency.
* Track customer migration between segments to measure the impact of retention and upselling initiatives.

#### Question 3 Analysis Output
																	
<img width="1469" height="641" alt="image" src="https://github.com/user-attachments/assets/3d9f3f89-a4a6-436f-8e36-de54b12486c2" />

Key Insights:

* Revenue is highly concentrated, with <10% of customers driving a disproportionate share of spend.

* Over 65% of customers spend less than $50, indicating the possibility for a significant upside in customer development.

* High-frequency customers show a clear preference for premium products, particularly Liberica and Excelsa.

* Increased engagement is strongly associated with higher average order values and premium product adoption.

Based on this analysis, I recommend the following actions:

* Introduce tiered loyalty rewards to incentive higher purchase frequency and spending thresholds.
* Deploy personalised product recommendations to encourage trade-up into premium coffee types.
* Design targeted campaigns for low- and mid-frequency customers to stimulate repeat purchases.
* Offer exclusive benefits and early access to new products for top-tier customers to protect retention.
* Track conversion rates between frequency tiers and average order value uplift as core loyalty Key Performance Indicators (KPI).

#### Question 4 Analysis Output
																	
<img width="1240" height="701" alt="image" src="https://github.com/user-attachments/assets/44bdefae-f750-49e1-a31d-6736c86cd9a3" />

Key Insights:

* Mid-range priced products drive the highest sales volume (~945 units), showing strong mass-market demand.

* Premium-priced products achieve higher unit margins (~$15/unit) but lower volumes (~850 units), indicating selective, value-driven demand.

* Large pack sizes (2.5 kg) dominate revenue contribution (~$24K, over 40% of total sales), confirming bulk purchasing as the primary revenue engine.

* High-price, high-volume products generate the highest total revenue (~$20K+), making them the most commercially impactful category.

Based on this analysis, I recommend the following actions:

* Prioritise high-price, high-volume Stock Keeping Units (SKU) through targeted promotions, preferred shelf placement, and availability optimisation.
* Expand bulk pack incentives (e.g., subscriptions, loyalty multipliers, bundle discounts) to reinforce repeat purchasing.
* Refine pricing strategy by product tier, protecting premium margins while using mid-tier products to drive scale.
* Leverage smaller packs as acquisition tools, focusing on sampling, onboarding, and upsell pathways into larger formats.

#### Question 5 Analysis Output
																	
<img width="1240" height="961" alt="image" src="https://github.com/user-attachments/assets/e8a4860c-7efb-4202-a8a8-71d12f0a497f" />

Key Insights:

* Sales are highly cyclical, peaking in second quarter and Spring/Summer and weakening in fourth quarter and Winter.

* The ~50% revenue collapse in 2022 represents a material business risk and likely reflects macroeconomic, pricing, or supply-chain disruption rather than product mix changes.

* Medium and light roasts drive warm-season growth, while dark roasts provide seasonal stability in colder months.

* Excelsa exhibits strong upside volatility, making it a high-impact lever for growth acceleration, while Liberica shows higher sales volatility, implying greater exposure to operational and supply risks.

Based on this analysis, I recommend the following actions:

* Implement seasonal demand forecasting models to align production, inventory, and logistics with second quarter and Spring/Summer peaks. 
* Deploy targeted fourth quarter recovery strategies, including pricing bundles, limited-edition winter blends, and loyalty promotions to stabilize off-peak revenue.
* Shift product mix dynamically by season, prioritizing lighter and medium roasts in warmer months and dark roasts in colder periods.
* Conduct root-cause analysis of the 2022 decline (pricing, supply constraints, channel performance, or macro impacts) and embed risk mitigation controls.






































