# School_District_Analysis
1. Overview of the school district analysis:
The purpose of this analysis is to examine the relationships between test scores and a variety of metrics such as spending per student, school size, and school type. These analyses were primarily performed on the school level, with data aggregated from test scores across the district. This analysis also set out to determine metrics such as the average scores in math and reading, as well as the rates of passing in math and reading and overall. These were compiled at the school aggregation level, and the schools were ranked according to their overall rates of passing.
Critically, the test scores from the 9th grade class at Thomas High School have come under suspicion, necessitating their removal from the testing dataset and a subsequent reanalysis of the data. This was performed on the same metrics as above.  

2. There is a bulleted list that addresses how each of the seven school district metrics was affected by the changes in the data (10 pt).
Before:
<img width="1136" alt="District_summary_before" src="https://user-images.githubusercontent.com/90073490/137670106-5e1751d3-9686-4369-ab34-9e57ba352f88.png">
After:![District summary after](https://user-images.githubusercontent.com/90073490/137670163-fc02d68e-7e16-44d4-a6bd-054cdc4b4f60.png)
•	How is the district summary affected?
o	The total students and total budget metrics remains unchanged. Although there are potentially fraudulent scores, their removal and replacement with NaN does not affect the size of the overall student population nor the total district budget. 
o	After removal of the scores from the 9th graders from Thomas High School, the average math score drops slightly, while the average reading score remains unchanged to the first decimal place. The average scores of the removed data appears to be higher on average that the district scores, so their removal has led to a decrease in the average scores.
o	The percentages of passing students decreases across the board with the removal of the potentially fraudulent scores. This is due to a higher proportion of passing scores among the removed scores than those within the district population. One interesting note is that the amount that the rates of passing scores decreased is greater than the amount that the average scores decreased. This suggests a higher variance within the potentially fraudulent scores than within the district as a whole.
•	How is the school summary affected?
o	Before:
<img width="1114" alt="Summary_before" src="https://user-images.githubusercontent.com/90073490/137670206-341f377e-96ee-4b3b-a6c9-90cf70f69578.png">
After:
<img width="1125" alt="Summary_after" src="https://user-images.githubusercontent.com/90073490/137670226-2ae4c09c-af71-4bce-8111-1125e274ff24.png">
o	Removal of the scores did not alter the results for other schools, although it did lead to a drop in Thomas High School’s average scores and rates of passage, with the exception of the average reading score. 
o	The sole exception here was THS’ average reading scores, which increased slightly after removal of the 9th graders’ scores. This suggests that the scores removed were lower than the school’s average, but that the rate of passing scores is higher than the schools’ average. These two phenomena lead to the conclusion that there is relatively high degree of variance within the potentially fraudulent scores.
How does replacing the ninth-grade scores affect the following:
•	Math and reading scores by grade
o	Math scores:
	Before:
<img width="513" alt="math_scores_by_grade_before" src="https://user-images.githubusercontent.com/90073490/137670364-7bfa651a-5ccd-4bd9-b3c7-7be5fa6843c7.png">
	After:
<img width="434" alt="math_scores_by_grade_after" src="https://user-images.githubusercontent.com/90073490/137670389-ee096715-833a-4ba8-b727-9b647e6f5ead.png">
o	Reading scores:
	Before:
<img width="464" alt="reading_scores_by_grade_before" src="https://user-images.githubusercontent.com/90073490/137670422-c2694b14-526c-4529-9bdb-ecf18b5bf46c.png">
	After:<img width="471" alt="reading_scores_by_grade_after" src="https://user-images.githubusercontent.com/90073490/137670435-5d77c97a-826d-4eb4-8317-edb66da19043.png">
o	As can be seen from the above screenshots, the Thomas High School 9th grade scores are the only ones affected by their removal. The scores for each THS 9th grader were replaced with NaN without interfering with any other student scores.
•	Scores by school spending
o	Before: 
<img width="945" alt="Averages_by_spending_before" src="https://user-images.githubusercontent.com/90073490/137670523-913be1db-c0bf-4515-ba4e-beddab37dad8.png">
o	After: <img width="1020" alt="Averages_by_spending_after" src="https://user-images.githubusercontent.com/90073490/137670543-dff7a24e-476e-4fd9-84c5-67dc3b0d0c8b.png">
o	There is no change to the outcomes by spending ranges before or after the removals. However, this analysis only looks at the rates of passage out to the whole percentage, and scores out to the tenth of a percent. There is some variation at smaller intervals than those displayed here.
•	Scores by school size
o	Before: 
<img width="857" alt="Averages_by_school_size_before" src="https://user-images.githubusercontent.com/90073490/137670599-2671dd0c-4848-455b-bd44-d832e68f9f14.png">
o	After: <img width="919" alt="Averages_by_school_size_after" src="https://user-images.githubusercontent.com/90073490/137670613-191c7245-5b11-4631-abbf-d07905150545.png">
o	Similarly to the above, there is no variation in the overall averages within the decimal intervals. There is some variation at smaller intervals than those displayed here.
•	Scores by school type
o	Before: <img width="826" alt="Averages_by_type_before" src="https://user-images.githubusercontent.com/90073490/137670676-535cadb3-0c3c-42ba-a2cb-a04f7461bc01.png">
o	After: <img width="941" alt="Averages_by_type_after" src="https://user-images.githubusercontent.com/90073490/137670731-3b716335-62d4-45b1-b1d2-03ae9ebd0984.png">
o	In a similar fashion to the size and spending metrics, type appears to be unaffected by the removals at the designated intervals.
3. Summary: There is a statement summarizing four changes to the school district analysis after reading and math scores have been replaced (5 pt)
o	After the scores were removed, the overall score breakdowns by size, spending, and type of school corresponding to Thomas High School’s respective categories fell slightly. The medium size, 630-644$ per student, and charter school category breakdowns’ scores fell slightly but remained inside the decimal interval used in the analysis.
o	Overall and subject-specific rates of passage at the district level fell by .2, .1, and .3 percent, respectively. The average reading score remained unchanged within the decimal interval, while the average math score dropped by .1%.
o	The schools’ rankings across the district remain unchanged, although the overall rate of passage for students in THS dropped.
o	The greater drop in passage rates than the corresponding drop in average scores after the removal of the potentially fraudulent scores suggests a higher degree of variance within that data than within the district data as a whole. 
