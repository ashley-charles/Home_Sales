# Home_Sales

Use of SparkSQL to determine key metrics about home sales data. Then you'll use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

![image](https://github.com/user-attachments/assets/3a9d0a0a-a4ff-4975-a4bc-15e942abc7ab)

# Findings

1. What is the average price for a four-bedroom house sold for each year? Round off your answer to two decimal places.

![image](https://github.com/user-attachments/assets/4c92fc84-3b95-42a0-8963-37f28650c727)

2. What is the average price of a home for each year it was built that has three bedrooms and three bathrooms? Round off your answer to two decimal places.

![image](https://github.com/user-attachments/assets/455fab75-8553-40a3-9c3c-e14c39c00ef3)

3. What is the average price of a home for each year that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off your answer to two decimal places.

![image](https://github.com/user-attachments/assets/45ed4db6-624e-4b3b-9e1d-99886f4d08d4)

4. What is the "view" rating for homes costing more than or equal to $350,000? Determine the run time for this query, and round off your answer to two decimal places.

![image](https://github.com/user-attachments/assets/622a1238-5678-4531-9fd1-87ad415e26b0)

5. Using the cached data, run the query that filters out the view ratings with an average price of greater than or equal to $350,000. Determine the runtime and compare it to uncached runtime. Partition by the "date_built" field on the formatted parquet home sales data.

- Cached data

![image](https://github.com/user-attachments/assets/909f4c03-2331-467a-9fd4-ab25f6025b8f)

- Parquet formatted data

![image](https://github.com/user-attachments/assets/e920c218-f831-4233-a21b-63779c41d414)

Both the cached data and the Parquet formatted data have faster runtimes compared to the original data .

In conclusion, Parquet formatted data demonstrates the best runtime among the three options (Run time for original data, cached data and parquet formatted data).


