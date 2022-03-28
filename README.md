# School_District_Analysis
This repository uses Python, anaconda, panda and Jupiter notebooks


## Project Overview
The project aims to analyze the performance trends and patterns of about fifteen different schools by gathering various data using python Panda library. Maria, a chief Data scientist is responsible for analyzing the information from a variety of sources in a variety of format of the school district. Here the main analysis is focused on the performance of math and reading scores. However, after school board reviewed the data, it was determined that the data from Thomas High School's 9th grade class shows evidence of academic dishonesty. For this the math and reading scores for Thomas High School with "NaNs" while keeping the rest of the data intact and to repeat the school district analysis that was done in this module and write up a report to describe how these changes affected the overall analysis.

## New technologies used
1.	Anaconda with Python Data environment
2.	Jupyter notebook
3.	Pandas and Numpy libraries


## Main Steps involved in general
1. Open Jupyter Notebook files from local directories using a anaconda pythan data development environment.
2. Read an external CSV file into a DataFrame.
3. Replacing certain values with “NANs” usimg loc() function of nympy package.
4. Format a DataFrame column.
5. Determine data types of row values in a DataFrame.
6. Retrieve data from specific columns of a DataFrame.
7. Merge, filter, slice, and sort a DataFrame.
8. Apply the groupby() function to a DataFrame.
9. Use multiple methods to perform a function on a DataFrame.
10. Perform mathematical calculations on columns of a DataFrame or Series.
11. [Click Here for original code base of School District Analysis ](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb)
12. [Click Here for challenge code base of School District Analysis](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb)

## Result
### Initial screen shot
- Post Addition of NaN values to the School data dataframe: After the math and reading values are replaced with "NAN" the data frame looks as below: <br>

![Modified School Data Dataframe with NAN values](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/SchoolDataWithNANs.PNG) <br>  

-	Combination of School and student dataframe looks like below: <br>
![Combined  School and student dataframe](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/CombinationDfStudent%26School.PNG) <br>


### How is the district summary affected?   
-	At district level, there is slight change in the figures - around 1%. <br>
   Original Analysis: <br>
    ![originalDistrictSummary](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/originalDistrictSummary.PNG) <br>


    Adjusted Analysis: <br>
    ![ModifedDistrictSummary](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/ModifedDistrictSummary.PNG) <br>

1. At Thomas High School, 461 9th graders data for math and readinging values were assigned to NANs, but still the total no of student remained same as we did not delete the Student id.
2. Average math score has changed from 79 to 78.9.
3. % Passing Math has reduced from 75% to 74.8%.
4. % Passing Reading has reduced from 86% to 85.7%.
5. % Overall Passing has reduced from 65% to 64.9%.

<br>

### How is the school summary affected?   
In the original analysis, Thomas High School displayed 91% overall passing rate, which was a concern to the school board as being too high. Recalculating the total number of 10th - 12th grade students as the new denominator, the rest of the testing data was adjusted accordingly. <br>

- The % Passing Math column values have changed from 93.27% to 66.91% for Thomas High School.
- The % Passing Reading column values have changed from 97.31% to 69.66% for Thomas High School.
- Removing the 9th grade students from the data, impacted overall passing rate from 91% to 65%. <br>

Original Analysis: <br>
![Original Summary](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/OriginalSchoolSummary.PNG) <br>

                                                                                                                                                                       
 Adjusted Analysis: <br>
![Adjusted Summary](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/ModifiedSchoolSummary.PNG) <br>     
We can conclude that the school performance based on the new student count displays drastic drop in the performance of Thomas High School compared to original analysis.

<br>

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
After replacing the ninth graders’ math and reading scores, Thomas High School that ranked second in the school list initially, is now at the bottom three. Please refer the screen shots. <br>
Original Analysis: <br>
![Before Impact](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/BeforeImpact.PNG) <br>
Adjusted Analysis: <br>
![Post Impact](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/PostImpact.PNG) <br>

### How does replacing the ninth-grade scores affect the following:

- Math and reading scores by grade: Post adjustment of 9th grade data, Thomas High School's math and reading values are have been replaced with "NAN" values.  <br> <br>
Math grades: <br>
![Thomas High School's math](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/mathTHS.PNG) <br>  <br>
Reading Grades: <br>

![Thomas High School's Reading Grades](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/ReadingTHS.PNG) <br><br>



- Scores by school spending: Schools whose per student budget ranges between $631 -645 were affected and refering to the below image we can conclude
 1. % Passing Math reduced from 73% to 67%.
 2. % Passing Reading reduced from 84% to 77%.
 3. Overall Passing reduced from 63% to 56%.

![spending range](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/ModifiedRanges.PNG) <br>
    
<br>

- Scores by school size: There is very little impact by campus size due to changing the 9th grade scores.Only the scores for medium schools have been affected.
1.  %Passing Math reduced from 94% to 88%.
2.  % Passing reading reduced from 97% to 91% .
3.  % overall Passing reduced from 90% to 85%.
![School Size](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/scoresBySchoolSize.PNG) <br><br>


- Scores by school type
In school type, there is no change in the District level but only Charter level.
1. %Passing Math reduced from 94% to 90%.
2. % Passing reading reduced from 97% to 93%.
3. % overall Passing reduced from 90% to 87%. <br>

![School Type](https://github.com/ashwinihegde28/School_District_Analysis/blob/main/Resources/SchoolType.PNG) <br>
 


## Summary: Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

1. The overall passing rate for Thomas High School charter school, changed drastically from 91% to 65%. 

2. Thomas High School's ranking dropped from 2nd to bottom third place in performance after modification. 

3. Data at the grade level will now show as "NaN" in reports for the 9th grade students at Thomas High School  

4. Apart from overall passing rate, the math and reading averages and passing percentages were all affected.  

The major changes will be seen at the lower views of the disaggregated data with minor impact to the larger data views.





