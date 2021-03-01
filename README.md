# School_District_Analysis

## Project Overview
The school board has notified us that the file containg all the grades for the differents schools (students_complete.csv) appears to have been corrupted.
Specifically, the reading and math grades for Thomas High School ninth graders appeared to have been changed.
To fix the results, the school board has asked us to:

-Replace all the reading and math scores for the 9th grade students in Thomas High School with "NaN".
-Repeat the school district analysis and recreate the following metrics:
  -The district summary
  -The school summary
  -The top 5 and bottom 5 performing schools, based on the overall passing rate
  -The average math score for each grade level from each school
  -The avearage reading score for each grade level from each school
  -The scores by school spending per student, by school size, and by school type.

## Resources
Data Sources: students.complete.csv, schools.complete.csv
Software: Python 3.7.6, Visual Studio Code 1.53.2

## Summary

The re-analysis of the grades from all the different schools show that
-  !![image](![image] 



## Election Audit Summary

We succeded in conducting the audit and provided all the metrics requested by writting a generalized script that could easily be adapted to audit any another election.

This could be done by first altering the name of the file containing the ballot results (e.g. "election_results.csv") in the following line of code: 
`file_to_load = os.path.join("Resources", "election_results.csv")`. 

Secondly the code could be adapted to analyze election results from files that contained the "county" and the "candidate name" on different columns than those observed in this file: column #1 for county, column#2 for candidate name.  This could be done by changing the numbers in the square brackets to match the column number where the candidate name and county names are found the following lines of code:

` # Get the candidate name from each row.`
  `candidate_name = row[2]`

  `# 3: Extract the county name from each row.`
  `county_name = row[1]`
