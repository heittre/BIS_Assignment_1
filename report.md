## Dataset
- `data/supersalesdata.csv`  Superstore sales dataset (orders, sales, profit, quantity, discount, region, category, etc.).

## Processing steps
- Loaded `data/supersalesdata.csv` and parsed `Order Date` as datetime.
- Dropped duplicates, extracted `Year` and `Month`, and cleaned obvious parse issues.

## Key analyses performed
- Dataset overview and summary statistics (`df.describe()`).
- Sales aggregated by `Region` and plotted (`images/sales_by_region.png`).
- Sales aggregated by `Category` and plotted (`images/sales_by_category.png`).
- Sales distribution histogram (`images/sales_distribution.png`).
- Top 10 Sub-Categories by sales ranking (`images/top_subcategories_sales.png`).
- Monthly sales trend time series (`images/monthly_sales_trend.png`).

## Key findings

### Regional Performance
- **West Region** leads in total sales with approximately **$725,458**, representing the strongest market performance.
- **East Region** follows closely with **$677,451** in sales, indicating solid market penetration.
- **Central Region** generates **$501,240** in sales, showing moderate performance.
- **South Region** has the lowest sales at **$391,722**, suggesting growth opportunities or market challenges.

### Category Performance
- **Technology** dominates with **$836,154** in total sales, indicating strong demand for tech products.
- **Furniture** category generates **$742,000** in sales, performing well but slightly behind Technology.
- **Office Supplies** contributes **$718,047** in sales, maintaining steady performance across all regions.
- Technology consistently outperforms other categories across all regions.

### Sales Distribution
- Sales follow a right-skewed distribution, with most transactions being smaller orders.
- The distribution reveals a wide range of order values, indicating diverse customer purchase behaviors.
- Majority of sales fall below the median, with a long tail of high-value orders.

### Top Performing Sub-Categories
- Specific sub-categories within each category show varied performance levels.
- Focus areas for inventory management and marketing can be identified through sub-category rankings.
- Top-performing sub-categories drive disproportionate revenue compared to their count.

### Seasonal Trends
- Monthly sales data reveals clear seasonal patterns throughout the year.
- Peak sales periods can be identified for better inventory planning and promotional timing.
- Understanding seasonal fluctuations aids in cash flow forecasting and resource allocation.

## Saved outputs (`images/`)
- `sales_by_region.png` - Bar chart showing total sales by the four regions
- `sales_by_category.png` - Bar chart showing total sales by Technology, Furniture, and Office Supplies
- `sales_distribution.png` - Histogram displaying the distribution of individual transaction sales
- `top_subcategories_sales.png` - Horizontal bar chart of the top 10 performing sub-categories
- `monthly_sales_trend.png` - Line chart displaying monthly sales trends over time

## How to regenerate
1. Open the notebook `notebooks/superstoresalesdataAnalysis.ipynb`.
2. Run all cells (this will save plots under `images/`).

---
