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

Which ultimately helped to create the final table, **retiring_titles**:

![image](https://user-images.githubusercontent.com/94148420/152713410-72104ac0-08ee-4cce-8244-a48054c411c6.png)

This is the output of the **retiring_titles** table:

![image](https://user-images.githubusercontent.com/94148420/152713625-3b51ff10-304b-4f76-b05c-e5c90b8c0a41.png)

Significant findings in this table include:
1. There are a total of 7 titles included with those that will be retiring.
2. A total of 72,458 employees will be retiring.
3. The largest title group retiring is Senior Engineer with 25,916 employees, followed closely by Senior Staff with 24,926 employees
4. There are two Managers that will be retiring

### Determining Employees that are Eligible for the Mentorship Program
Below is the code that created the **mentorship_eligibility** table:

![image](https://user-images.githubusercontent.com/94148420/152723349-13a31c01-2d51-4250-a90d-e920964ee753.png)

To be eligible for the Mentorship Program, the employee had to have been born in 1965.  There are a **total of 1549 employees** that are eligible for the program.  Here is an image of last seven who are eligible:

![image](https://user-images.githubusercontent.com/94148420/152715598-7da62c1d-6154-4dd1-8388-33308462bafe.png)



## Summary
The Human Resources Department and the Leadership Team at Hewlett Packard will have work to do in order to minimize the impact of the impending "silver tsunami."
* An analysis of retiring employees by title demonstrated that there is a total of **72,458** employees eligible for retirement, and thus roles to be filled.  These are employees with a birth date between January 1, 1952 and December 31, 1955.  Here is an image of the last seven employees in this list:

![image](https://user-images.githubusercontent.com/94148420/152720742-45e05bb5-3949-4ed0-9afe-cf24d5c19860.png)

* There are a total of 1549 employees eligible for the Mentorship program.  These are employees that were born in 1965.  Here is a sample of the employees that would be eligible for the Mentorship Program:

![image](https://user-images.githubusercontent.com/94148420/152721016-89945dc8-5a8a-42e4-a7da-6cb212d9f3e7.png)

* A Mentorship Program can be successful by identifying Senior Engineers (25,916), Senior Staff (24926), and Managers (2) who have an interest in becoming a Mentor before they retire.  **There are enough retirement ready employees to become Mentors.**
* The Human Resources Department will take the lead, with the assistance of the Leadership Team to:
     * Define and establish the Mentorship Program
     * Identify and train potential Mentors
     * Promote the Mentorship Program to the 1549 eligible candidates
     * Enroll eligible candidates into the program
     * Candidates to complete and graduate from the program
     * Assess the results of the initial Mentorship Program class and make changes as necessary


