# Pewlett-Hackard-Analysis
Developing an employee database to analyze retiring employees and determine eligibility of a mentorship program with SQL.

## Overview of the Analysis
The purpose of this project was to assist Bobby, a human resource analyst, in a project that that was assigned to him by his manager that would *"future proof"* Pewlett Hackard.  The ultimate goals of this project included:
* Determine the number of retiring employees by title
* Determine the employees that are eligible for a Mentorship Program
* A final report that would help managers to prepare for the upcoming *"silver tsunami"*

### Resources

Data Source (initial):
  * departments.csv
  * dept_emp.csv
  * dept_manager.csv
  * employees.csv
  * salaries.csv
  * titles.csv

Code:
  * Employee_Database_challenge.sql

Software:
  * pgAdmin 6.1; Visual Studio Code 1.64.0

## Results
The two deliverables in this project included:
1. Determining the number of retiring employees by title
2. Determining employees that are eligible for the Mentorship Program

In order to visualize the relationship between the available data sources and the Pewlett Hackard employee structure, an Entity Relationship Diagram was developed:


![image](https://user-images.githubusercontent.com/94148420/152712774-7a0f8248-d1d2-4403-bb57-e48d807ca8ec.png)


### Determining the Number of Retiring Employees by Title
In order to determine the number of retiring employees by title (retiring_titles), two tables had to be created:
* retirement_titles
* unique_titles

Below is the code that created the **retirement_titles** table:

![image](https://user-images.githubusercontent.com/94148420/152713180-18a34adb-c779-455d-a44d-544adb6dc201.png)

The **unique_titles** table was created with this code:

![image](https://user-images.githubusercontent.com/94148420/152713248-4e79d8a3-0de1-44b6-8a3d-41deb73e73c0.png)

Which ultimately created the final table, **retiring_titles**:

![image](https://user-images.githubusercontent.com/94148420/152713410-72104ac0-08ee-4cce-8244-a48054c411c6.png)

This is the output of the **retiring_titles** table:

![image](https://user-images.githubusercontent.com/94148420/152713625-3b51ff10-304b-4f76-b05c-e5c90b8c0a41.png)

Significant findings in this table include:
1. There are a total of 7 titles included with those that will be retiring.
2. A total of 72,458 employees will be retiring.
3. The largest title group retiring is Senior Engineer with 25,916 employees, followed closely by Senior Staff with 24,926 employees
4. There are two Managers that will be retiring
5.  








## Summary
