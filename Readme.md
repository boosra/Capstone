# Capstone: Strategies for Women in Tech to Negotiate a Salary

##### Najiha Boosra [Github](https://git.generalassemb.ly)

## Table of Contents:  
 - **[Problem Statement](#Problem-Statement)**.

 - **[Executive Summary](#Executive-Summary)**.  

 - **[Data Dictionary](#Data-Dictionary)**.

 - **[Project Files](#Project-Files)**.  

 - **[Datasets](#Datasets)**   

 - **[Conclusions and Recommendations](#Conclusions-and-Recommendations)**.  

 - **[References](#References)**.

### Problem Statement:

There 's plenty of talk about "women in tech" right now.

Women in Tech are a minority in the industry and don't have many tools to help them navigate the business For both new hires and seasoned industry veterans, the most challenging aspect of taking a new job is salary negotiation.

If discussing what one have earned — and what one expect to earn — makes one uncomfortable. A survey from Glassdoor reports that 60 percent of woman and 48 percent of men believe salary history questions should not be asked. Women are also less likely to negotiate compensation, two out of three women (68 percent) do not negotiate pay compared to just about 52 percent of men.

We at NB Recruiting help place women in rewarding tech positions. Our goal is build a regression model to help predict assesses various features like education, job types, and organization, to help a woman predict her likely salary in a new job. Also for them who want to switch their job. It’s a good idea to research the job and the employer to be sure that the compensation package is negotiable.We will use root mean squared error (RMSE) as our regression metric to evaluate the success of our models.

### Executive Summary

The objective of our study is to use regression to examine the [data.world](https://data.world/finance/data-professional-salary-survey/workspace/file?filename=2019_Data_Professional_Salary_Survey_Responses.xlsx) dataset, which includes Job title, years with this type of job,  salary, and additional benefits, gathered from women all over the world. For this study, we will limit our scope to just US working women.


Our US-only dataset has 6893 observations. We cleaned the data replaced NaN values, checked for duplicates, and did extensive  exploratory data analysis, looking for individual columns of  importance to Salary, our target variable. Some variables were feature engineered to focus on the important aspects of this problem.


We checked only in the USA what type of jobs are popular in given survey years, also find out that jobs salary especially for women. women who have jobs but for some reason, they are looking for another job.  We checked how long they worked per week. How much they are getting paid with having a certificate, education level, and job status. Based on the primary database, we also look for years of working women, how about their salary, and career plan. We have a clear vision from our EDA part about Salary dependency.


Before women even think about negotiating salary, it’s important to know how much they expect to earn in their next job. If the offer isn’t close, they don’t need to take it. If they were expecting \\$60k, for example, and the offer is for \\$40k, it is probably too much of a reach. This model is designed to help women  rethink their expectations and land the right job.

### Data Dictionary:  

| **Data Name**              |  **Data Type** |                          **Description**                         |
|----------------------------|:--------------:|:----------------------------------------------------------------:|
| Survey Year                |      int64     |                   years of 2017, 2018 and 2019                   |
| Timestamp                  | datetime64[ns] |                             datetime                             |
| SalaryUSD                  |     object     |                      Salary is given in USD                      |
| Country                    |     Object     |                      Countries of the survey                     |
| PrimaryDatabase            |     Object     |                     Tech related Job database                    |
| YearsWithThisDatabase      |      int64     |        How many year people are working in these databases       |
| EmploymentStatus           |     Object     |   Type of employee statuses like full time/per time and others   |
| JobTitle                   |     Object     |         Title of the Job related to the primary database         |
| ManageStaff                |     Object     | Title of the Job related to the Managing staff as a boolean form |
| YearsWithThisTypeOfJob     |      int64     |         How many years people are working with these jobs        |
| CompanyEmployeesOverall    |     Object     |               Range of total employees in companies              |
| Education                  |     Object     |                        Level of education                        |
| EducationIsComputerRelated |     Object     |           Education is related to computer based or not          |
| Certifications             |     Object     |              Their certificates are valid or expired             |
| HoursWorkedPerWeek         |      int64     |             How many hours per week they are working             |
| LookingForAnotherJob       |     Object     |           Who are looking for new job passively or not           |
| CareerPlansThisYear        |     Object     |              about career plan they are asked or not             |
| Gender                     |     Object     |               Male, Female and Other gender people               |

### Project Files:

MainNoteBook.ipynb

### Datasets:

1. Main dataset: '2019_Data_Professional_Salary_Survey_Responses.xlsx'
2. cleaned dataset : 'cleaned_dataframe.csv'

### Conclusion and Recommendations:

Our Decision Tree Regressor was able to give us the most successful RMSE scores and was selected as the best model to help solve our study problem. But If I get more time I will go over unexpected columns importance again to have a more proper prediction.

Negotiating salary isn’t easy, and it can be especially difficult for women. In general, women are less likely to ask for more money when they are offered a job and more likely to stay in a lower paid job. Reasons vary, but some of it involves being uncomfortable discussing salary and being hesitant to ask for more.

Some experts believe one should always negotiate salary and ask for more money. Before one do that though, it’s a good idea to research the job and the employer to be sure that the compensation package is negotiable. There are some positions where the pay rate is set in advance. On the plus side, there won’t be gender discrimination because everyone is paid the same. On the negative side, what you are offered is what you will be paid.Our model will help Women of the United State to know what should they research for, how much they can get hourly in which job or title of the job, how much their education is necessary to have a better salary.

### References:

1. [Data.world](https://data.world/finance/data-professional-salary-survey/workspace/file?filename=2019_Data_Professional_Salary_Survey_Responses.xlsx)

2. https://www.roberthalf.com/blog/compensation-and-benefits/who-most-likely-negotiated-salary
