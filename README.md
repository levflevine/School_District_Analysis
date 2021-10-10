# School District Analysis
## Overview ##
The Office of Chief Data Scientist of a City School Distric has requested to aggregate various student and school data and reveal the trends in school performance in order to make decisions on the school budgets and priorities.

### Initial Analysis ###
The initial project scope included the following analysis of the school district deliverables: 
- A high-level snapshot of the district's key metrics, presented in a table format
- An overview of the key metrics for each school presented in a table format
- Tables presenting each of the following metrics:
  - Top 5 and bottom 5 performing schools, based on the overall passing rate
  - The average math score received by students in each grade level at each school
  - The average reading score received by students in each grade level at each school
  - School performance based on the budget per student
  - School performance based on the school size 
  - School performance based on the type of school

### Revised Analysis ###
Upon completion of the initial project scope, the School Board has determined that the student raw data records demonstrated evidence of academic dishonesty. Specifically, reading and math grades for Thomas High School ninth grade students appeared to have been altered. Consequently, second phase of the project has been approved that required the following deliverables:
- Replacing the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact
- Rerunning the school district analysis 
- Producing a report to describe how these changes affected the overall analysis

### Resources and Disclosures ###
The analysis of school data has used  following open-software packages: 
- Anaconda 
- Jupyter Notebook

The city school district data has been published and can be located [here](https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-online/module_4/schools_complete.csv).

In compliance with the Family Education Rights and Privacy Act (1974) that protects the privacy of all student educational records in the US, the student names and IDs have been altered and do not represent the personally identifiable infromation. The altered student data can be found [here](https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-online/module_4/students_complete.csv).

## Results ##

Using bulleted lists and images of DataFrames as support, address the following questions.

How is the district summary affected?
How is the school summary affected?
How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
How does replacing the ninth-grade scores affect the following:
Math and reading scores by grade
Scores by school spending
Scores by school size
Scores by school type

![image1](/Resources/New_Bottom_5_Schools.png)
![image2](/Resources/Old_Bottom_5_Schools.png)
![image3](/Resources/New_District Summary.png)
![image4](/Resources/Old_District Summary.png)
![image5](/Resources/New_Math_by_Grade.png)
![image6](/Resources/Old_Math_by_Grade.png)
![image7](/Resources/New_per_School_Summary.png)
![image8](/Resources/Old_per_School_Summary.png)
![image9](/Resources/New_per_School_Summary_Excl_Grage_9.png)
![image10](/Resources/New_Reading_by_Grade.png)
![image11](/Resources/Old_Reading_by_Grade.png)
![image12](/Resources/New_School_Type.png)
![image13](/Resources/Old_School_Type.png)
![image14](/Resources/New_Size_Ranges.png)
![image15](/Resources/Old_Size_Rangse.png)
![image16](/Resources/New_Spending_Ranges.png)
![image17](/Resources/Old_Spending_Rangse.png)
![image18](/Resources/New_Top_5_Schools.png)
![image19](/Resources/Old_Top_5_Schools.png)

## Summary ## 

Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
