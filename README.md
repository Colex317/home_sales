# Home Sales Challenge

## SparkSQL

In this challenge, we use SparkSQL to determine key metrics about home sales data. Then used Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## Files Included

Home_Sales.ipynb.ipynb


## Steps
1. Import the necessary PySpark SQL functions.
   
2. Read the `home_sales_revised.csv` data into a Spark DataFrame.

<img width="752" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/f54b1c17-d7ca-4eb0-b65a-9fb9356a8b18">

3. Create a temporary table called `home_sales`.
   
4. Answer the assignment questions.
   
5. Cache the temporary table `home_sales`.

6. Check if the temporary table is cached.

7. Use the cached data to run the last query (which calculates the average price of a home per "view" rating with an average home price greater than or equal to $350,000). Determine the runtime and compare it to the uncached runtime.

8. Partition by the `"date_built"` field on the formatted parquet home sales data.

9. Create a temporary table for the parquet data.

10. Run the last query (which calculates the average price of a home per "view" rating with an average home price greater than or equal to $350,000). Determine the runtime and compare it to the uncached runtime.

11. Uncache the home_sales temporary table.

12. Verify that the home_sales temporary table is uncached using PySpark.

13. Download the `Home_Sales.ipynb` file and upload it to the GitHub repository.


## Using SparkSQL to answer the following:

- What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

- What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

- What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

- What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.


