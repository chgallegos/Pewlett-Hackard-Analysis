# PEWLETT-HACKARD-ANALYSIS
----
## Overview

The purpose of this analysis was to apply SQL database language in order to extract, merge and export information requested by PH's Human Resources department. The directions are intended for the company to have a proactive approach to the upcoming stream of employees reaching a retirement date. The analysis was divided into two parts, the first one is focused on exctracting the number of retiring employess by title, and secondly, the employees that will be eligible to become mentors after they retire.

----
## Results
### PART 1 "Employees Retiring by Title"

-The importance for every department to understand the need for this proactive approach is to be considered fundamental. With this information, different departments will have an idea of their future staffing needs as well as incentivize internal advancement in order to fulfill upcoming needs.

-The Retirement Titles table was created from joining data from the "employees" table and the "titles" table. This was also narrowed to only provide employees within a certain range of birthdays.

![Screenshot](https://github.com/chgallegos/Pewlett-Hackard-Analysis/blob/main/Analysis%20Projects%20Folder/Pewlet-Hackard-Analysis%20Folder/resources/retirement_titles.png)

-After the retirement titles was extracted, another query and table was created in order to narrow down employees that were currently employed.

![Screenshot](https://github.com/chgallegos/Pewlett-Hackard-Analysis/blob/main/Analysis%20Projects%20Folder/Pewlet-Hackard-Analysis%20Folder/resources/unique_titles.png)

-Lastly, a count was done for every employee currently employed and close to retirement. This was summarized in a way that the count was grouped by department as to provide a macro piece of data to each department head.

### PART 2 "Employees Eligible for the Mentorship Program"

-In order to maintain employee engagement and to provide exceptional training for current employees, the company has decided to create a "Mentorship Program" for post-retirement employees.

-The database analysis for this part of the process was similar to the retrieval of retirement titles, however it joined with two more tables: "Department Employees" and "Titles". Finally the filter extracted only employees with birthdays during 1965 as this establishes a level of seniority that can be considered effective for the program

![Screenshot](https://github.com/chgallegos/Pewlett-Hackard-Analysis/blob/main/Analysis%20Projects%20Folder/Pewlet-Hackard-Analysis%20Folder/resources/mentorship_eligibility.png)

----
## Summary 

How many roles will need to be filled as the "silver tsunami" begins to make an impact?

In order to answer this question, a table was created based on a refactored query, I added the count that the retiring titles table provided into another table, providing a result of 72,458 employees

![Screenshot](https://github.com/chgallegos/Pewlett-Hackard-Analysis/blob/main/Analysis%20Projects%20Folder/Pewlet-Hackard-Analysis%20Folder/resources/total_employees_retiring.png)
![Screenshot](https://github.com/chgallegos/Pewlett-Hackard-Analysis/blob/main/Analysis%20Projects%20Folder/Pewlet-Hackard-Analysis%20Folder/resources/total_employees_retiring_2.png)

Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

The total of employees eligible to mentor is 1,549. if the same amount of employees retiring will be coming in, I think that the program could be beneficial as it provides options for retired employees to pass on their skill and talents. I do believe that it is likely that not all eligible employees will take the opportunity to mentor, although it is most likely also that not all employees take advantage of having a mentor.

![Screenshot](https://github.com/chgallegos/Pewlett-Hackard-Analysis/blob/main/Analysis%20Projects%20Folder/Pewlet-Hackard-Analysis%20Folder/resources/total_employees_mentoring.png)
![Screenshot](https://github.com/chgallegos/Pewlett-Hackard-Analysis/blob/main/Analysis%20Projects%20Folder/Pewlet-Hackard-Analysis%20Folder/resources/total_employees_mentoring_2.png)