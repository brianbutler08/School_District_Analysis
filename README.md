# School_District_Analysis

# Overview

For this project, we were approached by Maria, a data analyst for a large school district. One of her responsibilities is to work with all standardized test data, preparing it for analysis, reporting and presentation purposes. She was looking for assistance to specificically look at school funding and student standardized test scores. We were granted to access to the district dataset and proceded to aggregate the applicable data in order to showcase trends in school performance. Our analysis was intended to assist the superintendent and school board to make informed decisions around school funding and priorities setting.

However, once the project was effectively completed, we were approached by Maria to make some adjustments to our analysis. There was evidence to suggest that the reading and math scores for the 9th grade students at Thomas High School had been unethically altered and they needed to be removed from our analysis. We therefore replaced the impacted scores with null values and re-ran all of our analyses without those values. 

There were two datasets that we utilized during this analysis and they were combined into a single set for ease of aggregation. The fields contained in the final database included:

- Student ID
- Student name
- Student gender
- Student grade
- School name
- Standardized math score
- Standardized reading score
- School ID
- School type
- School size (number of students)
- School budget

# Results

By replacing the standardized test scores of ninth grade students at Thomas High School with a null value, we anticipated that there may be some changes in the overall outcomes realted to the analysis. In order to attempt to quantify these changes, we wanted to directly compare our original DataFrames with the DataFrames that were produced after the removal of the suspicious scores. 

## District Summary

- Original District Summary

![](https://github.com/brianbutler08/School_District_Analysis/blob/main/Resources/Images%20for%20report/district_summary_original.png)

- Edited District Summary

![](https://github.com/brianbutler08/School_District_Analysis/blob/main/Resources/Images%20for%20report/district_summary_edited.png) 

Once the ninth grade Thomas scores were removed from the dataset, there was little change to the district summary. The proportion of students passing math and reading (as well as overall passing rates) decreased slightly. This is primarily due to the large size of the dataset (39,170 students). Removing a few hundred data points is not going to have that much of an effect on the overall outcomes.

## School Summary

-Original School Summary

![](https://github.com/brianbutler08/School_District_Analysis/blob/main/Resources/Images%20for%20report/school_summary_original.png) 

- Edited School Summary

![](https://github.com/brianbutler08/School_District_Analysis/blob/main/Resources/Images%20for%20report/school_summary_edited.png)

Removing a class of test scores obviously won't effect the school level reports of other schools, but it greatly affected the percentage of students that passed the standardized tests at Thomas. The proportion that passed math decreased 25%, reading passing rates decreased by 27% and the overall passing percentage decreased by 26%. When an adjustment was made and the scores for the 10th, 11th, and 12th graders were ananlyzed appropriately, the passing proportions returned to close to "normal".

## Math Scores By Grade

- Original Math Scores

![](https://github.com/brianbutler08/School_District_Analysis/blob/main/Resources/Images%20for%20report/math_scores_by_grade_original.png)

- Edited Math Scores

![](https://github.com/brianbutler08/School_District_Analysis/blob/main/Resources/Images%20for%20report/math_scores_by_grade_edited.png)


## Reading Scores By Grade

- Original Reading Scores

![](https://github.com/brianbutler08/School_District_Analysis/blob/main/Resources/Images%20for%20report/reading_scores_by_grade_original.png)

- Edited Reading Scores

![](https://github.com/brianbutler08/School_District_Analysis/blob/main/Resources/Images%20for%20report/reading_scores_by_grade_edited.png)

Again, no other schools were affected by our re-running of the data (which is important to display, no matter how obvious).

## Scores By School Spending, School Size and School Type

By the time we ran the data again for school spending, size and type, we had adjusted the overall scores for Thomas High School and added our new data based on the scores from the students in 10th, 11th, and 12th grade. As a result, there was little difference in the outcomes of our new dataset when compared to the orginal one. Again, when grouped with several other high schools, and thousands of other students, it is harder to discern any changes to the group when alterations have been made on a few hundred students.

The most noticable change was in the spending group which included Thomas High School ($630 - $644). After the adjustment was made, there was approximately a three percent increase in the proportion of students that passed math, reading and overall testing. 

- Edited School Spending

![](https://github.com/brianbutler08/School_District_Analysis/blob/main/Resources/Images%20for%20report/school_spending_edited.png)

- Edited School Size

![](https://github.com/brianbutler08/School_District_Analysis/blob/main/Resources/Images%20for%20report/school_size_edited.png)

- Edited School Type

![](https://github.com/brianbutler08/School_District_Analysis/blob/main/Resources/Images%20for%20report/school_typer_edited.png)

# Summary
