# School District Analysis
## Project Overview
We have been tasked with analyzing standardized test data to glean insights on school performance; This analysis will discuss how factors like school size, type (public or charter), and the amount spent per student affect the pass rate. 

### Purpose
We will deploy a python jupyter notebook to read and merge two .csv files, then investigate this data.

---
## Analysis
Before we can start the analysis we've been informed that 9th graders from Thomas High School have corrupt data. To rectify this mistake we must first replace the 9th graders' math and reading score with N/A values. <br />
<img width="672" alt="1) Remove, 9th grade, format" src="https://user-images.githubusercontent.com/79609464/161644425-86fa688b-9700-47eb-99cc-b0a6ed277044.png">

Now we are going to merge the schools and students data frame; this allow us to manipulate both data frames at once. <br />
<img width="831" alt="2) Merge" src="https://user-images.githubusercontent.com/79609464/161644431-02ccd8b2-3515-4c4c-96ad-306c2b71d441.png">

#### District Statistics <br />
<img width="937" alt="3) Overall Statistics" src="https://user-images.githubusercontent.com/79609464/161644434-877b7e58-731b-4f1c-86c1-acc086ba57dc.png">

#### Top Five Schools
<img width="1002" alt="4) Top Five" src="https://user-images.githubusercontent.com/79609464/161644436-88bb8161-60a2-4d58-9476-28c532ac0e3d.png">

#### Bottom Five Schools
<img width="999" alt="5) Bottom five" src="https://user-images.githubusercontent.com/79609464/161644440-1c68dd9d-0254-4394-9951-8c6ef89bd6d6.png">

#### Schools Average Reading and Math Scores by Grade
From the table below its clear the variance of scores between grades is relatively low; hence, grade level is not a determining factor of test scores.<br />
<img width="500" alt="Screen Shot 2022-04-09 at 11 17  (2)" src="https://user-images.githubusercontent.com/79609464/162584898-b7d1804b-d6b0-4f64-ac93-7ba10a5a36a1.png">


#### Amount Spent Per Student vs Pass Rates
By soley observing this dataframe an inversly proportional trend emerges between the amount spent per student and the pass rates.<br />
<img width="828" alt="8) Pass rates by amount spent per student" src="https://user-images.githubusercontent.com/79609464/161644447-17201be3-271a-4aae-8038-cfeeb4547119.png">

#### School Size vs Pass Rates
These results speak more to the inefficiencies of large schools than to the success of small and medium schools; the most obvious trend is that schools with a population over 2,000 tend to have significantly lower pass rates. The pass rates from small to medium schools are extremely similar; though we would expect smaller schools to have greater pass rates than medium, this is not the case. The overall pass rate for medium schools is even greater than that of small schools. <br />
<img width="774" alt="9) Pass Rates by school size" src="https://user-images.githubusercontent.com/79609464/161644449-55739d1d-dfd3-4679-b285-fb625b694679.png">

#### Public and Charter vs Pass Rates
From these results its clear Charter schools have a greater pass rate than public schools. <br />
<img width="729" alt="10) Public Vs  Charter" src="https://user-images.githubusercontent.com/79609464/161644466-2055d6c3-10dd-4d3f-8c33-f1ac9c1dfaa8.png">

### Challenges and Difficulties Encountered
In trying to put together a full picture, this data seems to be missing some pieces like student satisfaction rating, bullying levels, etc; Standardized test pass rates are surely one metric- and probably the easiest to gauge- but it doesn't capture what the environment is like. The reason this is important is that metrics like the amount of money spent per student need context to be properly interpreted; right now it's saying the less money we spend per student, the more successful they'll be- but that seems suspicious. For example, if we are comparing a "rich" charter school and an "impoverished" public school, both of them may have the same amount of money spent per student. In the charter school, the extra money goes to pay the teachers and admin, allowing them to have a high retention level; to make up for these gaps, rich parents will provide money for extracurricular activities- buying the football team new gear. Impoverished public schools will not have the same luxury. Furthermore, this pattern is supported by the Top and Bottom five schools' table; both of these categories spend roughly the same amount per student. The only difference- in our recorded metrics- is the size of each school. Though the size of the school is an important factor and maybe the most important, it can't be the only factor; there must be another metric outside our data frame affecting these results. Things like bullying, satisfaction level, afterschool assistance, and extracurriculars could surely affect the graduation rate.

---
## Results
- Charter schools perform better than public schools on a standardized test.
- Schools with a population of less than 2,000 outperform those with a population larger than 2,000.
- Schools with a medium population outperform schools with a population of less than 1,000.
- Grade level does not affect performance on standardized tests.
- The amount spent per student at top-performing schools is the same as the bottom performing.
- The amount spent per student is an important factor, but charter schools tend to receive- and rely on- donations outside of the district budget.
- The main difference between public and charter schools is attention to the skewness of their pass rates
  - Public schools have a lot of students on the failing side of this distribution; its normally distributed around the mean
  - Charter schools don't have any- or very few outliers- that lie below the mean; their data is skewed left.

---
## Summary
Charter schools are more successful- in terms of pass rates- than public schools; This can be attributed to several reasons outside the scope of our data. Before we replaced the n/a values this data set would have told a much different story; Thomas Highschool would have been in the bottom five schools instead of the top five. Thus we couldn't have concluded charter schools are more successful. Additionally, this would have changed how we viewed medium-sized schools; instead of marginally outperforming small schools, medium schools would have appeared to perform nearly as poorly as large schools. This would have also affected our district statistics and average scores.

---
