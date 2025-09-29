# plsql-window-function-iradukunda-nicole
## Project overview
Business Context: A retail company with branches in Rwanda, selling groceries and beverages.
Data Challenge: The sales manager struggles to identify which products perform best per region and to track customer purchase patterns over time.
Expected Outcome: Use SQL window functions to rank products, measure sales growth, and segment customers for targeted marketing.
#5 measurable goals using window functions:
Top 5 products per region/quarter → RANK()

Running monthly sales totals → SUM() OVER()

Month-over-month growth → LAG()/LEAD()

Customer quartiles → NTILE(4)

3-month moving averages → AVG() OVER()

#Database Schema

customers

customer_id (PK)

name

region
Example: (1001, John Doe, Kigali)

products

product_id (PK)

name

category
Example: (2001, Coffee Beans, Beverages)

transactions

transaction_id (PK)

customer_id (FK)

product_id (FK)

sale_date

amount
Example: (3001, 1001, 2001, 2024-01-15, 25000)

## How to run
1. Run sql/create_tables.sql in Oracle SQL Developer.
2. Run sql/insert_sample_data.sql to insert test data.
3. Run queries in the sql/queries_*.sql 

## Key queries & insights

...

## Results analysis
Top products in Kigali for Q1 were Roast Coffee 250g and Ground Coffee 500g, accounting for 48% of regional sales. Running totals show steady growth in Western region from March through June.”

Diagnostic (why?)
“Kigali’s top products align with higher footfall and a marketing campaign launched in early Q1. The Western region growth likely resulted from a new store opening in late February and local promotions.”

Prescriptive (what next?)
Increase inventory of the two top coffee SKUs in Kigali and run targeted promotions for mid-quartile customers to lift them into higher quartiles; reassign marketing budget from low-performing snacks to best-selling beverages in Q3.”

## References
[[List of references — at least 10]](https://docs.oracle.com/en/database/oracle/oracle-database/)

