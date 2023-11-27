# Home_Sales

I renamed the `Home_Sales_starter_code.ipynb` file to `Home_Sales.ipynb`.

I imported all the necessary PySpark SQL functions for the assignment.

I read the `home_sales_revised.csv` data from the starter code into a Spark DataFrame.

I created a temporary table called `home_sales`.

Using SparkSQL, I answered the following questions:

1. I calculated the average price for a four-bedroom house sold each year, rounding off the answers to two decimal places.

2. I determined the average price of a home for each year it was built that has three bedrooms and three bathrooms, again rounding off to two decimal places.

3. I found the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet, with the results rounded to two decimal places.

4. I analyzed the "view" rating for homes costing more than or equal to $350,000 and determined the run time for this query, rounding off the results to two decimal places.

After that, I cached the `home_sales` temporary table and checked to ensure that it was indeed cached.

Using the cached data, I ran the query again to filter out the view ratings with an average price of greater than or equal to $350,000. I measured the runtime of this query and compared it to the runtime when the data was not cached.

I partitioned the data by the "date_built" field on the formatted parquet home sales data and created a temporary table for the parquet data.

I executed the query to filter out the view ratings with an average price of greater than or equal to $350,000 on the parquet data. I determined the runtime and compared it to the runtime when using the cached data.

I then uncached the `home_sales` temporary table and verified using PySpark that the table was no longer cached.

Finally, I downloaded the `Home_Sales.ipynb` file and uploaded it into my "Home_Sales" GitHub repository.
