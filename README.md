# Pandas Challenge
Week 4 - Data Analytics Boot Camp - University of Oregon

![Pandas Challenge](/images/education.png)

## Scenario
You are the new Chief Data Scientist for your city's school district. In this capacity, you'll be helping the school board and mayor make strategic decisions regarding future school budgets and priorities.

As a first task, you've been asked to analyze the district-wide standardized test results. You'll be given access to every student's math and reading scores, as well as various information on the schools they attend. Your task is to aggregate the data to showcase obvious trends in school performance.


## Instructions
Using Pandas and Jupyter Notebook, create a report that includes the following data. Your report must include a written description of at least two observable trends based on the data.

### District Summary
Perform the necessary calculations and then create a high-level snapshot of the district's key metrics in a DataFrame.

Include the following:
- Total number of unique schools
- Total students
- Total budget
- Average math score
- Average reading score
- % passing math (the percentage of students who passed math)
- % passing reading (the percentage of students who passed reading)
- % overall passing (the percentage of students who passed math AND reading)


### School Summary
Perform the necessary calculations and then create a DataFrame that summarizes key metrics about each school.

Include the following:
- School name
- School type
- Total students
- Total school budget
- Per student budget
- Average math score
- Average reading score
- % passing math (the percentage of students who passed math)
- % passing reading (the percentage of students who passed reading)
- % overall passing (the percentage of students who passed math AND reading)

### Additional Charts
Create DataFrames for the following:

- Highest-Performing Schools
  - Schools sorted highest to lowest by % Overall Passing
- Lowest-Performing Schools
  - Schools sorted lowest to highest by % Overall Passing
- Math Scores by Grade
  - Summery of school grades broken down by student year.
- Reading Scores by Grade
  - Summery of school grades broken down by student year.
- Scores by School Spending
  - Categorize school spending by cost per student using pd.cut
- Scores by School Size
  - Categorize school by size of student body using pd.cut
- Scores by School Type
  - Summery of scores categorized by charter and district schools.


## Observations
Charter schools have a high overall passing rate of 90.4%.  District schools, on the other hand, have a poor overall passing rate of 53.7%, which require a closer look to identify the underlying problem.

If we compare at math and reading passing rates between charter and district schools, we see that charter schools do well in both reading and math.  Charter school’s passing rate in reading is 96.6% with an average reading score of 83.9%.  Their passing rate in math is 93.3% with an average math score of 83.5%.
District schools seem to be doing OK in reading with a passing rate of 80.8% with an average reading score of 81.0%.  However, they are falling well below expected rates in math scores.  District school’s passing rate in math is only 66.4% with an average math score of 76.9%.
It seems that district students struggling in math may not be getting the support they need.  As a result, those struggling in math tend to pull down the overall passing percentage for district schools.  

In an effort to identify the discrepancies, we can look at the size of the student enrollment.  Charter schools tend to have fewer students, and most are classified as small to medium size (under 2000 students).  Whereas district schools are exclusively categorized as large schools (2000-5000 students).  It would be good to gather data on the student to teacher ratio, as this may impact the success of students.

In general, Charter schools have the lowest cost per student whereas district schools have a higher cost per student.  This brings up the question as to how they are investing their money.  Are charter schools hiring better quality teachers?  It might be worth comparing the average salary of a charter school teacher with the average salary of a district school teacher.  Perhaps hiring better quality teachers are contributing factor to success rates.  

District schools have higher cost per student, but this may be the result of school size.  Large schools have more overhead costs that are not directly related to teaching costs.  It would be good to break down budgets of overhead vs teaching expenses to see if there are any differences in the allocation of funding between charter and district schools.

Since district schools are struggling in the math department, it is worth looking at the allocation of budget and resources specifically in the math dept to see if there is a way to bolster the success rate.  Perhaps hiring more teachers so classroom sizes are smaller and students get more 1:1 learning, or tutoring programs to get homework help.
Another area to look at is how often students miss class.  Math is a subject where the current lesson builds upon the previous lesson.  If a student misses or doesn't understand one of the lessons, it is easy to fall behind and not catch up.  It would be good to look at if students are more likely to miss lessons in charter vs district schools.  Or if there is support for students to get caught up on areas where they struggle.

Additionally, it may be worth looking at is the location of charter vs district schools.  Are charter schools more available in affluent neighborhoods than district schools?  Checking the average household income may be an indicator of a school’s demographic.  Affluent neighborhoods may have better access to resources and more parent involvement with school activities, which may impact a student’s success.  

