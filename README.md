# School_District_Analysis

The School District Analysis has been a very challenging, at times exahusting and demanding task that has grown intensively from a quantitative description to be a qualitative analysis with some curveballs thrown along the way. The requested data description of the schools' results based on the passing scores and the grade of the students presented was sorted by school, by grade, student total and more importantly by budget.

The suspected scores reported academic dishonesty altered the approach of the analysis and we had to consider a different approach towards Thomas High School specifically, having to modify the math scores results and replace them with NaN by using the following code:

student_data_df.loc[(student_data_df["grade"]== "9th") & (student_data_df["school_name"]=="Thomas High School") , "reading_score"] = np.nan


~How is the district summary affected?
The summary district describes a group of high schools district and charter that present a variety of results, considering the size of the affected school not being one of the top performers, the district summary remains somewhat unaffected

~How is the school summary affected?
Excluding the affected Thomas High School, whose values are NaN, the remaining schools stay unaffected, nor their budget or ranking position varied.

~How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
The performance relative to other schools was barely affected in the analysis

