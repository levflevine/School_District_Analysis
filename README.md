# School District Analysis
## Overview ##
The Office of Chief Data Scientist of a City School Distric has requested to aggregate various student and school data and reveal the trends in school performance in order to make decisions on the school budgets and priorities.

### Initial Analysis ###
The ***initial project scope*** included the following analysis of the school district deliverables: 
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
Upon completion of the initial project scope, the School Board has determined that the student raw data records demonstrated evidence of academic dishonesty. Specifically, reading and math grades for Thomas High School ninth grade students appeared to have been altered. Consequently, ***second phase of the project*** has been approved that required the following deliverables.

#### Deliverable 1: ####
- Replacing the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact

#### Deliverable 2: ####
- Rerunning the school district analysis 

#### Summary Report: ####
- Producing a report to describe how these changes affected the overall analysis
 
### Resources and Disclosures ###
The analysis of school data has used  following open-software packages: 
- Anaconda 
- Jupyter Notebook

The city school district data has been published and can be located [here](https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-online/module_4/schools_complete.csv).

In compliance with the Family Education Rights and Privacy Act (1974) that protects the privacy of all student educational records in the US, the student names and IDs have been altered and do not represent the personally identifiable infromation. The altered student data can be found [here](https://2u-data-curriculum-team.s3.amazonaws.com/dataviz-online/module_4/students_complete.csv).

## Results ##
### Initial Analysis ###
The ***initial analysis*** has generated the following metrics.

**1. A high-level snapshot of the district's key metrics, presented in a table format**
![image4](/Resources/Old_District_Summary.png)

**2. An overview of the key metrics for each school presented in a table format**
![image8](/Resources/Old_per_School_Summary.png)

**3. Tables presenting each of the following metrics:**

    3.a. Top 5 and bottom 5 performing schools, based on the overall passing rate
    
    Top 5 Schools in the District
  ![image19](/Resources/Old_Top_5_Schools.png)
  
    Bottom 5 Schools in the District
  ![image2](/Resources/Old_Bottom_5_Schools.png)
  
    3.b. The average math score received by students in each grade level at each school
  ![image6](/Resources/Old_Math_by_Grade.png)
  
    3.c. The average reading score received by students in each grade level at each school
  ![image11](/Resources/Old_Reading_by_Grade.png)
  
    3.d. School performance based on the budget per student
  ![image17](/Resources/Old_Spending_Ranges.png)
  
    3.e. School performance based on the school size 
  ![image15](/Resources/Old_Size_Ranges.png)
  
    3.f. School performance based on the type of school
  ![image13](/Resources/Old_School_Type.png)

### Revised Analysis: Deliverable 1 ###
The altered student score records have been identified based on the following criteria: 
- School: Thomas High School
- Grade: 9
- Subjects: Reading and Math

Then, the reading and math scores for the ninth graders in Thomas High school have been replaced with NaNs. An example of the resulting DataFrame is below.

![image00](/Resources/New_Student_Scores_by_Grade.png)

### Revised Analysis: Deliverable 2 ###
To eliminate the impact of the altered 9th grade math and reading scores at Thomas High School, we excluded the impacted scores and the corresponding student records from the analysis and rerun the entire distric school metrics based on a reduced dataset.

The ***rerunning the analysis*** has generated the following ***revised metrics***.

**1. A high-level snapshot of the district's key metrics, presented in a table format**
![image4](/Resources/New_District_Summary.png)

**2. An overview of the key metrics for each school presented in a table format**
![image8](/Resources/New_per_School_Summary_Excl_Grade_9.png)

**3. Tables presenting each of the following metrics:**

    3.a. Top 5 and bottom 5 performing schools, based on the overall passing rate
    
    Top 5 Schools in the District
  ![image19](/Resources/New_Top_5_Schools.png)
  
    Bottom 5 Schools in the District
  ![image2](/Resources/New_Bottom_5_Schools.png)
  
    3.b. The average math score received by students in each grade level at each school
  ![image6](/Resources/New_Math_by_Grade.png)
  
    3.c. The average reading score received by students in each grade level at each school
  ![image11](/Resources/New_Reading_by_Grade.png)
  
    3.d. School performance based on the budget per student
  ![image17](/Resources/New_Spending_Ranges.png)
  
    3.e. School performance based on the school size 
  ![image15](/Resources/New_Size_Ranges.png)
  
    3.f. School performance based on the type of school
  ![image13](/Resources/New_School_Type.png)


Using bulleted lists and images of DataFrames as support, address the following questions.

How is the district summary affected?
How is the school summary affected?
How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
How does replacing the ninth-grade scores affect the following:
Math and reading scores by grade
Scores by school spending
Scores by school size
Scores by school type





## Summary ## 

Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
