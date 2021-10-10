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
- Pandas Library
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
- School: *Thomas High School*
- Grade: *9*
- Subjects: *Reading* and *Math*

Then, the reading and math scores for the ninth graders in Thomas High school have been replaced with *NaNs*. An example of the resulting DataFrame is below.

![image00](/Resources/New_THS_Student_Scores_by_Grade.png)

### Revised Analysis: Deliverable 2 ###
To eliminate the impact of the altered 9th grade math and reading scores at Thomas High School, we excluded the impacted scores and the corresponding student record counts from the Score and % Passing analyses and rerun the entire distric school metrics based on a modified dataset.

The ***rerunning the analysis*** has generated the following ***revised metrics***.

**1. A high-level snapshot of the district's key metrics, presented in a table format**
![image4](/Resources/New_District_Summary.png)

In the revised analysis, the **distric summary has been affected** as follows.

| Metrics | Revised Analysis | Initial Analysis | Impact |
|-------|-------|------|-------|
|Average Math Score | 78.9   | 79.0 | Has been reduced in the revised analysis  |
|Average Reading Score | 81.9   | 81.9 | Unchanged (changed below the level of material significance)   |
|% Passing Math |  74.8%  | 75.0% |  Has been reduced in the revised analysis |
|% Passing Reading | 85.7%   | 85.8% | Has been reduced in the revised analysis  |
|% Passing Overall |  64.9%  | 65.2 | Has been reduced in the revised analysis  |

**2. An overview of the key metrics for each school presented in a table format**
![image8](/Resources/New_per_School_Summary_Excl_Grade_9.png)

In the revised analysis, only one school's metrics got **impacted: the metrics of Thomas High School** (below are rounded to 2 decimal points)
| Metrics | Revised Analysis | Initial Analysis | Impact |
|-------|-------|------|-------|
|Average Math Score | 83.35   | 83.42 | Has been reduced in the revised analysis  |
|Average Reading Score | 83.90   | 83.85 | Has been increased in the revised analysis   |
|% Passing Math |  93.19%  | 93.27% |  Has been reduced in the revised analysis |
|% Passing Reading | 97.02%   | 97.31% | Has been reduced in the revised analysis  |
|% Passing Overall |  90.63%  | 90.95% | Has been reduced in the revised analysis  |

**3. Tables presenting each of the following metrics:**

    3.a. Top 5 and bottom 5 performing schools, based on the overall passing rate
    
    Top 5 Schools in the District
  ![image19](/Resources/New_Top_5_Schools.png)
  
Replacing the ninth graders’ math and reading scores **did not affect Thomas High School’s performance relative to the other schools** : they maintained the second position in the Top 5 schools in the District. However, the marginal advantange that Thomas High School had to Griffin High Scholl has shrunk.
    
    Bottom 5 Schools in the District
  ![image2](/Resources/New_Bottom_5_Schools.png)
  
    3.b. The average math score received by students in each grade level at each school
  ![image6](/Resources/New_Math_by_Grade.png)
  
Only one metrics has changed in the table as a result of the revised analysis: **Thomas High School Math scores for 9th grade students**: In the revised analysis, we exclude the scores from consideration and they show as *NaN*; in the initial analysis, the Math score for 9th graders have been *83.6*
  
    3.c. The average reading score received by students in each grade level at each school
  ![image11](/Resources/New_Reading_by_Grade.png)
  
Only one metrics has changed in the Table as a result of the revised analysis: **Thomas High School Reading scores for 9th grade students**: In the revised analysis, we exclude the scores from consideration and they show as *NaN*; in the initial analysis, the Reading score for 9th graders have been *83.7*
  
    3.d. School performance based on the budget per student
  ![image17](/Resources/New_Spending_Ranges.png)

In the revised analysis these **metrics have not changed** (based on the level of materiality).

    3.e. School performance based on the school size 
  ![image15](/Resources/New_Size_Ranges.png)

In the revised analysis these **metrics have not changed** (based on the level of materiality).
    
    3.f. School performance based on the type of school
  ![image13](/Resources/New_School_Type.png)

In the revised analysis these **metrics have not changed** (based on the level of materiality).

## Summary ## 

**The revised analysis conducted on the dataset with replaced reading and math scores for Thomas High School (THS) 9th Grade students has reveals the following dymanics:**

1. Thomas High School 9th grade Reading scores have been **increased**
2. Thomas High School 9th grade Math scores have been **reduced**
3. Thomas High School 9th grade Reading % Passing has been **reduced**
4. Thomas High School 9th grade Math % Passing has been **reduced**
5. Thomas High School 9th grade Overall % Passing has been **reduced**
6. City School District Math scores, % Passing for Math, Reading, and Overall have been **reduced**

Based on the analysis, certain conclusions could be made that might be helpful in the investigation of who is responsible for the student score alteration:
1. The **Math** scores for 9th graders at THS had been unlawfully altered by increasing both, the scores and the passing %, consistently accross the 9th grade at THS
2. The **Reading** scores for 9th graders at THS had been unlawfully altered by increasing the Scores for selected students at 9th grade that were likely failing the course while trying to keep the overall Passing % for Reading unchanged, which required to reduce the Reading scores for some other students in the 9th Grade to the level that they appeared as failed. This could be a reason why the the overall Reading scores in the revised analysis are higher than in the initial analysis.
