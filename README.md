# Retail Product Portfolio & Sales Performance Analysis

## 1. About the Project
This project analyzes retail product portfolio and sales performance using a comprehensive transaction and product dataset processed in Google Colab / Jupyter Notebook.

## 2. Objective
* Understand category-wise and product-wise revenue drivers.
* Evaluate monthly sales trends and seasonal impacts.
* Analyze price tier distributions across the product catalog.
* Apply **ABC inventory segmentation** to identify key patterns and high-value contributors in retail data.

## 3. Tools & Technologies Used
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Environment:** Jupyter Notebook / Google Colab

## 4. Steps Performed
1. **Data Loading & Cleaning:** Loaded and verified dataset attributes, handling file encodings and standardizing column names for consistency.
2. **Feature Engineering:** Created derived features including `Unit_Price`, `YearMonth`, and `Price_Tier` (`<$50`, `$50–$250`, `>$250`).
3. **Data Aggregation:** Calculated total revenue, total quantity sold, and average order values (AOV) grouped by product categories and individual items.
4. **ABC Inventory Segmentation:** Performed cumulative revenue calculations to classify products into three segments:
   * **Class A:** Top revenue drivers
   * **Class B:** Moderate revenue contributors
   * **Class C:** Low-performing items
5. **Visual Analytics:** Built multi-panel charts using Seaborn and Matplotlib to illustrate category revenue, monthly sales trends, and price tier distributions.
6. **Insight Generation:** Extracted structured observations and performance summaries from the aggregated metrics.

## 5. Key Findings
* **Revenue Drivers & ABC Classification:** Product segmentation successfully isolated top-performing revenue drivers (Class A) from low-performing items (Class C), highlighting core inventory contributors.
* **Sales Trends & Seasonality:** Monthly trend analysis and holiday multipliers (observed during November and December) demonstrated distinct spikes in order quantities and revenue during peak holiday shopping seasons.

## 6. Conclusion
The analysis successfully uncovered critical sales patterns across different product categories and price tiers. By leveraging ABC segmentation and visual trend analysis, this project provides actionable insights for inventory management and revenue optimization.

## 7. Dataset Source
* **Sample Superstore Dataset** (or synthetic retail transaction dataset generated within the analytical workflow).