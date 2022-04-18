# Pewlett-Hackard-Analysis


## Purpose:

### Determining the number of retiring employees per title eligible for retirement.
### Identifying employees who are eligible to participate in a mentorship program.
### We are preparing Bobby’s manager for the “silver tsunami” as many current employees reach retirement age.


## Deliverable 1

### Using the Pewlett-Hackard Employee Database:

### Created a Retirement Titles table that holds all the titles of employees who were born between January 1, 1952 and December 31, 1955. (Retirement eligible age group)

### Determined the number of retiring employees per title.

Used the DISTINCT ON statement in Postgres Query to create a table that contains the most recent title of each employee.
 
Then, used the COUNT() function to create a table that has the number of retirement-age employees by most recent job title. 

Finally, because we wanted to include only current employees in our analysis, we excluded those employees who have already left the company.

Number of Retirement eligible employees by title:


 <img width="359" alt="Screen Shot 2022-04-17 at 9 52 57 PM" src="https://user-images.githubusercontent.com/99001393/163746941-f88132ce-d83e-4f14-a6f4-17f4f5ee84af.png">

  

Number of Retirement eligible employees by title:

<img width="196" alt="Screen Shot 2022-04-17 at 9 45 55 PM" src="https://user-images.githubusercontent.com/99001393/163746308-adfac8da-0fc2-41f2-9716-72ab5f795f83.png">


Deliverable 2

Using the ERD I created as a reference and  SQL, created a mentorship-eligibility table that holds the current employees who were born between January 1, 1965 and December 31, 1965.


<img width="1113" alt="EmployeeDB" src="https://user-images.githubusercontent.com/99001393/163746331-e1dd0506-b078-4b6b-ad04-030a32347ead.png">

### Along with filtering birthdates to conclude who was elgible for the mentorship program we ensured that the table only drew information on *current employees* from the employee database. We did that by adding:

 - AND (de.to_date = '9999-01-01') -

## This tells the query that we are only looking at employees without a defined end date at the company.

<img width="510" alt="Screen Shot 2022-04-17 at 10 17 00 PM" src="https://user-images.githubusercontent.com/99001393/163749015-eff32e5d-c685-45c5-b684-a2d3596cdc21.png">



<img width="789" alt="Screen Shot 2022-04-17 at 10 20 26 PM" src="https://user-images.githubusercontent.com/99001393/163749275-5c735b31-685d-42b3-b0f6-3e39289e5d34.png">



Summary:

## How many roles will need to be filled as the "silver tsunami" begins to make an impact?
### There are 72458 roles that are included in retirement eligibilty. 

## Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?

### If they are able to implement the mentorship prontorship program each employee as a mentor would be in charge of mentoring too large of a group of people considering that there were only 1549 employees considered eligible for this program. This program should still be implemented as soon as possible to atleast create some ease through such a large transition for the company.
