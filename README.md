# School_District_Analysis
## Overview 
After complete a complete analysis of the school district and return valuable budgeting projections, Maria and her supervisor were informed of academic dishonesty at Thomas High School. The school board wants to up-hold the testing standards of the district and would like Maria to remove the math and reading scores for grade 9 at Thomas High School. The scores are to be replaced with NaN and the analysis must be refactored in order to assist the school board make a new budgeting decision based on the updated analysis.

## Results:

- How is the district summary affected?

	The district summary showed the score we not truly affected by the removal of the 9th grade scores
	
	(Original District Summary Dataframe)
	![district_summary_df](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/district_summary_df.png)
	
	(Updated District Summary Dataframe)
	![district_summary_df_New](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/district_summary_df_new.png)

	The code for the new scores used a different formatting for the decimal point which created different results. If rounded up the changes are insignificant:
		- Average Math Score: 79 > 78.9
		- Average Reading Score: 81.9 > 81.9
		- % Passing Math: 75 > 74.8
		- % Passing Reading: 86 > 85.7
		- % Overall Passing: 65 > 64.9

- How is the school summary affected?

The School Summary Dataframe did not see any major changes after the update.

	(Original School Summary Dataframe)
	![per_school_summary_df](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/per_school_summary_df.png)

	(Updated School Summary Dataframe)
	![per_school_summary_df_new](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/per_school_summary_df_new.png)

	Overall, the scores and passing percentages dropped slightly by tenths of a decimal point, however the changes are not enough to affect any major decisions.


- How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

	Thomas High School did not see any changes compared to other school.

	(Original top 5 schools)
	![top_five](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/top_five.png)

	(Updated top 5 schools)

	![top_five_new](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/top_five_new.png)

Thomas Highs School sat at number two during the original analysis based on “% Overall Score”. Since the “% Overall Score”, or any scores did not experience much change, the school position remained the same.

	- How does replacing the ninth-grade scores affect the following:
		- Math and reading scores by grade
		- Scores by school spending
		- Scores by school size
		- Scores by school type
