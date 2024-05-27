# Home Sales Challenge

## SparkSQL

In this challenge, we use SparkSQL to determine key metrics about home sales data. Then used Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## Files Included

Home_Sales.ipynb.ipynb


## Steps
1. Import the necessary PySpark SQL functions.
   
2. Read the `home_sales_revised.csv` data into a Spark DataFrame.

<img width="879" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/b0724ace-575d-4dd1-97f3-e69b53e4c7d2">


3. Create a temporary table called `home_sales`.
   
4. Answer the assignment questions.
   
5. Cache the temporary table `home_sales`.

6. Check if the temporary table is cached.

7. Use the cached data to run the last query (which calculates the average price of a home per "view" rating with an average home price greater than or equal to $350,000).
   **Determine the runtime and compare it to the uncached runtime.**

8. Partition by the `"date_built"` field on the formatted parquet home sales data.

9. Create a temporary table for the parquet data.

10. Run the last query (which calculates the average price of a home per "view" rating with an average home price greater than or equal to $350,000).
    **Determine the runtime and compare it to the uncached runtime.**

11. Uncache the home_sales temporary table.

12. Verify that the home_sales temporary table is uncached using PySpark.



## Use SparkSQL to answer the following:

- What is the average price for a four-bedroom house sold each year?
  
-------------------------------------------------------------------------------------------------------------------


- What is the average price of a home for each year the home was built that has three bedrooms and three bathrooms?

  The average price of a home with three bedrooms and three bathrooms from 2010 to 2017 ranged from $288,770.30 to $295,962.27; the highest prices were for homes built in 2013, and the lowest were for homes built in 2015.

<img width="754" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/be496873-728d-4ff4-a553-39a7eb677885">


-------------------------------------------------------------------------------------------------------------------

- What is the average price of a home for each year the home was built that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

<img width="502" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/d8b246f6-4698-468d-9954-0ac2ae3c39d1">

-------------------------------------------------------------------------------------------------------------------

- What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

<img width="562" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/fe97522e-404e-4b40-a3aa-dfc4f7acb032">

