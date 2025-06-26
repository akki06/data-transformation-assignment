## SQL Task: Product Catalog Comparison

### Objective:
Compare two snapshots of a product catalog (`products_day1.csv` and `products_day2.csv`) to:
- Identify full rows that are added or removed.
- Detect column-level changes in matching product IDs.

### Tools:
- Python
- Pandas
- DuckDB (in-memory SQL engine)

### Output Files:
- `changes_full.csv`: Full rows that were added/removed with `change_type`
- `changes_column.csv`: Column-level changes with `old_value` and `new_value`

### Approach:
- Registered CSVs as SQL tables in DuckDB
- Used `EXCEPT` for full row comparison
- Used JOIN and WHERE clause to compare columns for matching `product_id`
- Avoided hardcoding for column comparison
