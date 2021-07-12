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
After removing the scores of Thomas High School 9th graders, the average math score for the district decreased by 0.1%, whereas the average reading score stayed consistent. The % of students passing decreased slightly overall, by ~0.2% for % Passing Math, by ~0.1% for % Passing Reading, and by ~0.3% for % Overall Passing. 
  
  **District Summary: Pre-Removal of THS Ninth Grade Scores**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_District%20Summary%20-%20PreChallenge.png)
  **District Summary: Post-Removal of THS Ninth Grade Scores**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_District%20Summary%20-%20PostChallenge.png)

### How is the school summary affected?
Although the THS 9th graders' scores have been removed, Thomas High Schools' rank (when schools are ranked by % Overall Passing) remains similar and maintains the rank #2 spot. All other schools scores/rank remain the same, given this removal of scores is isolated to Thomas High School. 

  **School Summary: Top 5 Schools - Pre-Removal of THS Ninth Grade Scores**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary_Top5%20-%20PreChallenge.png)
  **School Summary: Top 5 Schools - Post-Removal of THS Ninth Grade Scores**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary_Top5%20-%20PostChallenge.png)
  **School Summary: Bottom 5 Schools - Pre-Removal of THS Ninth Grade Scores**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary_Bottom5%20-%20PreChallenge.png)
  **School Summary: Bottom 5 Schools - Post-Removal of THS Ninth Grade Scores**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary_Bottom5%20-%20PostChallenge.png)

### How does replacing the ninth graders' math and reading scores affect Thomas High School's performance relative to the other schools?
Prior to removing scores, Thomas High School ranked #2 (as shown above in the School Summary), with an Overall % Passing of 90.9%. After removing the scores, Thomas High School maintains this ranking, but edges closer to the #3 spot, as its Overall % Passing is ~90.6% - <1% away from the next school (see School Summary screenshots above). 

  **Thomas High School Performance: Pre-Removal of Ninth Grade Scores**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary_PreChallenge.png)
   **Thomas High School Performance: Post-Removal, Final Percentages**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary_THS%20PostReplace.png)

### How does replacing the ninth grade scores affect the following: 
#### - Math and reading scores by grade
By removing the 9th grade scores from THS, there is now a "NaN" reflected in the following data tables (Math and Reading scores by grade). Only 10-12th graders' average scores are available for the Thomas High School row. 
 
  **Math Scores by Grade**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_Math%20Scores%20By%20Grade.png)
  
  **Reading Scores by Grade**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_Reading%20Scores%20By%20Grade.png)

#### - Scores by school spending
While removing the 9th grade scores for THS did change the average scores slightly, they still round to the same levels as before, resulting in a similar result for this Scores by School Spending analysis. 
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_Spending%20Summary.png)

#### - Scores by school size
While removing the 9th grade scores for THS did change the average scores slightly, they still round to the same levels as before, resulting in a similar result for this Scores by School Size analysis. 
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Size%20Summary.png)

#### - Scores by school type
While removing the 9th grade scores for THS did change the average scores slightly, they still round to the same levels as before, resulting in a similar result for this Scores by School Type analysis. 
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Type%20Summary.png)

## Summary
Four changes in the updated school district analysis after scores for Thomas High School Ninth Graders have been replaced with "NaN"s: 
 1. This analysis now involves extra script for replacing all Thomas High School Ninth Graders' scores with "NaN", in order to remove their test results from the dataset. The student data has been preserved for keeping track of who belongs to the 9th grade class of THS, but their scores are removed to prevent any unfair skewing of results. 
 
 **Screenshot of Code for Updated Student Data - Thomas High School Ninth Graders' scores replaced with "NaN"**  
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Code%20for%20Deliverable%201_Replace%20Gr.9%20Thomas%20HS%20Grades%20to%20NaN.png)
  **Screenshot of Updated Student Data - Thomas High School Ninth Graders' scores replaced with "NaN"**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%201_Replace%20Gr.9%20Thomas%20HS%20Grades%20to%20NaN.png)
 
 2. Next, additional script was needed to determine the number of 10-12th graders at Thomas High School, as all test results for this school would only correspond to these students, rather than the entire THS student population. 
  
  **Screenshot of Code/Result for Re-calculation of Total # of Students Passing among THS 10-12th graders**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Code%20for%20Deliverable%201_THS%20New%20Student%20Counts.png)
 
 3. With the new student count of THS 10-12th graders only, the appropriate "% Passing" percentages can be calculated for each of the tests (reading and math) and overall (for those passing both tests). This accurately calculates the passing percentages for the students of THS whose test scores are being counted. 
  
  **Screenshot of Code/Result for Re-calculation of % Passing Percentages among THS 10-12th graders**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Code%20for%20Deliverable%201_ReCalculating%20Total%20Passing%20%2B%20Percentages.png)
  **Thomas High School Performance: Post-Removal, Pre-Recalculating Percentages**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary_THS%20PreReplace.png)
   **Thomas High School Performance: Post-Removal, Final Percentages**
  ![Screenshot](https://github.com/aseo67/school-district-analysis/blob/main/Resources/Deliverable%202_School%20Summary_THS%20PostReplace.png)
 
 4. These updates have resulted in slightly different results for the overall analyses - district summary, school summary, scores by grade/ by school spending/ by school size/ by school type. While overall insights remain very similar (as the resulting changes are very small, shifting less than a percent in most cases), this is a more accurate reflection of actual student performance. 
  
