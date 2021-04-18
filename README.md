## Analysis for Pewlett Hackard

### Overview

This analysis of Pewlett Hackard's HR data breaks down the numbers for employees that will soon retire. With a great number of employees on the verge of retirement, this analysis give company management the opportunity to select employees eligible for training to take over the retirees' jobs. 

### Results

Here are the four major findings from the analysis:


* After running a SUM() function on retiring_titles table, the total number of retiring titles is 90398. Using the COUNT() method on employee numbers from the employees table, there are currently 300024 employees at the company, which means 30.13% of all employees are retiring. 

* The breakdown of retiring job titles shows that Senior Engineer (29414 people) and Senior Staff (28254 people) are the two biggest positions that will begin to see retirees. 

* To create the mentorship eligibility table, all employees are filtered to show those born in 1965 only and are current employees of the company. The list is then sorted by arranging employee numbers column in ascending fashion, and also sorting the most recent employment date column (to_date) from titles table in descending fashion. Using COUNT() on the employee numbers column, there is a total of 1549 current employees eligible for mentorship. 

* Using the COUNT() function on the 'title' column in the mentorship eligibility table, the total number of eligible employees by title can be seen [here](https://github.com/donovancai/Pewlett-Hackard-Analysis/blob/main/eligible_for_mentorship.png). Senior Staff and Senior Engineer are the two titles with the most eligible employees for mentorship. 

### Summary

#### How many roles will need to be filled as the "silver tsunami" begins to make an impact?

A total of 90398 positions will need to be filled, about 1/3 of total employees at the company. 


#### Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of Pewlett Hackard employees?
There are not enough qualified, retirement-ready employees in the departments to be mentored. There are 569 eligible Senior Staff to be mentored for 28254 Senior Staff due to retire, a mere 2.01% of future vacancies. Also the same situation occurs for Senior Engineers, with only 529 eligible Senior Engineers for 29414 future Senior Engineer vacancies, which is just 1.8% of the retirees. 
