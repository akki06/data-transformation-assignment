## Python Task: Data Cleaning & Transformation

### Objective:
Clean and transform messy sales data using reusable UDFs and create a derived column.

### Tasks Completed:
- Converted `order_id`, `product_id`, `quantity` to integers
- Converted `price_per_unit` to float
- Parsed `order_date` into datetime format using multiple formats
- Handled missing and malformed values
- Calculated `total_price = quantity * price_per_unit`
- Saved cleaned data to `cleaned_sales.csv`

### Tools Used:
- Python
- Pandas
