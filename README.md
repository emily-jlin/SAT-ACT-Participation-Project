# Statistical Analysis on the 2017-2018 SAT and ACT participation data to recommend appropriate strategies to expand SAT participation rate in the United States.


## Problem Statement
To increase SAT participation rate in the United States by examining competitor's participation rate and education policies that influence the business of College Board.

## Executive Summary

### Organization Overview

College Board is a national education nonprofit that aims to expand college accessibility to all students in the United States. Its core products are Advanced Placement tests, SAT, and the PSAT. Currently, there are 16 states and the District of Columbia have contracts with College Board to administer state-funded SAT to all high school students (College Raptor). The College Board's competitor, ACT, offer free tests to all juniors in 16 states (College Raptor).

### Market Analysis

According to the Washington Post in 2018, the SAT has regained its position as the most popular test among high school graduates. This is attributable to the multi-year contracts that the College Board has secured in states like Colorado and Illinois where the participation percentage spiked 89% and 90% respectively. To ensure that College Board is expanding students' access to higher education, College Board needs to increase participation rate in 50 states. This analysis examines the participation percentage of SAT and ACT in 2017 and 2018 to find where College Board can capture the opportunity to increase its presence. In addition, it will look at the success stories of states like Illinois and Colorado to replicate the efforts in states where it is appropriate.


### Contents:

- [2017 Data Import & Cleaning](#Data-Import-and-Cleaning)
- [2018 Data Import and Cleaning](#2018-Data-Import-and-Cleaning)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Data Visualization](#Visualize-the-data)
- [Descriptive and Inferential Statistics](#Descriptive-and-Inferential-Statistics)
- [Outside Research](#Outside-Research)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

Provided below is the data dictionary used to help navigate data analysis process.

### Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|SAT/ACT|50 states plus D.C. indicator that is spelled out, ie California.|
|2017 act participation %|float|ACT|The participation percentage in every state in 2017.|
|2018 act participation %|float|ACT|The participation percentage in every state in 2018.|
|english|float|ACT|The average english score of all participants in the state. Ranges from 1 to 36.|
|2017 act math|float|ACT|The average math score of all participants in the state. The ACT score ranges from 1 to 36. |
|reading|float|ACT|The average reading score of all participants in the state. Ranges from 1 to 36.|
|science|float|ACT|The average science score of all participants in the state. Ranges from 1 to 36.|
|2017 composite|float|ACT|The average composite score of all participants in the state in 2017. Ranges from 1 to 36.|
|2018 composite|float|ACT|The average composite score of all participants in the state in 2018. Ranges from 1 to 36.|
|2017 sat participation %|float|SAT|The participation percentage in every state.|
|2017 reading and writing|float|SAT|The average evidence-based reading and writing score of all participants in the state. Ranges from 200 to 800.|
|2017 sat math|float|SAT|The average math score of all participants in the state. The SAT score ranges from 200 to 800.|
|2017 total|float|SAT|The average total score of all participants in the state. Ranges from 400 to 1600.|
|2018 sat participation %|float|SAT|The participation percentage in every state.|
|2018 reading and writing|float|SAT|The average evidence-based reading and writing score of all participants in the state. Ranges from 200 to 800.|
|2018 sat math|float|SAT|The average math score of all participants in the state. The SAT score ranges from 200 to 800.|
|2018 total|float|SAT|The average total score of all participants in the state. Ranges from 400 to 1600.|




## Research

The three states that are beneficial to the analysis are California, West Virginia, and Ohio. Despite having a pretty decent percentage in SAT participation,  education policies in California are decided locally instead of statewide. While most states use the ACT or SAT to satisfy the federal requirement of administering summative test for all high school students, California's school districts can decide whether to administer ACT or SAT (1). The SAT participation in California increased from 53% to 60% while the ACT participation rate decreased from 31% to 27%. Unlike California, Illinois's drastic increase from 9% in 2017 to 99% in 2018 is due to the College Board securing a multi-year contract with the Illinois Department of Education (2). Since California has a decentralized education department, it is important to target individual school districts rather than spending money on lobbying the department of education at the state level.

Like California, Ohio does not have a contract with either testing services. The SAT participation rate of Ohio increased from 12% to 18% while the ACT participation increased from 75% to 100%. It is requiring schools to administer the ACT or the SAT (3). This gives College Board the opportunity to expand testing service by offering free testing materials. For example, if a student is taking an AP class and is expecting to take AP exam, College Board could offer more free test prep for those students. In general, expanding the testing base will be key to College Board. Students may be more likely to take a test with their friends so they are heavily influenced by peers. This cannot be inferred from the analysis with so few data, but it will be beneficial to the business development team if College Board can collect data on student behavior and how peers affect students' test choice. If College Board can offer test vouchers to after school programs that encourage students to sign up for the same testing date. This may help College Board to boost participation rate.

West Virginia is the third state of interest because the SAT participation, while low, is on the rise. The SAT participation rate increased from 14% to 28% while the ACT participation decreased from 69% to 65%. In 2018, West Virginia's state began to administer SAT tests to all high school students and this is the only test that will be recognized as admission require to the Promise program (4).

Sources:
1. Fensterward, John. “Growing number of California school districts offer students free college entrance exam”. https://edsource.org/2017/more-evidence-supports-school-districts-that-offer-free-satact-to-all-students/585696
2. Chen, Elaine. “Illinois has embraced the SAT, and the ACT is mad about it”. https://chalkbeat.org/posts/chicago/2018/07/27/act-protests-state-boards-embrace-of-rival-test-provider/
Ohio Department of Education, http://education.ohio.gov/Topics/Testing/State-Funded-SAT-Test
3. Quin, Ryan. “WV chooses SAT as new high school standardized test for juniors”. https://www.wvgazettemail.com/news/education/wv-chooses-sat-as-new-high-school-standardized-test-for/article_b60d2618-4943-56f6-b180-4b4442172ef8.html

## Recommendation and Conclusion

Since Ohio's state department does not endorse the ACT over the SAT, College Board may not be able to employ the same strategy in Illinois and Colorado where the the state signed a multi-year contract. However, there are creative ways to help College Board improve participation rate outside of lobbying.

College's other two core products: PSAT and AP are a great venue for the organization to gain insight on student behavior. While it cannot be confirmed in this data, students may choose to take tests that they are better prepared for because this leads to higher scores that are crucial to college admission. College Board should work towards administering state-funded PSAT to all 9th and 10th graders because the PSAT gives students a preview of the SAT. Next, the data team at College Board will be able to conduct A/B testing to see if students' participation in PSAT affect SAT.

To increase the participation rate of students in Ohio, College Board should consider giving students who are already taking AP class free test preps for the SAT. Students who are taking the SAT are already familiar with College Board so they might be more likely to take the SAT. Since Of course, this will require College Board to gather data on the percentage of students who take the SAT given that they are taking AP courses.

College Board can also provide free test vouchers to school districts that have lower participation rate. Free tests encourage students to try the test and their testimony may influence how their peers choose ACT or SAT.

### Additional Data
Some data that  would be beneficial in the analysis are:
1. The percentage of students who take AP participated in SAT.
2. The percentage of students who participated in PSAT took the SAT.
3. Students' major of interest in college .
4. Students' used test preps or not.  

There are a couple of conditional probabilities that would be interesting to look at if College Board can survey students from all the states:
1. The probability that a student will take the SAT given that the student took the ACT
2. The probability that a student will take the SAT given that the student took the PSAT
3. The probability the student will take the ACT given that student took the PSAT.
