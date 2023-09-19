# sql-challenge

### This repo contains the necessary artifacts to satisfy the requirements of this challenge.

| File | Description |
| - | - |
| `EmployeeSQL/data/*.*` | CSV data files distributed with the challenge exercise. |
| `EmployeeSQL/QuickDBD-export.png` | ERD image exported from the QuickDBD software. |
| `EmployeeSQL/QuickDBD-export.sql` | Table schema exported from the QuickDBD software and used to build the tables and constraints. |
| `EmployeeSQL/data_analysis.sql` | SQL statements for the eight data analysis challenge problems.  |
| `EmployeeSQL/data_load.sql` | SQL script used to load the data into the tables. |

### NOTES:
* Instead of using pgAdmin to import the data, I wrote a script (`EmployeeSQL/data_load.sql`) to perform that task.  I figured out how to accomplish this by reading the PostgreSQL documentation (https://www.postgresql.org/docs/16/sql-copy.html)
* We did not cover date comparisons in class, but I was able to find how to get the year using the PostgreSQL docmentation (https://www.postgresql.org/docs/current/functions-datetime.html#FUNCTIONS-DATETIME-EXTRACT)
* When determing the size for the text field names (departments.dept_name, employees.first_name, employees.last_name, and titles.title), I opened the .csv in Excel, obtained the length of the value, and then found the max length.  In a real-world scenario, I would have accounted for expansion and made those fields larger, instead of making them just big enough to fit all the starter data.
