# CODETECH-Task-2-1
# : Prajapati Udit Mukesh
# Company: CODTECH IT SOLUTIONS
# Id: CT12EHC
# Domain: SQL
# Duration: DECEMBER 17th, 2024 to FEBRUARY 17th, 2025.
# Mentor: Muzammil Ahmed

# Overview
In this task, we created two related tables—employees and department—within a MySQL database and performed multiple types of joins (INNER JOIN, LEFT JOIN, RIGHT JOIN, and FULL JOIN) to combine the data meaningfully. The goal was to demonstrate how different join operations work in relational databases and ensure that the dept_id column is consistent between the two tables to avoid errors and get meaningful results.

# Key Activities
Database Creation: Created a new MySQL database called company to house the two tables.
Table Creation: Defined the structure of two tables:
employees: Contains information about employees, including emp_id, name, and dept_id.
department: Contains information about departments, including dept_id and dept_name.
Data Insertion: Inserted matching data into both tables, ensuring that the dept_id values in the employees table match those in the department table.
Performing Joins:
INNER JOIN: Combined matching rows from both tables, returning only rows where there is a matching dept_id in both tables.
LEFT JOIN: Returned all rows from the employees table, with matching rows from the department table. If there was no match, NULL values were returned for the department.
RIGHT JOIN: Returned all rows from the department table, with matching rows from the employees table. If there was no match, NULL values were returned for the employee.
FULL JOIN (Emulated): Combined the results of both LEFT JOIN and RIGHT JOIN using UNION to simulate a full outer join. This operation returns all rows from both tables, with NULLs for unmatched rows.

# Technology Used
MySQL: A relational database management system used for creating databases, tables, and performing SQL queries. It was used to store and manage the data and perform various types of joins.
SQL (Structured Query Language): Used to write queries for creating tables, inserting data, and performing join operations (INNER JOIN, LEFT JOIN, RIGHT JOIN, and FULL JOIN).

# Key Insights
Understanding Joins:
INNER JOIN returns only the rows where there is a match between the two tables, filtering out non-matching data.
LEFT JOIN returns all rows from the left table, ensuring that even non-matching rows from the left table are included, with NULL values for columns from the right table.
RIGHT JOIN is similar to the LEFT JOIN but ensures that all rows from the right table are included, with NULL values for non-matching rows from the left table.
FULL JOIN (Emulated with UNION) combines the results of both LEFT and RIGHT joins, ensuring that all data from both tables is returned, even if there’s no match.
Database Structure: Proper table structure and matching key columns (dept_id) across both tables are crucial for successful joins. Ensuring consistency between related data in multiple tables is necessary for meaningful results.
Practical Use of Joins: Understanding how different types of joins impact the returned dataset is essential for querying relational databases effectively. Depending on the need, different joins can be used to retrieve the desired data from multiple tables.
