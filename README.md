# Task_7
use SQl inside py
# Task 7: Sales Summary from SQLite Database

## Objective
- Connect Python to an SQLite database
- Run SQL queries inside Python
- Summarize sales data
- Visualize revenue by product

## Tools
- Python (sqlite3, pandas, matplotlib)
- SQLite (built-in)

## Steps
1. Created a database `sales_data.db` with a `sales` table.
2. Inserted sample sales records.
3. Queried total quantity and revenue per product using SQL:
   ```sql
   SELECT product, SUM(quantity) AS total_qty, SUM(quantity * price) AS revenue
   FROM sales
   GROUP BY product;
4.Imported results into pandas and displayed them.
```o/p
Sales Summary:
     product  total_qty    revenue
0  Keyboard         30    45000.0
1    Laptop         30  1524000.0
2   Monitor         36   438000.0
3     Mouse         60    30000.0

5.Created a simple bar chart using matplotlib.
      
