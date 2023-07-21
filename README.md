School District Analysis
This project involves analyzing school district data using Python and the Pandas library. The code performs various calculations and data manipulations to generate key metrics and summaries related to schools, students, grades, and other relevant factors.

Getting Started
To get started with the project, you'll need the following data files:

schools_complete.csv: Contains information about the schools in the district.
students_complete.csv: Contains information about the students in the district.
Make sure you have the necessary dependencies installed, including Pandas and pathlib.

Data Loading and Merging
The code begins by loading the school and student data from the respective CSV files using Pandas. The pd.read_csv() function is used to read the CSV files into Pandas DataFrames. The data is stored in the school_data and student_data variables.

The school and student data are then merged into a single DataFrame called school_data_complete. The pd.merge() function is used to merge the data based on the "school_name" column.

District Summary
The code calculates several key metrics for the entire district:

Total number of unique schools
Total number of students
Total budget
Average math score
Average reading score
Percentage of students passing math
Percentage of students passing reading
Overall passing rate (percentage of students passing both math and reading)
These calculations are performed using Pandas operations on the school_data and student_data DataFrames.

School Summary
The code also generates a summary of key metrics for each school:

Total student count per school
Total school budget
Per capita spending per school
Average math score per school
Average reading score per school
Percentage of students passing math per school
Percentage of students passing reading per school
Overall passing rate per school
These calculations are performed using Pandas operations on the school_data DataFrame.

Top and Bottom Performing Schools
The code identifies the top and bottom performing schools based on the "% Overall Passing" metric. It sorts the schools by this metric in descending and ascending order, respectively, and displays the top 5 rows for each.

Math and Reading Scores by Grade
The code separates the student data by grade level (9th, 10th, 11th, and 12th) and calculates the average math and reading scores for each grade level and school. The results are stored in DataFrames named math_scores_by_grade and reading_scores_by_grade respectively. These DataFrames are then displayed.

Scores by Spending
The code categorizes the schools into spending ranges per student based on the budget per student. It uses the pd.cut() function to create bins and labels for the spending ranges. It then calculates the average math and reading scores, as well as the percentage of students passing math, passing reading, and overall passing rate, for each spending range. The results are stored in a DataFrame named spending_summary and displayed.

Scores by School Size
The code categorizes the schools into size ranges based on the total student count. It uses the pd.cut() function to create bins and labels for the size ranges. It then calculates the average math and reading scores, as well as the percentage of students passing math, passing reading, and overall passing rate, for each size range. The results are stored in a DataFrame named size_summary and displayed.

Scores by School Type
The code groups the schools by school type (e.g., District or Charter) and calculates the average math and reading scores, as well as the percentage of students passing math, passing reading, and overall passing rate, for each school type. The results are stored in a DataFrame named type_summary and displayed.
