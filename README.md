# Water Services SQL Analysis

## About the project

This project uses **SQL** to explore water services data from the `md_water_services` database.

I worked with information about employees, locations, water sources, visits, and waiting times. The aim was to practise SQL and learn how to find useful information from a database.

## What I did

- **Employee data:** Checked employee records, created email addresses, cleaned phone numbers, and counted employees in each town.
- **Visits:** Looked at visits and compared the visit totals for employees.
- **Locations:** Counted records by town, province, and rural or urban location.
- **Water sources:** Counted different types of water sources and looked at how many people they serve.
- **Waiting times:** Calculated average queue times and compared them by day and hour.
- **Global water access:** Looked at rural water access values from different countries.

## Some results

These results come from the saved notebook output:

- About **59.87%** of the location records are marked as rural.
- **Shared taps** serve the highest total number of people among the water source types in the dataset: **11,945,272**.
- The average queue time for records with a waiting time above zero is about **123.26** (in the dataset's `time_in_queue` units).
- **Saturday** has the highest average queue time in the weekday results (**246**), while **Sunday** has the lowest (**82**).
- The first and last visit records are dated **1 January 2021** and **14 July 2023**.

## Tools used

- MySQL
- SQL
- Python and Jupyter Notebook
- `ipython-sql` and `PyMySQL` to run MySQL queries in Jupyter

## Files

- **`ALX_SQL_Project_2.ipynb`** — The SQL notebook. It has a short, simple explanation above each query.

## How to run the notebook

1. Install MySQL and make sure the `md_water_services` database is available on your computer. You will need the tables `employee`, `visits`, `location`, `water_source`, and `global_water_access`.
2. Install Python and Jupyter Notebook. Install the SQL packages by running:

   ```bash
   pip install notebook ipython-sql pymysql
   ```

3. Open the notebook:

   ```bash
   jupyter notebook
   ```

4. In the database connection cell, replace `YOUR_PASSWORD` with your own MySQL password. If your database uses a different name or username, update those as well.
5. Run the notebook cells from top to bottom.

**Note:** The MySQL database itself is not included. You need the data to run the queries. Some queries use `UPDATE` and change employee records, so use a backup if needed. The saved results may need to be refreshed by running the cells again.

## What I learned

Through this project, I practised SQL commands such as `SELECT`, `WHERE`, `GROUP BY`, `ORDER BY`, `LIMIT`, `UPDATE`, `COUNT`, `SUM`, `AVG`, and `RANK`. I also worked with SQL functions to clean text and analyse dates and waiting times.
