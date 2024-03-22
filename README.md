#  Data Professional Survey Analysis

### Problem Statement

This project aims to analyze the responses collected from an online survey of data professionals. The survey captured various aspects related to the data professionals' roles, career trajectories, job satisfaction, and demographic information.

### Survey Fields

1. Unique ID: Unique identifier for each survey response.
2. Email: Email address of the respondent.
3. Date Taken (America/New_York): Date when the survey was taken (in the America/New_York timezone).
4. Time Taken (America/New_York): Time when the survey was taken (in the America/New_York timezone).
5. Browser: Web browser used to take the survey.
6. OS: Operating system of the device used to take the survey.
7. City: City of residence of the respondent.
8. Country: Country of residence of the respondent.
9. Referrer: Source from which the respondent accessed the survey.
10. Time Spent: Time spent by the respondent to complete the survey.
11. Q1 - Which Title Best Fits your Current Role?: Respondent's current job title.
12. Q2 - Did you switch careers into Data?: Whether the respondent switched careers into the data field.
13. Q3 - Current Yearly Salary (in USD): Respondent's current yearly salary in USD.
14. Q4 - What Industry do you work in?: Industry in which the respondent works.
15. Q5 - Favorite Programming Language: Respondent's favorite programming language.
16. Q6 - How Happy are you in your Current Position with the following?: Respondent's satisfaction levels in various aspects of their current position (e.g., Salary, Work/Life Balance, Coworkers, Management, Upward Mobility, Learning New Things).
17. Q7 - How difficult was it for you to break into Data?: Difficulty level the respondent faced when breaking into the data field.
18. Q8 - If you were to look for a new job today, what would be the most important thing to you?: Respondent's priority when looking for a new job.
19. Q9 - Male/Female?: Respondent's gender.
20. Q10 - Current Age: Respondent's current age.
21. Q11 - Which Country do you live in?: Country of residence of the respondent.
22. Q12 - Highest Level of Education: Respondent's highest level of education.
23. Q13 - Ethnicity: Respondent's ethnicity.


### Steps Followed
#### Data Cleaning
- Step 1 : Transform data into Power BI Desktop, dataset is a csv file.
- Step 2 : The columns browser, os, city, country, referrer are removed as they are empty. 
- Step 3: The column "Q1 - Which Title Best Fits your Current Role?" is modified by using split column - Delimiter is (. This creates a new column which is deleted. It simplifies the data in the Q1 - Which Title Best Fits your Current Role? column and limits the number of data fields.
- Step 4 : Perform step 3 for other columns that don't have a clearly defined data for the purpose of visualizing it later.
- Step 4 : Q3. Current yearly salary is a range so it's important to split in two columns having whole numbers so that we can take the average salary in a separate custom column (Average Salary)

#### Data Visualization
 - Step 1 : Open a text box and add title "Data Professional Survey Breakdown"
- Step 2 : Select a card option and insert the count of survey takers
- Step 3 : Select __card__ and insert __average age of survey takers__
- Step 4 : Select __stacked bar chart__ and plot for getting __average salary by job__ (average salary on the x axis v/s job title on the y axis) 
- Step 5 : Select __clustered column chart__ and plot count of unique id v/s favourite programming language to visualize their __favourite programming language__
- Step 6 : Using __Treemap__ group the total number of participants by country.
- Step 6 : Use __gauge__ to index __Happiness by Salary and Happiness by work life__ on a scale of 0 - 10
- Step 7 : Use __donut__ to find __average salary by gender__


### Insights and Visualizations Gained

- Country by Survey Takers : 261 participants from US, 73 participants from India, 40 from UK, 32 from Canada, 223 from other.

- Average Salary by Job Title: Data Scientist have the highest average salary with 94k USD followed by data engineer at 65k, data architect at 64k, data analyst at 55k, database developer at 33k and other at 60k

- Count of Survey Takers: Total count of survey takers is 630

- Average Age of Survey Takers: 29.87

- Happiness with Work-Life Balance: On a range of 0-10, average happiness with WLB is 5.74

- Happiness with Salary: On a range of 0-10, happiness with salary is 4.27

- Favorite Programming Language: Python is the favourite programming language followed by R

- Average Salary by Gender: Average salary for male is 55k, for female it is 53k

#### By analyzing these aspects, gained some insights into the career trajectories, job satisfaction levels, and demographics of data professionals. These insights can inform decision-making processes related to career development, job satisfaction enhancement, and talent acquisition strategies in the data field.
