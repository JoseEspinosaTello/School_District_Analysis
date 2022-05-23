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

		The math and reading scores were completely removed and replaced with a NaN (Not a Number) value.

	![avg_math_score](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/avg_math_score.png)

	![avg_reading_score](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/avg_reading_score.png)

		
	The removal of all the ninth-grade scores results in NaN listed for both categories under the ninth-grade students.
		
		
	- Scores by school spending

		Thomas Highs School has a budget of $638 per studnent and the scores were not affected for its spending range ($631 - $645).

	(Spending summary did not change)

	![spending_summary_df](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/spending_summary_df.png)

	
	- Scores by school size

		Thomas High School has a total 1635 student and sits in the Medium (1000 - 1999) range.

	(Size summary did not change)

	![size_summary_df](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/size_summary_df.png)

		
	- Scores by school type

		Thomas High School is a charter school and the changes did not affect the average scores of charter schools.

	(Type summary did not change)

	![Type_summary_df](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/Type_summary_df.png)

## Summary:

Overall the suspected academic dishonesty was insignificant towards the analysis results. However, even though the changes did not affect the finaly results, there were some noticable differences:

	- Reading scores now show NaN for Thomas High School ninth-graders
	- Math scores now show NaN for Thomas High School ninth-graders
	- Revised code for formating district_sumamry_df uses {:.1f} which rounds to the tenth decimal place while the old code uses {:.0f} which rounds to the nearest whole number.
	- Revised code per_school_summary_df will show incorrect values before any changes are made. If anyone wishes to further evaluate the altered code the must be aware of the changes that must be applied otherwise their analysis could be incorrect


	(per_school_summary_df immediatly after removing ninth-graders)
	![per_school_summary_df_wrong](https://github.com/JoseEspinosaTello/School_District_Analysis/blob/main/Resources/per_school_summary_df_wrong.png)


 The removal of all ninth-graders from Thomas High School did not cause major changes to the scores, percentages, or budegeting analysis. We have concluded that after removing the Thomas High School ninth-grade math and reading scores the same budgeting decisions can be made, as all scores remained mostly unchanged. This is the best possible outcome for the school board as the academic dishonesty failed to do what it was intended for; altering the average school scores and favorably influencing the budgeting decisions.
