**SENG 637- Dependability and Reliability of Software Systems***

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#:      |  17   |
| -------------- | --- |
| Student Names: | Mustayeen Abedin    |
|                |  Nur-Alhuda Ali   |
|                |  Brandon Lac   |
|                |  Mevin Moncy   |

# Introduction

This report outlines the use of a reliability assessment tool and conduct a series of tests using provided data. The report comprises two main methods of reliability assessment: Reliability Growth Testing and the use of a Reliability Demonstration Chart (RDC). These methodologies are designed to teach students the practical aspects of measuring and enhancing the reliability of software systems through empirical data analysis.

The subsequent sections of this report will outline the objectives, testing tools, procedures, and evaluation criteria for both reliability growth testing and reliability assessment using RDC, insights into the failure dynamics of software systems and the practical applications of theoretical models in real-world scenarios.
# 

# Assessment Using Reliability Growth Testing 
## Table Of Model Comparision Using Log-likelihood Using All The Data
![image](https://github.com/seng637-Winter/seng637-a5-Brandonlac/assets/19726423/1c4eca96-107a-4250-ad75-79116e30fd40)



## Graph Showing The Top 2 Models Using All the Data
![image](https://github.com/seng637-Winter/seng637-a5-Brandonlac/assets/19726423/a4508cf7-74c1-4e4d-8fef-f0f31f4e029c)

## Graph of the intensity
![image](https://github.com/seng637-Winter/seng637-a5-Brandonlac/assets/19726423/23db4206-a574-4eb4-b323-96225355d727)


In selecting an optimal model for software reliability from a set of candidates, Akaike's Information Criterion (AIC) and Bayesian Information Criterion (BIC) are essential metrics. AIC seeks a model that fits the data well without overcomplicating it, applying a constant penalty for each additional parameter. It's preferred when the focus is on the model’s goodness of fit, especially with larger data sets where overfitting is less of a concern.

BIC, conversely, imposes a stricter penalty that increases with sample size, favoring simpler models. This is particularly valuable in large-sample scenarios to avoid overfitting and ensure model parsimony. Ultimately, both AIC and BIC guide us toward a model that balances complexity with an accurate representation of the data, with the choice between them hinging on the specific modeling context and the risk of overfitting.

As depicted in the table, DW3 with covariates F and GM with covariate F gave the lowest scores for AIC and BIC. Thus being the most predictable for failure. With score of 122.199 (AIC), 127.935 (BIC) for DW3 Discrete Weibull Type 3 model covariant F and 125.323 (AIC), 129.625 (BIC) for GM Geometric Model. 

## Range analysis  

The range analysis was done using excel for Laplace calculations, the useful range of data was found to be roughly 80% mostly exclusing the outer boundaries of the failture data. This is probably due to the infancy stage and the wear out stage of the software development reliablity, also known as the bathtub curve.

## A discussion on decision making given a target failure rate

Setting a target failure rate is essential for guiding decisions in system maintenance and performance improvement. When actual failure rates near the target, it prompts actions like enhanced monitoring or maintenance. If rates consistently exceed the target, this may necessitate system redesign. Meeting targets comfortably could lead to resource reallocation. These decisions aim to balance reliability with resource optimization.

## Advantages of Reliability Growth Models

Advantages of Reliablity Growth Models:
1. Insight : Models are useful in predicting the reliablity over time, helps organizations make informed decisions in anticiptation of failures and to plan ahead.
2. Risk Reduction: By undestanding how the software reliablity changes with modifications, it can be used to reduce the risk of the system failure.
3. Allocation of resources: It helps organizations focus maintenance and testing efforts where they are most needed

Disadvantages of Reliablity Growth Models:
1. Dependent on the quality and quantity of the data, if the data is not accurate or tested correctly, could led to poor decisions.
2. Performing this type of analysis is time consuming with the calcuations for usefulness of the range and anaylsis overall about the system.
3. Diminishing returns as the system matures, the cost of achieving additional reliablity is extensive, outweighing the benefits.
# Assessment Using Reliability Demonstration Chart 

For the purposes of the assignment, values of Developer's Risk α (0.1), User's Risk β (0.1), and Discrimination Ratio γ (2) were left as the default. 

![image](https://github.com/seng637-Winter/seng637-a5-Brandonlac/assets/19726423/f76719b8-7a6f-4728-8602-4c1bf21d92da)

The failures was broken down uniformly within the interval as shown in the table above. For the first interval, there were 2 failure counts thus the time between failure was 0.5 for each. The second interval had 11 failures, evenly distributed would be 0.09 interval between each failure. 

![image](https://github.com/seng637-Winter/seng637-a5-Brandonlac/assets/19726423/916cd402-0a20-4d05-ac12-370047e55bbe)

Plotting the original data with zero of the data points being acceptable, with the acceptable failures of 92 failures per 31 intervals. MTTR = 31/ 92 = 0.33 intervals per failure being the acceptable rate. As shown in the figure above.

![image](https://github.com/seng637-Winter/seng637-a5-Brandonlac/assets/19726423/a98106de-15ad-48e4-a70b-321fba49085c)

Finding the minimum MTTR involved changing the maximum number of failures in order to make all the points of the data from SUT (System Under Test) outside of the unacceptable range. By trial and error, we acheived this by setting the acceptable range of 720 failures over 31 intervals. MTTR = 31/720 = 0.0430 intervals per failure being the acceptable rate. FIO = 720 / 31 = 23 failures per interval. As shown in the figure above.

![image](https://github.com/seng637-Winter/seng637-a5-Brandonlac/assets/19726423/ba4ddf57-a670-464e-8da8-232572ef397d)

Taking the MTTR of 0.0430 intervals per failure and halving it produced the figure below, showing less of the area being covered in the red (unacceptable range), less of our points are inside of the continue testing and more points inside of the green and grey area, which are acceptable. MTTR = 31/1440 = 0.02152 intervals per failure being the acceptable rate. FIO = 1440 /31 = 46 failures per interval. As shown in the figure above.


![image](https://github.com/seng637-Winter/seng637-a5-Brandonlac/assets/19726423/488c05fd-7358-4cc5-9852-1557dcc9acea)
Taking the MTTR of 0.0430 intervals per failure and doubling it produced the figure above. Showing now that the points mainly at the begining of the testing and at the end produced points in the non-acceptable range. The MTTR = 31/ 360 = 0.0861 intervals per failure. This makes sense as there is a higher rate of acceptance.

# 

# Comparison of Results

# Discussion on Similarity and Differences of the Two Techniques

# How the team work/effort was divided and managed
The work was divided into the two parts of Reliability Growth Testing done by Brandon and Mustayeen. The second part of Reliability Demonstration Chart anaylsis was done by Nur and Mevin. We all worked on the report together and then complied onto github for submission.
# 

# Difficulties encountered, challenges overcome, and lessons learned
The first difficulity that was incountered was getting SRTAT to open, we faced errors in the data not being in the correct format and then was forced to use the C-SFRAT tool and did. As shown in the figure below. The cumulative time was calculated by adding the previous time and the time between failure.
![image](https://github.com/seng637-Winter/seng637-a5-Brandonlac/assets/19726423/413c8bf0-1ef6-4e60-99f0-ceb91165b85f)


The interpretation of the data was another difficulity that we had to overcome. We spent many hours researching if the other columns could be used for calculating the inter failure time and understanding the data. By overcoming these challenges, our team not only enhanced our technical skills in software reliability analysis but also developed a better appreciation for the nuances of empirical research in software engineering. This experience will undoubtedly aid us in future projects, where data interpretation and tool compatibility will play essential roles in the successful execution of our assignments.

A lesson learnt from this assignment was that there are different intrepeations of which metric to use in order to find the best model that fits the failure data. There are pros and cons of each and all of the interperations are correct provided that there is a sound explaination.

# Comments/feedback on the lab itself
The data itself was confusing at first to read through and to interpret, we decided to use the time interval as a constant and assumed that the failures were uniformly distrubuted within the time interval in order to find the time between failures. We would suggest that the assignment would specified this as it was a road block for us.
