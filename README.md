# SAT & ACT Data: Analyzing participation rates and test scores from 2017-2018


## Problem Statement

The new format for the SAT was released in March 2016. As an employee of the College Board - the organization that administers the SAT - I'm part of a team that tracks statewide participation and recommends where money is best spent to improve SAT participation rates. With two years of data (2017 & 2018) available since we have implemented this new format, we would like to evaluate our progress so far and determine what step are necessary to increase participation across the United States.


## Executive Summary
**INTRODUCTION**

More than 2.1 million students in the class of 2018 took the redesigned SAT, an increase of 25% over the class of 2017, according to the 2018 SAT Suite of Assessments Program Results. This marks the highest SAT participation College Board has seen.

However, it is observed that ACT i sstill prominent in many states. There are 12 states that require every junior to take the ACT test and eight more that either require the test in some districts or offer it as a free option for students who wish to take it. This makes it difficult for SAT participation status to improve in these states.
 

To conduct an analysis on the SAT, datasets from both the SAT and ACT were used. Each dataset contains state-by-state average test scores and participation rates, specifically from 2017 and 2018. Analyzing test scores and participation rates between the SAT and ACT allowed for a point of comparison to measure the SAT against. 


**METHODOLOGY**

Firstly, the **problem statement** was identified that the College Board needed to determine how to increase SAT participation rates. Next, **data import** was performed by locating credible sources and each RELEVANT individual dataset was imported. Next, **data cleaning** was conducted to ensure that all datatypes were accurate and any other errors were fixed. Using all data of SAT and ACT for both 2017-2018, an **exploratory data analysis** was conducted to determine any parameters about the population being measured. All statistical findings were used to then perform **data visualization**. Once all data was visualized, **descriptive and inferential statistical analysis** was conducted to describe what the distributions were and any trends appeared in the data.  To confirm and support the observations made, **outside research** about the SAT and any other relevant data was conducted. Finally, **data-driven conclusions and recommendations** for the College Board were compiled. 

**SIGNIFICANT FINDINGS**

When analyzing the datasets, many findings about SAT and ACT test scores and participation rates were gathered. Here are the most significant findings, focusing primarily on the SAT: 

- Participation Rates: States with high SAT participation rates tend to have low ACT participation rates and vice versa
- Participation Rates: Higher participation rates in coastal region states as compared to the mid region states
- Participation Rates vs Test Scores, 2017-2018: In both years, there was a strong negative correlation between test scores and participation rates. The higher the participation rate, the lower the test score.
- SAT Total Scores, 2017-2018: The distribution of average test scores from all states was bimodal. Students either performed very poorly or very well.

---
## Data Dictionary
|Feature|Type|Dataset|Description|
|---|---|---|---|
|state|object|ACT/SAT|State name for associated SAT/ACT average scores and participation rates| 
|act_participation|object|ACT|participation rate for the ACT in each US state (values: 0-1)|  
|act_english|float|ACT|average score on english section of ACT (values: 0-36)| 
|act_math|float|ACT|average score on math section of ACT (values: 0-36)| 
|act_reading|float|ACT|average score on reading section of ACT (values: 0-36)|
|act_science|float|ACT|average score on science section of ACT (values: 0-36)| 
|act_composite|float|ACT|average score on composite section of ACT (values: 0-36)| 
|sat_participation|object|SAT|participation rate for the ACT in each US state (values: 0-1)|  
|sat_ebrw|int|SAT|average score on reading & writing section of SAT (values: 200-800)| 
|sat_math|int|SAT|average score on math section of SAT (values: 200-800)| 
|sat_total|int|SAT|average score on SAT (average of combined reading & writing + math)(values: 200-800)|

---
## External Research

More than 2.1 million students in the class of 2018 took the redesigned SAT resulting in an increase of 25% over the class of 2017, according to the 2018 SAT Suite of Assessments Program Results. This is the largest number of students in a graduating class to take the SAT.<sup>1</sup> 

Though this achievement does seems to be attractive at a face value, it is crucial to note that there is a negative correlation participation rates and test scores. This translates to the higher the participation rate, the lower the average total test score. Considering that high SAT scores are demanded for college admissions, this is a worrying issue.

It is important to address College Board current stand in believing that students are gaining greater access and opportunity as more students take SATs where in reality the more widely their test is offered, the higher the chances are of more students performing poorly. 

One notable example is Washington, DC, where students had one of the highest participation rates of all states in 2017 - 2018, but earned the lowest test scores. Conversely, Minnesota had participation rates in the bottom 10 in 2017-18, but earned the highest test scores. 

Taking a closer look at test scores, it was evident that the more students who performed poorly than well. If College Board wants to promote SAT as a significant contributor into getting to college, the SAT itself is currently hindering students' access to college.

<sup>1</sup> https://www.collegeboard.org/releases/2018/more-than-2-million-students-in-class-of-2018-took-sat-highest-ever


---
## Conclusions & Recommendations 

**Recommendations in selecting a state to increase participation rate**

- I would focus on states that doesn't have a very high ACT participation rate (probale ACT mandatory testing) and very high SAT participation rate and ideally in the mid region of the country
- I would also focus on states with a significant change in total test scores from 2017-2018 which will indicate the potential of being high peforming state and more receptive to positive changes.

**Assumption made:**

1. The number of high school graduates will not change drastically every year and it is approximately appropriate for future year projections
2. Money allocated  by the Central Board will be the same irregardless of which state is recommended to improve SAT participation rates.


**Future Consideration**
There is a distinct negative correlation between participation rates and test scores, where the higher the participation rates, the lower the test scores (and vice versa) . If the College Board decides to focus solely on increasing participation rates and ultimately achieving the ideal of a 100% participation rate, there is a very high chance that it might pave the way in deteriorating the test scores of the students

I recommend that College Board will shift its focus away from participation rate and more towards improving test scores by improving the access to test prep resources, allocating money to reduce the finanical burden students might have to encourage them to take SATs etc.

***Suggestions in improving data collection:***

As the composite ACT score is scaled differently from total SAT score, finding their average % against each individual maximum perfect score will enable analysis more representative.

- Collecting more granular data such as the particiaption district and school level in each state will give a better overall overview of the data collected
--- 
