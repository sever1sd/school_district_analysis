# school_district_analysis

## Overview of the District Analysis

The purpose of this analysis was to clean, aggregate, and analyze data of student scores from various schools. The aggregated data of student scores will provide valuable insights in the general efficacy of school performance as well as indentify trends at the district and individual school levels. The results of this analysis will be used to inform financial and strategic decisions regarding school funding.

It was identified that academic dishonesty was detected at Thomas High School at the 9th grade level. This analysis removed the math and reading scores from the 9th grade data and reevaluated the results. 

## Results

### The Analysis

Jupyter Notebook and the programming language Python was used to conduct this analysis. Throughout this analysis, the Pandas dependency was used to assist in cleaning, aggregating, and analyzing this data.

In an effort to maintain academic integrity, 461 math and reading scores were made "null" for 9th graders at Thomas High School. The results were then recalculated to provide the most accurate data for decision making. Side by side comparisons of each are provided in the below analysis. No other data was altered other than the 461 test scores.

### How is the district summary affected?

Original District Summary
![alt text](https://github.com/sever1sd/school_district_analysis/blob/ab5c1c29483ff655b7c1d34223be346ec1b08dff/Resources/Original%20District.png)

Updated District Summary
![alt text](https://github.com/sever1sd/school_district_analysis/blob/ab5c1c29483ff655b7c1d34223be346ec1b08dff/Resources/Updated%20District.png)

The district summary data did not change much with the removal of the 9th grade test scores. This is due to the fact that the total population of the 9th graders at Thomas High (N = 461) was ~1% of the total population in the dataset (N = 39,170). 

### How is the school summary affected?

Original Thomas High School Summary
![alt text](https://github.com/sever1sd/school_district_analysis/blob/ab5c1c29483ff655b7c1d34223be346ec1b08dff/Resources/Original_THS%20Summary.png)

Updated Thomas High School Summary
![alt text](https://github.com/sever1sd/school_district_analysis/blob/ab5c1c29483ff655b7c1d34223be346ec1b08dff/Resources/Updated_THS%20Summary.png)

The high school summary changed dramatically with the removal of 9th grade test scores. The passing math scores dropped from ~93% to ~67% and passing reading scores dropped from ~97% to ~70%. This dramatic change is a result of the passing total calculating off the total population of students in the school. The 461 9th graders are still being accounted for in the total school population, despite their test scores having been removed.

### How does replacing the 9th graders' math and reading scores affect Thomas High School's performance relative to other schools?

In order to better reflect the performance of students in both math and reading at Thomas High School, their percentage passing was recalculated to exclude the 461 9th graders with null values. This resulted in Thomas High Schools' passing scores for reading and math only changing marginally and thus they kept their position as the second highest overall passing rate among the 15 schools evaluated.

Original Top 5
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Original_Top%205.png)

Updated Top 5
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Updated_Top%205.png)


### How does replacing the 9th grade scores affect:

**Math and Reading Scores by Grade

The math and reading scores were largely unaffected by removing the 9th grade scores for Thomas High School, with the noteable exception that Thomas High Schools 9th grade scores were replaced with "nan." This nulls out the scores for that grade and removes their data from teh analysis.

Original Math
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Original%20Math.png)

Original Reading
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Original%20Reading.png)

Updated Math
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Updated%20Math.png)

Updated Reading
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Updated%20Reading.png)

**Scores by School Spending

The scores dileneated by spending were largely unaffected by the removal of the 461 9th graders. The changes were minimal and were impactful after rounding.

Original Spending
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Original%20Spending.png)

Updated Spending
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Updated%20Spending.png)

**Scores by School Size

The scores dileneated by school size were largely unaffected by the removal of the 461 9th graders. The changes were minimal and were impactful after rounding.

Original Size
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Original%20Size.png)

Updated Size
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Updated%20Size.png)


**Scores by School Type

The scores dileneated by school type were largely unaffected by the removal of the 461 9th graders. The changes were minimal and were impactful after rounding.

Original Type
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Original%20Type.png)

Updated Stype
![alt text](https://github.com/sever1sd/school_district_analysis/blob/40a2248f8412abf8b783121cb84fd80ad5df56fd/Resources/Updated%20Type.png)

## Summary

The removal of the 9th grades scores at Thomas High School impacted the analysis in the following ways:

1. The district scores and passing rates when down nominally
2. Thomas High School's all-in summary dropped dramatically when accounting for the total population
3. 9th grade scores at Thomas High School were made null and show as "nan" in the summary data
4. Even when accounting for the 9th grade population of 461 student, reading and math scores for Thomas High School shifted downward, albiet marginally


Additionally, all other metrics would see shifts minimally but when rounded, they will report no changes. Ultimately, outside of Thomas High School's individual summary data, the removal of its 9th grade data has minimal impact to the end result of this analysis. Further, when accounting for the change in population with the removal of the 9th graders, Thomas High School's metrics also experience minimal change. 
