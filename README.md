# sql-challenge

## Background

A research project was conducted on employees of a corporation from the 1980s and 1990s. All that remained of the database of employees from that period are six CSV files. The following tasks were carried out on the data set and explained in more detail below: **data modeling**, **data engineering**, and **data analysis**.


#### Data Modeling

* The data, in the form of CSVs, was inspected to determine appropriate column types.
* An ERD of the tables was constructed using [http://www.quickdatabasediagrams.com](http://www.quickdatabasediagrams.com).

#### Data Engineering

* A table schema was created for each of the six CSV files including appropriate data types, primary keys, foreign keys, and other constraints.

* Data from each CSV file was imported into the corresponding SQL table. 

#### Data Analysis

SQL queries were written to address each of the following:

1. List the following details of each employee: employee number, last name, first name, sex, and salary.

2. List first name, last name, and hire date for employees who were hired in 1986.

3. List the manager of each department with the following information: department number, department name, the manager's employee number, last name, first name.

4. List the department of each employee with the following information: employee number, last name, first name, and department name.

5. List first name, last name, and sex for employees whose first name is "Hercules" and last names begin with "B."

6. List all employees in the Sales department, including their employee number, last name, first name, and department name.

7. List all employees in the Sales and Development departments, including their employee number, last name, first name, and department name.

8. List the frequency count of employee last names (i.e., how many employees share each last name) in descending order.

#### Further Data Analysis with Python

As you examine the data, you begin to suspect that the dataset is fake. Maybe your boss gave you spurious data in order to test the data engineering skills of a new employee? To confirm your hunch, you decide to create a visualization of the data to present to your boss. Follow these steps: 

1. The SQL database was imported into Pandas. 

2. A histogram was created to visualize the most common salary ranges for employees.

3. A bar chart was created to display average salary by title.

## Analysis

* The employee salaries, as displayed in the histogram below, seem to make sense. More employees make less and fewer employees make more. This seems to decrease exponentially.
* The salaries start to seem suspicious when grouped with by title. When averaging each category, we found that they're all roughly the same. Typically, we would expect more variation here. For example, senior staff generally make more than staff, senior engineers generally make more than engineers, managers often make the most, etc.
* Out of over 300,000 employees, there are only 1,638 unique last names. Each name has around 150 - 200 occurrences except "Foolsday," which only has one occurrence. This further indicates that the employee data is fictitious. 

- - -

## References

* Assignment 9 instructions.
* [http://www.quickdatabasediagrams.com](http://www.quickdatabasediagrams.com)
