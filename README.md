# PyCitySchools with Pandas
Module 4 Challenge Data Analysis File Links
- ![PyCitySchools_Challenge.ipynb](https://github.com/aseo67/school-district-analysis/blob/main/PyCitySchools_Challenge.ipynb)
- ![schools_complete.csv](https://github.com/aseo67/school-district-analysis/blob/main/Resources/schools_complete.csv)
- ![students_complete.csv](https://github.com/aseo67/school-district-analysis/blob/main/Resources/students_complete.csv)

## Overview of School District Analysis
The city school district is looking to understand results for a recent standardized test, seeking insight into students' and schools' performance trends and patterns. This analysis prepares this standardized test data for analysis and reporting, so that the School Board and Superintendent can use these insights to inform strategic decisions at the school and district level, regarding budgets and priorities. 

One complication associated with this standardized test is that there is evidence of academic dishonesty among ninth graders attending Thomas High School (THS), in the form of grade alterations. In order to preserve the integrity of the testing data, this analysis removes the scores for ninth graders at Thomas High School and analyzes the performance of all remaining students. 

## Results
### How is the district summary affected?
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_District%20Summary%20-%20PostChallenge.png)
### How is the school summary affected?
  **School Summary: Top 5 Schools**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary%20-%20Top5.png)
  **School Summary: Bottom 5 Schools**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary%20-%20Bottom5.png)

### How does replacing the ninth graders' math and reading scores affect Thomas High School's performance relative to the other schools?
  **Thomas High School Performance: Pre-Removal of Ninth Grade Scores**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary_PreChallenge.png)
   **Thomas High School Performance: Post-Removal, Pre-Recalculating Percentages**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary_THS%20PreReplace.png)
   **Thomas High School Performance: Post-Removal, Final Percentages**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary_THS%20PostReplace.png)
### How does replacing the ninth grade scores affect the following: 
#### - Math and reading scores by grade
  **Math Scores by Grade**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_Math%20Scores%20By%20Grade.png)
  **Reading Scores by Grade**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_Reading%20Scores%20By%20Grade.png)

#### - Scores by school spending
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_Spending%20Summary.png)

#### - Scores by school size
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Size%20Summary.png)

#### - Scores by school type
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Type%20Summary.png)

## Summary
Four changes in the updated school district analysis after scores for Thomas High School Ninth Graders have been replaced with "NaN"s: 
 1. This analysis now involves extra script for replacing all Thomas High School Ninth Graders' scores with "NaN", in order to remove their test results form the dataset. 
  **Screenshot of Code for Updated Student Data - Thomas High School Ninth Graders' scores replaced with "NaN"**  
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Code%20for%20Deliverable%201_Replace%20Gr.9%20Thomas%20HS%20Grades%20to%20NaN.png)
  **Screenshot of Updated Student Data - Thomas High School Ninth Graders' scores replaced with "NaN"**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%201_Replace%20Gr.9%20Thomas%20HS%20Grades%20to%20NaN.png)
 2. Next, additional script was needed to determine the number of 10-12th graders at Thomas High School, as all test results for this school would only correspond to these students, rather than the entire THS student population. 
  **Screenshot of Code/Result for Re-calculatio of Total # of Students Passing among THS 10-12th graders**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Code%20for%20Deliverable%201_THS%20New%20Student%20Counts.png)
 3. With the new student count of THS 10-12th graders only, the appropriate "% Passing" percentages can be calculated for each of the tests (reading and math) and overall (for those passing both tests). 
  **Screenshot of Code/Result for Re-calculation of % Passing Percentages among THS 10-12th graders**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Code%20for%20Deliverable%201_ReCalculating%20Total%20Passing%20%2B%20Percentages.png)
 4. Finally,
  
