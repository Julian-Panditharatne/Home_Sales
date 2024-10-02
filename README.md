# Home Sales Challenge

- The purpose of this analysis is to use SparkSQL to determine key metrics about home sales data, and then use Spark to create temporary views, partition the data, cache and uncache a temporary table, and verify that the table has been uncached.

- The analysis was performed in the following manner:
  - Read the `home_sales_revised.csv` data in the starter code into a Spark DataFrame.
  - Created a temporary table called **home_sales**.
  - Answered the following questions using SparkSQL:
    - What is the average price for a four-bedroom house sold for each year? Round off the answer to two decimal places.
    - What is the average price of a home for each year the home was built, that has three bedrooms and three bathrooms? Round off the answer to two decimal places.
    - What is the average price of a home for each year the home was built, that has three bedrooms, three bathrooms, two floors, and is greater than or equal to 2,000 square feet? Round off the answer to two decimal places.
    - What is the average price of a home per "view" rating having an average home price greater than or equal to $350,000? Determine the run time for this query, and round off the answer to two decimal places.
  - Cached the temporary table **home_sales**.
  - Checked if the temporary table is cached.
  - Using the cached data, ran the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determined the runtime and compared it to uncached runtime.
  - Partitioned by the "date_built" field on the formatted parquet home sales data.
  - Created a temporary table for the parquet data.
  - Ran the last query that calculates the average price of a home per "view" rating having an average home price greater than or equal to $350,000. Determined the runtime and compared it to uncached runtime.
  - Uncached the **home_sales** temporary table.
  - Verified that the **home_sales** temporary table is uncached using PySpark.

---

## Repository Files and Folders

Besides this `README.md` file there are three other files in this repository:

- `Home_Sales_colab.ipynb`: A Jupyter Notebook containing the code used to perform the analysis with Google Colab.

- `Home_Sales_starter_code.ipynb`: A Jupyter Notebook containing the starter code for performing the analysis without Google Colab.

- `Home_Sales_starter_code_colab.ipynb`: A Jupyter Notebook containing the starter code for performing the analysis with Google Colab.
