# &#x20;                              **SALES REPORT**



**1. Problem Statement \& Scope**



&#x20;performance varies substantially across product categories, pricing tiers, and seasonal periods. This project evaluates a transactional retail dataset to compare sales across product lines, isolate high-performing revenue drivers from low-performing inventory, and analyze longitudinal time-based trends.



**2. Pre-Analysis Product Attribute Specification**



Before executing exploratory or statistical aggregations, the following product attributes and sales metrics were specified and programmatically verified within the dataset:

|**Attribute / Metric**|**Field Name**|**Classification**|**Analytical Role**|
|-|-|-|-|
|**Product Category**|Category|Product Attribute|Macro-level grouping (Electronics, Furniture, Office Supplies, Apparel).|
|**Product Identifier**|**Product\_Name**|product Attribute|Granular SKU/item identifier for ranking individual winners and laggards.|
|**Unit Price \& Tier**|Unit\_Price / Price\_Tier|product Attribute|Binned into Budget (less than $50), Mid-Range ($50–$250), and Premium (greater than $250).|
|**Transaction Date**|Order\_Date|Temporal Attribute|Aggregated to monthly periods (YearMonth) to detect seasonal demand spikes.|
|**Quantity Sold**|Quantity|Sales Measure|Measures unit movement velocity across categories.|
|**Total Revenue**|Revenue|Sales Measure|Primary financial metric (Unit Price X Quantity).|



**3. Analytical MethodologyData Verification \& Cleaning:** 



Programmatic assertion checks confirmed zero missing schema fields.



Dates were standardized to datetime objects, and continuous pricing was discretized into price tiers.Category \& Price-Tier Aggregation: 

Grouped transactions by Category and Price\_Tier to compare total revenue against unit volume and Average Order Value (AOV).



**ABC (Pareto) Inventory Classification:** 



**Ranked all products by cumulative revenue contribution:**



Class A (Top 80% Revenue): Core high-priority SKUs requiring strict stock-out prevention.



Class B (Next 15% Revenue): Moderate performers suited for targeted bundling.



Class C (Bottom 5% Revenue): Low-velocity items requiring clearance or assortment pruning.



Time-Series Trend Evaluation: Aggregated monthly sales across a 24-month window to evaluate seasonality and Q4 holiday demand surges.



**4. Key Findings \& Recommendations**



Revenue Concentration: High-ticket Electronics and Furniture items dominate total revenue despite lower unit volumes compared to Office Supplies, which drives high transaction frequency but low Average Order Value.



Seasonality: Monthly time-series analysis reveals a pronounced Q4 surge (November–December) across all categories, requiring inventory buffer expansion in early Q4.



Actionable Strategy: Protect inventory levels for Class A items (Gaming Laptops, Smartphones, Standing Desks), bundle Class B accessories (Wireless Earbuds, USB-C Hubs) with Class A purchases to raise AOV, and apply promotional discounting to liquidate slow-moving Class C items.

