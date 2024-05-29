# Home Sales Challenge

## SparkSQL

In this challenge, SparkSQL is used to determine key metrics about home sales data. Then, Spark is used to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

## Files Included

Home_Sales.ipynb


## Steps
1. Import the necessary PySpark SQL functions.
   
2. Read the `home_sales_revised.csv` data into a Spark DataFrame.

<img width="879" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/b0724ace-575d-4dd1-97f3-e69b53e4c7d2">

3. Create a temporary table called `home_sales`.
   
4. Answer the assignment questions.
   
5. Cache the temporary table `home_sales`.

6. Check if the temporary table is cached.

7. Use the cached data to run the last query (Question # 4 below). **Determine the runtime and compare it to the uncached runtime.**

8. Partition by the `"date_built"` field on the formatted parquet home sales data.

9. Create a temporary table for the parquet data.

10. Run the last query (Question # 4 below). **Determine the runtime and compare it to the uncached runtime.**

11. Uncache the home_sales temporary table.

12. Verify that the home_sales temporary table is uncached using PySpark.



## Use SparkSQL to answer the following:

### 1. What is the average price for a four-bedroom house sold each year?

The average price for a four-bedroom house ranged from $296,050.24 to $307,908.86.

<img width="898" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/807146d9-b971-4187-b3d4-f530bfcd03c2">


-------------------------------------------------------------------------------------------------------------------


### 2. What is the average price of a home for each year the home was built that has three bedrooms and three bathrooms?

The average price of a home with three bedrooms and three bathrooms ranged from $288,770.30 to $295,962.27 for the years 2010 to 2017; the highest prices were for homes built in 2013, and the lowest were for homes built in 2015.

<img width="754" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/be496873-728d-4ff4-a553-39a7eb677885">

-------------------------------------------------------------------------------------------------------------------

### 3. What is the average price of a home for each year the home was built that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet?

The average price of a home with three bedrooms, three bathrooms, two floors, and greater than or equal to 2,000 square feet ranged from $276553.81 to $307539.97 from 2010 to 2017; the highest prices were for homes built in 2012, and the lowest was for homes built in 2011.

<img width="723" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/8b46f0d9-bc45-49db-9bad-64de9982ed86">

-------------------------------------------------------------------------------------------------------------------

### 4. What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

The average price of a home per "view" rating, with an average home price greater than or equal to $350,000, is as below, with a **run time of 0.9524 seconds**.

<img width="562" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/fe97522e-404e-4b40-a3aa-dfc4f7acb032">

-------------------------------------------------------------------------------------------------------------------

### Use the cached data to run the last query (Question # 4 above). Determine the runtime and compare it to the uncached runtime.

The cached data run time was **0.5333 seconds**, which is 0.4191 seconds less than the uncached runtime.

<img width="774" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/a0f9be6a-466b-4968-a9a0-013acc83e4ef">

-------------------------------------------------------------------------------------------------------------------

### Partition by the "date_built" field on the formatted parquet home sales data and create a temporary table for the parquet data. Run the last query (Question # 4 above). Determine the runtime and compare it to the uncached runtime.

The **partitioned query runtime was 0.9847 seconds**, which is greater than the uncached runtime. This indicates that partitioning did not improve the query performance in this case. 

<img width="778" alt="image" src="https://github.com/Colex317/home_sales/assets/148498483/d8108ba7-9fcf-4457-92b5-b9b37f6ca2fe">
