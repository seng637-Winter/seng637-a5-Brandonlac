**SENG 637- Dependability and Reliability of Software Systems***

**Lab. Report \#5 – Software Reliability Assessment**

| Group \#:      |  17   |
| -------------- | --- |
| Student Names: | Mustayeen Abedin    |
|                |  Nur-Alhuda Ali   |
|                |  Brandon Lac   |
|                |  Mevin Moncy   |
|                |  Kate Reimann   |

# Introduction

This report outlines the use of a reliability assessment tool and conduct a series of tests using provided data. The report comprises two main methods of reliability assessment: Reliability Growth Testing and the use of a Reliability Demonstration Chart (RDC). These methodologies are designed to teach students the practical aspects of measuring and enhancing the reliability of software systems through empirical data analysis.

The subsequent sections of this report will outline the objectives, testing tools, procedures, and evaluation criteria for both reliability growth testing and reliability assessment using RDC, insights into the failure dynamics of software systems and the practical applications of theoretical models in real-world scenarios.
# 

# Assessment Using Reliability Growth Testing 
## Table Of Model Comparision Using Log-likelihood Using All The Data
![image](https://github.com/seng637-Winter/seng637-a5-Brandonlac/assets/19726423/1c4eca96-107a-4250-ad75-79116e30fd40)



## Graph Showing The Top 2 Models Using All the Data
![image](https://github.com/seng637-Winter/seng637-a5-Brandonlac/assets/19726423/a4508cf7-74c1-4e4d-8fef-f0f31f4e029c)

In selecting an optimal model for software reliability from a set of candidates, Akaike's Information Criterion (AIC) and Bayesian Information Criterion (BIC) are essential metrics. AIC seeks a model that fits the data well without overcomplicating it, applying a constant penalty for each additional parameter. It's preferred when the focus is on the model’s goodness of fit, especially with larger data sets where overfitting is less of a concern.

BIC, conversely, imposes a stricter penalty that increases with sample size, favoring simpler models. This is particularly valuable in large-sample scenarios to avoid overfitting and ensure model parsimony. Ultimately, both AIC and BIC guide us toward a model that balances complexity with an accurate representation of the data, with the choice between them hinging on the specific modeling context and the risk of overfitting.

As depicted in the table, DW3 with covariates F and GM with covariate F gave the lowest scores for AIC and BIC. Thus being the most predictable for failure. With score of 122.199 (AIC), 127.935 (BIC) for DW3 Discrete Weibull Type 3 model covariant F and 125.323 (AIC), 129.625 (BIC) for GM Geometric Model. 

The range analysis was done using 
# Assessment Using Reliability Demonstration Chart 

# 

# Comparison of Results

# Discussion on Similarity and Differences of the Two Techniques

# How the team work/effort was divided and managed

# 

# Difficulties encountered, challenges overcome, and lessons learned

# Comments/feedback on the lab itself
