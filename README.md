# sql-challenge
Module 9 Challenge for UM Bootcamp

# Background
It's been two weeks since you were hired as a new data engineer at Pewlett Hackard (a fictional company).  Your first major task is to do a research project about people whom the company employed during the 1980s and 1990s.  All that remains of the employee database from that time period are six CSV files.

For this project, you'll design the tables to hold the data from the CSV files, import the CSV files into a SQL database, and then answer questions about the data.  That is, you'll perform data modeling, data engineering and data analysis respectively.

# Overview
I used PgAdmin 4, and PostgreSQL 14 to create the tables from the CSV files and the overall database needed for this project.  I also used Visual Studio Code for organizing and analyzing the data. I used Quick DBD as well.

There were three parts to this week's challenge: data modeling, data engineering and data analysis.

## Data Modeling
I created the Entity Relationship Diagram (ERD) using the QuickDBD (Quick Database Diagrams) Tool to map out the tables that were included in the six CSV files: employees, departments, dept_emp, dpt_manager, salaries and titles.  The map included the table titles, fields and relationships between them.

## Data Engineering
I used PgAdmin 4 and PostgreSQL to create a table schematic for each of the six files (listed above) that included the data types, primary keys and foreign keys for the relationships of these tables within the database.

After the table schematic was created, I imported the CSV files into the tables to run the Data Analysis on the information.

## Data Analysis
1. List the employee number, last name, first name, sex, and salary of each employee.  This was done by joining the employees and salaries tables to display the needed information.

2. List the first name, last name, and hire date for the employees who were hired in 1986.  This was done with a query on the employees table for hire dates between 1/1/1986 and 12/31/1986.

3. List the manager of each department along with their department number, department name, employee number, last name and first name. This was done joining departments, dept_manager and employees tables to display the needed information.

4. List the department number for each employee along with that employee's employee number, last name, first name, and department name.  This query joined employees, dept_emp, and department tables to find the needed information.

5. List first name, last name, and sex of each employee whose first name is Hercules and whose last name begins with the letter B.  This was done with a query on the employees table for first name being Hercules and last name starting with B.  There are a total of 20 employees fitting this criteria.

6. List each employee in the Sales department, including their employee number, last name and first name.  This was done by joining departments, dept_emp, and employees tables finding the sales department employees.

7. List each employee in the Sales and Development departments, including their employee number, last name, first name, and department name.  Similarly to the one before, but including an OR statement to also find the Development department.

8. List the frequency counts, in descending order, of all the employee last names.  For this one, the last name frequencies were counted and grouped by last name in descending order with Baba having 226 employees with this last name.

# Credits
Thank you to tutor, Marc Calache, who helped with an issue I had figuring out the frequency counts and a couple of other formatting issues.

Thank you to Hunter Hollis, instructor, and TA's: Randy and Sam for all of their teaching and support during this week's lessons of the Bootcamp.