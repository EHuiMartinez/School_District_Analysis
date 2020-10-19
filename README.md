# School_District_Analysis
Analysis of school district data

## Overview of the school district analysis:

The purpose of this analysis is to review a local school district data with school and student information.  There was a raised concern that one of the schools, Thomas High School's ninth grade data appears to have been altered.  Using these provided sets of data and performing analysis using Python3, Pandas, and Numpy via Jupiter notebook, information can be cleaned and replaced.  Following the request instructions, ninth grade reading and math scores were replaced with NaNs, updated school summary data frame and repeated the school district analysis to compare any affect to the overall analysis. All analysis codes are included in file: PyCitySchools-Challenge.ipynb

## Results:

- How is the district summary affected?  

Comparing the district summary after removing the Thomas High School's 9th grade scores and updated the school summary data frame, the information displayed for the district summary remained the same from prior comparison.

- How is the school summary affected?

    - Before manipulating the data, Thomas High School's scores for % Passing Math = 66.91%, % Passing Reading = 69.66% and % Overall Passing = 65.08%.  After removing the 9th grade data and converting to NaN, the scores for Thomas High School was recalculated using only the remaining grades 10 - 12 data.  The new calculated scores for Thomas High School's % Passing Math = 93.19%, % Passing Reading = 97.19% and % Overall Passing = 90.63%.  This is an overall increase when the 9th grade data was removed.

Thomas High School 9th grade scores convert to NaN:
![ThomasHS_9th_NaN.png](https://github.com/EHuiMartinez/School_District_Analysis/blob/main/Resources/ThomasHS_9th_NaN.png)


School Summary Before:
![School_summary_before_replace_ThomasHS.png](https://github.com/EHuiMartinez/School_District_Analysis/blob/main/Resources/School_summary_before_replace_ThomasHS.png)

School Summary After:
![School_summary_after_replace_ThomasHS.png](https://github.com/EHuiMartinez/School_District_Analysis/blob/main/Resources/School_summary_after_replace_ThomasHS.png)

- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

After updating the school summary with data only for 10th - 12th grades, Thomas High School remained as one of the top 5 high schools, as second place, same as prior performance comparison with other schools.  

![Top5_percent_overall_passing.png](https://github.com/EHuiMartinez/School_District_Analysis/blob/main/Resources/Top5_percent_overall_passing.png)

- How does replacing the ninth-grade scores affect the following:
    - Math and reading scores by grade
        - It does not affect grades 10 - 12; only 9th grade data was changed to NaN.

    - Scores by school spending
        - It does not show any affect from prior comparison.

    - Scores by school size
        - It does not show any affect from prior comparison.

    - Scores by school type
        - It does not show any affect from prior comparison.

## Summary:
Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

In this analysis, the school summary dataframe (per_school_summary_df) was updated with passing math, reading and overall percentage scores after removing 9th grade data.  Since the rest of the scores are based on the updated school summary dataframe data, it remained the same as prior comparison.  This analysis also showed that the Thomas High School 9th grade data can be manipulated and the school summary was updated with scores that ommited the 9th grade data. If the data included the 9th grade data, with an apparent lower % Passing Math, % Passing Reading and % Overall Passing scores for Thomas High School, the school may not remain in the top 5 school list.  It could also potentially bring down the percentage scores by school type for Charter schools.  School spending based on scores may also be affected.  
