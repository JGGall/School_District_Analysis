# School District Analysis

## Overview of the School District Analysis

### This analysis was always meant to allow the school board and other stakeholders to see tables of data that would allow them to make comparisons among the schools based on school performance, school size, spending per student, and type of school (district school or charter school). The analysis had to be adjusted after the math and reading scores of all of the ninth-graders at a medium-sized high school were set aside due to academic dishonesty. It became a special point of interest to see how this adjustment impacted the overall analysis.


## Results
### How is the district summary affected?
- Because the academic dishonesty among Thomas High School ninth graders required the exclusion of only 461 students' math and reading scores in a district of 39,170 students, the change in the district summary was a very small one. The average math score dropped from 79.0 to 78.9. The average reading score remained unchanged. The percentage passing math and reading dropped by  0.2% and and 0.3% respectively. The overall passing percentage dropped by 0.1%.
### How is the school summary affected?
- In the DataFrame "per_school_summmary_df," the changes brought on by excluding the scores of Thomas High School ninth graders are more evident, but they still do not make a large impact. Of course, among the 15 schools the only school affected at all is Thomas High School itself. The two average scores (math and reading) dropped slightly, but when the scores are rounded the difference practically disappears. The percentage passing in math, reading, and overall dropped by about 0.1%, 0.2%, and 0.3% respectively.
![Code_Image_select_math]
![Code_Image_select_reading]


### How does replacing the ninth-grade scores affect the following:
- Math and reading scores by grade
    - Replacing the math and readings scores of Thomas High School ninth graders with NaNs had no impact on any other school's data, nor on the data of the other three grades at Thomas. But before the replacement, the ninth graders at Thomas had better average math scores than any other grade, and better reading scores than one other grade. But if the dishonesty had not been caught, the ninth graders' scores at Thomas would not have been remarkably different than the scores of the students in the other grades at Thomas High School.

- Scores by school spending
    - When we consider the spending summary DataFrame, in which the schools are separated into four spending "bins" based on spending per student, the category in which Thomas High School falls ($630-$644) had an overall passing percentage drop--but the drop was only a tenth of a percentage point, from 62.9% to 62.8%. This is not large, and will probably not have a significant impact on school planning for the next budget year.

- Scores by school size
    - There are three ranges of school size in the size summary DataFrame. Thomas High School falls in the "medium" range, and after the ninth graders' scores were excluded, the impact was so insignificant that there was no apparent difference once the scores were rounded to the tenths place and the percentages were rounded to the nearest whole percentage point.

- Scores by school type
    - Something similar can be stated about the DataFrame in which the schools were sorted into two categories: district or charter. Thomas High School is a charter school, and after the ninth graders' scores were excluded, the imact was only a slight one. After the figures were rounded, there was no apparent difference.


## Summary
### The most important change in the School District Analysis after the Thomas High School ninth graders' scores were excluded is the simple fact that the math and reading scores for those students are missing and will never be restored. As they move through the grades of their high school in future years it will be impossible to measure the progress of that cohort. A second change is that is also impossible to compare the scores of the current ninth graders at that school with the scores of students in the other grades. A third change is that the scores of ninth graders at THS can no longer be compared to the scores of ninth graders at other schools in the district. 
![DF_Image_Top_after_adjustment]
![DF_Image_Top_after_adjustment]
A fourth change is that Thomas High School, which is the second-highest-performing school based on overall percentage of student passing in math and reading, experienced a drop in that key indicator: its overall percentage dropped from 90.948012% to 90.630324%. This very nearly led to Thomas dropping in rank from #2 to #3 in the district. That percentage drop highlights the fact that is is now impossible to know whether the original percentage was accurate, or whether it was based on math and reading scores that had been altered rather than earned.
