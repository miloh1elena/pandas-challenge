# School District Analysis

This project involves analyzing school district data using Python and the Pandas library. The code performs various calculations and data manipulations to generate key metrics and summaries related to schools, students, grades, and other relevant factors.

## Getting Started

Using the following data files:

- `schools_complete.csv`: Contains information about the schools in the district.
- `students_complete.csv`: Contains information about the students in the district.

Necessary dependencies installed: Pandas and pathlib.

## Data Loading and Merging

The code begins by loading the school and student data from the respective CSV files using Pandas. The `pd.read_csv()` function is used to read the CSV files into Pandas DataFrames. The data is stored in the `school_data` and `student_data` variables.

The school and student data are then merged into a single DataFrame called `school_data_complete`. The `pd.merge()` function is used to merge the data based on the "school_name" column.

## District Summary

The code calculates several key metrics for the entire district:

- Total number of unique schools
- Total number of students
- Total budget
- Average math score
- Average reading score
- Percentage of students passing math
- Percentage of students passing reading
- Overall passing rate (percentage of students passing both math and reading)

These calculations are performed using Pandas operations on the `school_data` and `student_data` DataFrames.

## Analysis Report

### Summary:
The analysis of district-wide standardized test results reveals significant variations in school performance. The district comprises 15 schools, with student counts ranging from 427 to 4976. The budget per school varies, with the highest at $3 124 928 and the lowest at $248 087. The per-student budget also exhibits diversity, ranging from $578 to $655.

### Conclusions and Comparisons:

#### Budget Allocation and Performance:

Higher budget schools do not necessarily guarantee better academic performance. For instance, Bailey High School, with the highest budget of $3,124,928, has a relatively low overall passing rate of 54.6%. On the contrary, Cabrera High School, with a lower budget of $1,081,356, boasts a remarkable overall passing rate of 91.3%. This suggests that factors beyond financial resources contribute to academic success.

#### Charter vs. District Schools:

Charter schools consistently outperform district schools. The top five schools with the highest overall passing rates are charter schools, while the bottom five are district schools. Cabrera High School, a charter school, leads with a 91.3% overall passing rate, whereas Bailey High School, a district school, trails with 54.6%. This indicates a potential need for further investigation into the practices and strategies employed by charter schools.

In conclusion, the analysis highlights the need for a nuanced approach to budget allocation and a closer examination of the practices employed by charter schools for potential implementation in district schools. These insights will be crucial for the school board and mayor in making informed decisions regarding future school budgets and priorities.
