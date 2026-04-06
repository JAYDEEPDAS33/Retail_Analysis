# Retail Analysis Report

## Overview
This report summarizes the key findings from the retail transaction analysis conducted on the retail_transactions dataset stored in PostgreSQL.

## Data Source
- Database: PostgreSQL (localhost)
- Table: retail_transactions
- Connection: User 'postgres'

## Key Metrics
- **Average Order Value**: Calculated from total revenue per invoice
- **Total Revenue**: Aggregated across all transactions
- **Customer Base**: Unique customers by country

## Revenue Analysis

### Revenue by Country
- Top countries by total revenue were analyzed
- Visualization: Bar chart showing top 10 countries

### Revenue Distribution
- Log-transformed revenue distribution to handle skewness
- Filtered distribution for revenues under $5000
- Histograms showing the spread of transaction values

### Average Revenue per Country
- Countries ranked by mean transaction value
- Top performers identified for high-value markets

## Product Analysis

### Top Selling Products
- Products ranked by total quantity sold
- Horizontal bar chart visualization
- Top products by revenue contribution
- **Revenue visualization**: Bar chart showing top 10 products by total revenue value

### Product Pricing
- Average price per unit for top products
- Products with highest average prices identified

### Product Popularity
- Products ranked by number of unique orders
- Frequency of product appearance in transactions

## Customer Analysis

### Top Customers
- Customers ranked by total revenue contribution
- Bar chart showing top 10 customers by spending
- **Geographic distribution**: Top customers by country breakdown

#### Top 10 Customers by Revenue:
1. **Customer 14646.0** (Netherlands) - $280,206.02
2. **Customer 18102.0** (United Kingdom) - $259,657.30
3. **Customer 17450.0** (United Kingdom) - $194,550.79
4. **Customer 16446.0** (United Kingdom) - $168,472.50
5. **Customer 14911.0** (EIRE) - $143,825.06
6. **Customer 12415.0** (Australia) - $124,914.53
7. **Customer 14156.0** (EIRE) - $117,379.63
8. **Customer 17511.0** (United Kingdom) - $91,062.38
9. **Customer 16029.0** (United Kingdom) - $81,024.84
10. **Customer 12346.0** (United Kingdom) - $77,183.60

**Country Distribution of Top 10 Customers:**
- United Kingdom: 6 customers
- EIRE: 2 customers  
- Netherlands: 1 customer
- Australia: 1 customer

#### Top Customer Purchasing Patterns:
- **Customer 14646.0** (Netherlands): Lighting products, snack boxes, lunch boxes
- **Customer 16446.0** (UK): Bulk buyer of PAPER CRAFT, LITTLE BIRDIE (80,995 units)
- **Customer 12346.0** (UK): Bulk buyer of MEDIUM CERAMIC TOP STORAGE JAR (74,215 units)
- **Customer 18102.0** (UK): Office/kitchen items (memo boards, blackboards, card holders)
- **Customer 17450.0** (UK): Home decor (wicker items, T-light holders, pantry tins)
- **Customers from EIRE**: Focus on cake stands and baking accessories
- **Customer 17511.0** (UK): Party supplies (bunting, bags)
- **Customer 16029.0** (UK): Craft items and dolls

## Order Analysis

### Order Size Distribution
- Histogram of items per order
- Distribution of order quantities

### Temporal Analysis

#### Monthly Revenue Trend
- Revenue plotted over time by month
- Seasonal patterns and growth trends

#### Revenue by Day of Week
- Weekly patterns in sales
- Peak and low days identified

#### Revenue by Hour
- Hourly sales distribution
- Peak sales hours throughout the day

## Key Findings

### Top Performers
- **Country with Most Revenue**: United Kingdom generated the highest revenue of **$7,308,391.55**
- **Month with Maximum Revenue**: November 2011 had the highest monthly revenue of **$1,161,817.38**
- **Product with Most Sales (by Quantity)**: "PAPER CRAFT, LITTLE BIRDIE" sold **80,995 units**
- **Product with Highest Revenue**: "PAPER CRAFT, LITTLE BIRDIE" generated **$168,469.60** in total revenue
- **Top Customer**: Customer ID **14646.0** from **Netherlands** with **$280,206.02** in total spending

### Business Metrics
- **Average Order Value**: **$480.76** across all transactions
- **Day with Highest Revenue**: Thursday generated **$1,976,859.07** in revenue
- **Peak Sales Hour**: 12 PM (noon) showed maximum hourly revenue of **$1,378,571.48**
- **Country with Highest Average Transaction**: Netherlands with **$120.80** per transaction
- **Largest Customer Base**: United Kingdom with **3,921 unique customers**

### Business Insights
- The United Kingdom dominates both revenue and customer base, representing the primary market
- November shows peak seasonal performance, suggesting strong holiday sales
- Paper craft items show exceptional popularity, indicating demand for creative/hobby products
- Thursdays are the busiest sales days, possibly due to mid-week shopping patterns
- Peak sales occur around noon, suggesting optimal staffing and marketing timing
- Netherlands customers spend significantly more per transaction despite smaller market size

## Country-Specific Product Analysis

### Top Revenue Products by Country (Top 10 Countries):
- **United Kingdom**: PAPER CRAFT, LITTLE BIRDIE - $168,469.60 (represents significant portion of UK revenue)
- **Netherlands**: WHITE HANGING HEART T-LIGHT HOLDER - High-value home decor items
- **EIRE**: REGENCY CAKESTAND 3 TIER - Premium baking equipment
- **Germany**: ROUND SNACK BOXES SET OF4 WOODLAND - Kitchen storage solutions
- **France**: RABBIT NIGHT LIGHT - Popular lighting products
- **Australia**: 60 CAKE CASES VINTAGE CHRISTMAS - Seasonal baking supplies
- **Switzerland**: PICNIC BASKET WICKER 60 PIECES - Premium outdoor/entertainment items
- **Spain**: 3 TIER CAKE TIN RED AND CREAM - Baking accessories
- **Belgium**: Manual - Administrative/transaction items
- **Norway**: 12 PENCILS SMALL TUBE RED RETROSPOT - Art supplies

**Key Insights:**
- Different countries show distinct product preferences based on cultural and regional needs
- UK market dominated by craft/hobby items
- European markets show strong preference for home decor and kitchen items
- Baking and party supplies popular across multiple countries
- Visualization available showing top products for top 5 countries by revenue

## Customer Reorder Analysis

### Top Customers by Order Frequency (Most Reorders):
1. **Customer 12748.0** (United Kingdom) - **210 orders**, $33,719.73 total revenue
2. **Customer 14911.0** (EIRE) - **201 orders**, $143,825.06 total revenue
3. **Customer 17841.0** (United Kingdom) - **124 orders**, $40,991.57 total revenue
4. **Customer 13089.0** (United Kingdom) - **97 orders**, $58,825.83 total revenue
5. **Customer 14606.0** (United Kingdom) - **93 orders**, $12,156.65 total revenue
6. **Customer 15311.0** (United Kingdom) - **91 orders**, $60,767.90 total revenue
7. **Customer 12971.0** (United Kingdom) - **86 orders**, $11,189.91 total revenue
8. **Customer 14646.0** (Netherlands) - **74 orders**, $280,206.02 total revenue
9. **Customer 16029.0** (United Kingdom) - **63 orders**, $81,024.84 total revenue
10. **Customer 13408.0** (United Kingdom) - **62 orders**, $28,117.04 total revenue

### Customer Segmentation by Reorder Behavior:

#### High-Frequency, Lower-Value Customers:
- **Customer 12748.0**: 210 orders, $160.57 average order value
- **Customer 14606.0**: 93 orders, $130.72 average order value
- **Customer 12971.0**: 86 orders, $130.11 average order value

#### High-Frequency, High-Value Customers:
- **Customer 14911.0**: 201 orders, $715.55 average order value
- **Customer 14646.0**: 74 orders, $3,785.22 average order value
- **Customer 13089.0**: 97 orders, $606.45 average order value

**Key Insights:**
- **Customer 12748.0** is the most loyal customer with 210 orders (exceptional reorder frequency)
- **Different customer segments**: High-frequency/low-value vs. high-frequency/high-value buyers
- **UK dominance**: 8 out of 10 top reorder customers are from the United Kingdom
- **Loyalty patterns**: Some customers reorder frequently but with smaller order values, others combine frequency with high spending
- **Retention opportunities**: High-frequency customers represent valuable long-term relationships
- Visualization available showing order frequency vs. total revenue for top reorder customers

## Conclusions
- Key insights from the analysis
- Recommendations based on findings
- Areas for further investigation

## Visualizations
The analysis includes several charts and plots:
- Revenue distribution histograms
- Country-wise revenue bar charts
- Product sales visualizations
- Customer revenue charts
- Order size distributions
- Temporal trend plots
