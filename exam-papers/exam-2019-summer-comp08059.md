![](Aspose.Words.4ebf4bab-32e3-4e68-bc1c-78345ae63c03.001.png)

**LIMERICK INSTITUTE OF TECHNOLOGY *![](Aspose.Words.4ebf4bab-32e3-4e68-bc1c-78345ae63c03.002.png)***

**SUMMER** **EXAMINATIONS** **2018/2019**

COMP08059 – Machine Learning 

Summer Examinations 2018/2019  Page 1 of 7 

**MODULE:**  

**PROGRAMME(S):**  

LC\_KSFDM\_KMY LC\_KISYM\_KMY 

LC\_KISYA\_KMY 

**YEAR OF STUDY:  EXAMINER(S):** 

**TIME ALLOWED:  INSTRUCTIONS:**  

COMP08059-Machine Learning for Predictive Analytics 

Bachelor of Science (Honours) Software Development Bachelor of Science (Honours) Internet Systems Development 

Bachelor of Science (Honours) Internet Systems Development 

4 

Dr. Carol Rainsford  (Internal) Dr. Christophe Meudec  (External) 

**2 HOURS** 

**Answer Question 1 (MANDATORY) and any 2 other questions. Question 1 carries 34 marks and all other questions carry 33 marks.**  

COMP08059 – Machine Learning 

Summer Examinations 2018/2019  Page 3 of 3 

**PLEASE DO NOT TURN OVER THIS PAGE UNTIL YOU ARE INSTRUCTED TO DO SO. ![](Aspose.Words.4ebf4bab-32e3-4e68-bc1c-78345ae63c03.003.png)**The use of a scientific calculator is allowed.

The use of programmable or text storing calculators is expressly forbidden. 

Please note that where a candidate answers more than the required number of questions, the examiner will mark all questions attempted and then select the highest scoring ones.![](Aspose.Words.4ebf4bab-32e3-4e68-bc1c-78345ae63c03.004.png)

***There are no additional requirements for this paper.***

***QUESTION 1                   MANDATORY  [TOTAL MARKS: 34]* Q 1(a)  [10 Marks]** 

The table below lists a dataset containing details of policy holders at an insurance company. The descriptive features included in the table describe each policy holder. The features are ID, occupation, gender, age, the type of insurance policy they hold and their preferred contact channel. The preferred contact channel is the target feature in this domain.  



|**ID** |**OCCUPATION** |**GENDER** |**AGE** |**POLICYTYPE** |**PREFCHANNEL** |
| - | - | - | - | - | - |
|1 |Farmer |female |young |PlanC |Email |
|2 |LabTech |Female |Young |PlanA |Phone |
|3 |Painter |Male |Young |PlanA |Email |
|4 |Geologist |Female |Middle- aged |PlanB |Phone |
|5 |Manager |Male |Middle- aged |PlanC |Phone |
|6 |Nurse |Male |Middle- aged |PlanA |Email |
|7 |Doctor |Male |mature |PlanC |phone |
|8 |Teacher |Male |Mature |PlanB |Email |
|9 |Professor |Male |mature |PlanC |Phone |

Examine the descriptive features in the dataset and outline the features that you would exclude prior to building a predictive model. For each feature you decide to exclude explain why you have made this decision. Assume that this is the complete dataset.  

**Q 1(b)  [12 Marks]** 

The following is a training data set of weather conditions and a target feature of whether it was possible to have a Picnic. Calculate the frequencies and probabilities required by a Naïve Bayes model to represent this domain.  



|**Weather** |**Picnic** |
| - | - |
|Sunny |No |
|Overcast |Yes |
|Rainy |Yes |
|Sunny |Yes |
|Sunny |Yes |
|Overcast |Yes |
|Rainy |No |
|Rainy |No |
|Sunny |Yes |
|Rainy |Yes |
|Sunny |No |
|Overcast |Yes |
|Overcast |Yes |
|Rainy |No |

**Q 1(c)  [12 Marks]** 

State and explain the elements of Baye’s Theorem. Using the results calculated in **Q1(b)** what target level will a naïve Bayes model predict for the following query: 

A person will go on a picnic if the weather is Sunny -  P(yes | sunny). 

***[End of Question1]*** 

COMP08059 – Machine Learning 

Summer Examinations 2018/2019  Page 3 of 7 
***QUESTION 4  [TOTAL MARKS: 33]* Q 2(a)  [12 Marks]** 

Machine Learning is fundamentally an ill-posed problem. Discuss what is meant by this statement? Use an example to illustrate your answer. 

**Q 2(b)  [9 Marks]** 

Discuss what is meant by the term inductive bias and discuss two types of inductive bias that a machine learning algorithm can use. 

**Q 2(c)  [12 Marks]** 

“It is often said that 80% of the work done on predictive analytic projects is done in the Business Understanding, Data Understanding and Data Preparation phase of the CRISP-DM and just 20% is  spent on the Modelling, Evaluation and Deployment phases” (Kelleher J.D et al., 2015) 

Discuss why this may be the case? 

***[End of Question2]*** 

COMP08059 – Machine Learning 

Summer Examinations 2018/2019  Page 4 of 7 
***QUESTION 5  [TOTAL MARKS: 33]* Q 3(a)  [7 Marks]** 

The following table is a snapshot of a large dataset that contains customer policy details of an insurance company. The descriptive features describe the policy holder (ID, occupation, gender, age, motorvalue, policytype). The target feature prefchannel describes the policy holders preferred method of communication.  



|**ID** |**OCCUPATION** |**GENDER** |**AGE** |**MOTOR VALUE** |**POILICY TYPE** |**PREF CHANNEL** |
| - | - | - | - | :- | :- | :- |
|1 |Teacher |Female |22 |42,000 |plana |Txt |
|2 |Programmer |Male |65 |43,000 |Plana |Phone |
|3 |Engineer |Male |23 |21,000 |planc |Txt |
|4 |Nurse |Male |56 |29,000 |Planc |Phone |
|5 |Scientist |Female |78 |18,000 |Planc |Phone |
|6 |Accountant |Female |55 |35,500 |Planb |Email |
|7 |Doctor |Male |48 |42,000 |Plana |Email |
|8 |Mechanic |Male |39 |17,890 |Planc |Email |
|9 |Programmer |Female |36 |60,000 |Plana |Email |
|10 |Engineer |Female |55 |32,000 |planb |email |

1) State whether each descriptive and target feature contains numeric, interval, ordinal, categorical, binary, or textual data. 
1) How many levels does each category and ordinal feature have? 

COMP08059 – Machine Learning 

Summer Examinations 2018/2019  Page 5 of 7 

**Q 3(b)  [14 Marks]** 

A mobile operator is trying to reduce customer churn. Customers are not renewing their contracts once completed. They are moving to competitor mobile networks.  As a  data  analyst  propose  **TWO**  potential  analytical  solutions  to  help  address  this business problem. For each proposed analytical solution **(i)** describe the predictive model that you will build, **(ii)** how the model could be used could by the business, and **(iii)** how using the model will help address the business problem.  

**Q 3(c)  [12 Marks]** 

Once a set of possible analytical solutions are defined that address the business problem, the next task is to evaluate the feasibility of each solution. This involves the data analyst asking a number of questions to business domain experts. Discuss the key questions you would ask in determining the feasibility of the proposed solutions.  

***[End of Question3]*** 

COMP08059 – Machine Learning 

Summer Examinations 2018/2019  Page 6 of 7 
***QUESTION 7  [TOTAL MARKS: 33]* Q 4(a)  [15 Marks]** 

The data quality report is the most important tool of the data exploration process. What information should a data quality report include? 

**Q 4(b)  [12 Marks]** 

When you generate histograms of features, there are a number of common, well- understood shapes that you should look out for. These shapes relate to well-know standard probability distributions. Recognizing that the distribution of the values of a feature in an ABT match one of these standard distributions can help when building machine learning models.  

Define the different distributions that may exist and use an example to illustrate your answer. 

**Q 4(c)  [6 Marks]** 

A goal of the Data Exploration phase of the CRISP-DM is to understand and identify any data quality issues. A data quality issue can be defined as anything unusual about the data in an ABT.  Discuss the most common type of data quality issues that may exist.  

***[End of Question4] [END OF EXAM]*** 
COMP08059 – Machine Learning 

Summer Examinations 2018/2019  Page 7 of 7 
