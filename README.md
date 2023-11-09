# DEI, PIP, and Management Analyses Project 

## Summary

In this project, I made use of a fictitious employee dataset to answer critical business questions across several topics. 

**Management Practices**

* How do and job performance, engagement levels, and satisfaction levels vary for employees under different managers?

**Performance Improvement Plans**

* How effective are the company's Performance Improvement Plans (PIP's)?

**Diversity, and Equity**

* What is the overall diversity profile of the company?
* Which recruiting sources promote diversity?
* Is compensation at the company equitable between identity groups?

The entire project is contained in the attached Jupyter notebook, where I begin by programmatically collecting the data from the Kaggle website; then clean and manipulate the dataset to prepare it for analysis; then perform exploratory data analysis, which provided and overview of the dataset and revealed unexpected insights; and finally answer the specific business questions posed above. The notebook has many visualizations and comments that make it easy to follow my thought process. 

Dataset Link: https://www.kaggle.com/datasets/rhuebner/human-resources-data-set/data

## Exploratory Data Analysis

From the EDA alone, a number of insights about the company's workforce revealed themselves, informing the following recommendations:

1) The more engaged and satisfied employees are, the higher performing they tend to be. This means that the company should look to promote employee engagement and satisfaction not only to improve employee experience, but also to boost job performances. Importantly, engagement is an even higher priority than satisfaction for this goal since the former is more strongly correlated with performance

2) The company is doing a good job making sure that its employees are engaged at work, but there is substantial room for improvement in terms of employee satisfaction

3) Employees that are late to work more frequently tend to be less engaged, less satisfied, and worse performing. This means that monitoring employees' tardiness could provide insight into their engagement, satisfaction, and job performance without the need for more costly and time-consuming surveys and performance reviews

4) The company website accounts for a very small (< 5%) portion of employee recruitments. The company should investigate whether there are problems with the website that could explain this. For example, the website could be designed in a way that makes it difficult to navigate to the 'Careers' page, or the positions listed on the website could not be up-to-date

5) One of the most common reasons that employees left the company was because they were offered more money elsewhere. There is also a very weak correlation between job performance and salary. The company should thus evaluate whether they are properly compensating their high performing employees so that they don't lose them

## Management Practices Analysis

Since an employee's manager can have a big impact on their engagement levels, satisfaction levels, and job performance, it makes sense for the company to ask whether different managers are associated with differences in these KPI's. The answer to this question could highlight which managers seem to be managing their employees better, and also inform intervention strategies aimed at improving management practices within the company. 

To address this question, I conducted the appropraiate ANOVA's for each KPI (based on whether the distribution of the KPI violated the assumption of homoscedasticity). All three resulted in p-values > 0.05, which led me to conclude that there was insufficient evidence to conclude that engagement levels, satisfaction levels, and job performance varied in a statistically significant way between managers. 

## Performance Improvement Plan Efficacy Analysis

The company assigned employees with the lowest possible performance scores to Performance Improvement Plans (PIP's). I set out to investigate whether programs were effective at improving performance by comparing the rates of involuntary terminations of employees assigned to PIP's and employees with the second-lowest performance score ('Needs Improvement'), who were not assigned to PIP's. 

The initial evidence seemed to support the efficacy of PIP's, as the rates of involuntary termination for 'PIP' and 'Needs Improvement' employees were 15.4% and 27.8%, respectively. However, a chi-square test showed that there was insufficient evidence to conclude that the PIP's elevated employee performance so much that the employees outperformed those scoring a grade above in performance evaluations. Importantly, this analysis was constrained by a small sample size, with fewer than 20 employees in each group, which greatly limited the test's statistical power (its ability to capture a true effect). As a result, the company should continue investing in the PIP's and monitoring employee outcomes, and run a similar analysis once sample sizes increase. 

## Diversity and Equity Analysis
