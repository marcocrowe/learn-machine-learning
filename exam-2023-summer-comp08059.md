***QUESTION 3  [TOTAL MARKS: 25]*** 

![](Aspose.Words.17b57e7b-c820-4cb7-8c23-e01c907eeb7f.001.png)

**TECHNOLOGICAL UNIVERSITY OF THE SHANNON: MIDLANDS MIDWEST *![](Aspose.Words.17b57e7b-c820-4cb7-8c23-e01c907eeb7f.002.png)*SUMMER** **EXAMINATIONS** **2022/2023**

**MODULE:**    COMP08059 - Machine Learning** 

**PROGRAMME(S):**  

LC\_KSOFM\_KMY  Bachelor of Science (Honours) Software Development LC\_KISYM\_KMY  Bachelor of Science (Honours) Internet Systems 

Development 

LC\_KISYA\_KMY  Bachelor of Science (Honours) Internet Systems 

Development 

**YEAR OF STUDY:**   4 **EXAMINER(S):**  

Carol Rainsford  (Internal) Mr. Michael Connolly  (External) 

**TIME ALLOWED:**    2.5 HOURS 

**INSTRUCTIONS:    Answer 4 questions. All questions carry equal marks. ![](Aspose.Words.17b57e7b-c820-4cb7-8c23-e01c907eeb7f.003.png)**

**PLEASE DO NOT TURN OVER THIS PAGE UNTIL YOU ARE INSTRUCTED TO DO SO.** The use of programmable or text storing calculators is expressly forbidden.

Please note that where a candidate answers more than the required number of questions, the examiner will mark all questions attempted and then select the highest scoring ones.![](Aspose.Words.17b57e7b-c820-4cb7-8c23-e01c907eeb7f.004.png)

***Requirements for this paper: 1. Calculators***

**Q 1(a)  [6 Marks]** Machine learning has become an important subject within development organisations that are looking for innovative ways to leverage data assets to help business gain a new level of understanding of the information available to them.  Discuss the benefit of using machine learning in an organisation? 

**Q 1(b)  [12 Marks]** 

Today, we are seeing major advancements and commercial solutions in Machine Learning tool and technologies. Discuss six key enablers to these advancements. 

**Q 1(c)  [7 Marks]** 

Define what is meant by Supervised Learning. Use an example to illustrate your answer. 

***[End of Question 1]*** 

The revenue commission performs audits on public companies to find and fine tax defaulters. To perform an audit, a tax inspector visits a company and spends several days examining the company’s accounts. This is time consuming, expensive and relies on experienced, expert tax inspectors, performing an audit. The revenue commission currently  selects  companies  for  audit  at  random.  A  lot  of  time  is  spent  auditing compliant companies which could be better spent auditing companies which have a high propensity to commit revenue fraud.  

The revenue commissioner would like to make the process more efficient by targeting audits at companies who are likely to be in breach of tax regulations, rather than selecting  companies  at  random.  In  this  way  the  revenue  commission  hopes  to maximize the yield from the audits that it performs. 

Companies interact with the revenue commission by registering the company when it is formed. During registration the company provides information such as the type of industry the company is involved in, details of the directors of the company, and where the company is located. Once a company has been registered, it must provide a tax return at the end of every financial year. This includes all financial details of the company’s operations during the year and is the basis of calculating the tax liability of a company. Public companies also must file public documents every year that outline how they have been performing, details of any changes in directorship, and so on. 

COMP08059 – Machine Learning 

Summer Examinations 2022/2023  Page 3 of 12 

**Q 2(a)  [4 Marks]** Discuss **four** (4) reasons why companies may use Analytical models.  

**Q 2(b)  [18 Marks]** 

Propose **two** (2) ways in which predictive data analytics could be used to help address the above business problem. For each proposed analytical approach, 

1) describe the predictive model that will be built, 
1) how the model will be used by the business, and  
1) how using the model will help address the original business problem 

**Q 2(c)  [3 Marks]** 

Once  a  set  of  possible  analytical  solutions  have  been  defined  that  address  the business's problem, the next task is to evaluate the feasibility of each solution. Discuss **three** (3) question you would ask to determine the feasibility of each solution involves. 

***[End of Question 2]*** 

COMP08059 – Machine Learning 

Summer Examinations 2022/2023  Page 4 of 12 
***QUESTION 5  [TOTAL MARKS: 25]*** 

**Q 3(a)  [8 Marks]** 

The table below shows the age of each member in a tennis club. Based on this data calculate the following summary statistics for the AGE feature: 


| **ID**  | 1  | 2  | 3  | 4  | 5  | 6  | 7  | 8  | 9  | 10 | 11 | 12 | 13 | 14 | 15 | 16 | 17 | 18 | 19 | 20 |
|---------|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|----|
| **AGE** | 51 | 39 | 34 | 27 | 23 | 43 | 41 | 55 | 24 | 25 | 38 | 17 | 21 | 37 | 35 | 38 | 31 | 24 | 35 | 33 |

| Id | Age |
|----|-----|
| 1  | 51  |

1) Range

The range is the difference between the maximum and minimum values in a dataset. It gives an idea of how spread out the values are in a dataset. The formula for calculating the range is:

$\text{Range} = \text{Max} - \text{Min}$
$\text{Range} = 55 - 17$
$\text{Range} = 38$

2) Variance

Variance is a measure of how spread out the values in a dataset are around the mean. It is calculated as the average of the squared differences between each value and the mean. The formula for calculating the variance is:

$$\text{Variance} = \frac{\sum_{i=1}^{n} (x_i - \bar{x})^2}{n}$$

$\bar{x}$ is the mean of the dataset.
$\bar{x} = \frac{\sum_{i=1}^{n} x_i}{n} = \frac{51 + 39 + 34 + \ldots + 33}{20} = \frac{671}{20} = 33.55$

#### As a formula

$\text{Variance} = \frac{(51 - 33.55)^2 + (39 - 33.55)^2 + \ldots + (33 - 33.55)^2}{20} = \frac{17.45^2 + 5.45^2 + \ldots + 0.55^2}{20} = \frac{304.40 + 29.70 + \ldots + 0.30}{20} = \frac{1024.50}{20} = 92.1475$

#### As a table

| Id                               | Age | $Age_i - \overline{Age}$ | $(Age_i - \overline{Age})^2$    |
|----------------------------------|-----|--------------------------|---------------------------------|
| 1                                | 51  | (51-33.55) = 17.45       | $17.45^2$ =  304.5025           |
| 2                                | 39  | 5.45                     | 29.7025                         |
| 3                                | 34  | 0.45                     | 0.2025                          |
| 4                                | 27  | -6.55                    | 42.9025                         |
| 5                                | 23  | -10.55                   | 111.3025                        |
| 6                                | 43  | 9.45                     | 89.3025                         |
| 7                                | 41  | 7.45                     | 55.5025                         |
| 8                                | 55  | 21.45                    | 460.1025                        |
| 9                                | 24  | -9.55                    | 91.2025                         |
| 10                               | 25  | -8.55                    | 73.1025                         |
| 11                               | 38  | 4.45                     | 19.8025                         |
| 12                               | 17  | -16.55                   | 273.9025                        |
| 13                               | 21  | -12.55                   | 157.5025                        |
| 14                               | 37  | 3.45                     | 11.9025                         |
| 15                               | 35  | 1.45                     | 2.1025                          |
| 16                               | 38  | 4.45                     | 19.8025                         |
| 17                               | 31  | -2.55                    | 6.5025                          |
| 18                               | 24  | -9.55                    | 91.2025                         |
| 19                               | 35  | 1.45                     | 2.1025                          |
| 20                               | 33  | -0.55                    | 0.3025                          |
| -                                | -   | -                        | -                               |
| $\sum(Age_i - \overline{Age})^2$ |     |                          | 1,842.95                        |
| $Variance$                       |     |                          | $\frac{1,842.95}{20} = 92.1475$ |

3) 1st quartile (25th percentile)  

The 1st quartile is the value below which 25% of the data falls. To calculate the 1st quartile, the data must be sorted in ascending order. The formula for calculating the 1st quartile is:

$\text{1st quartile} = \frac{n + 1}{4}$
$\text{1st quartile} = \frac{20 + 1}{4}$
$\text{1st quartile} = \frac{21}{4}$
$\text{1st quartile} = 5.25$

The formula used to calculate the first quartile (Q1) between the 5th and 6th data points is generally expressed as follows:

$Q1 = P_{lower} + \text{fraction} \times (P_{higher} - P_{lower})$

Where:

- $P_{lower}$ is the lower value, i.e., the 5th data point in the sorted data set (24 in this case).
- $P_{higher}$ is the higher value, i.e., the 6th data point in the sorted data set (25 in this case).
- $\text{fraction}$ is the difference between the calculated Q1 index and the integer part of that index. In this case, it was calculated to be 0.25.

To calculate Q1:

$Q1 = 24 + 0.25 \times (25 - 24)$
$Q1 = 24 + 0.25 \times 1$
$Q1 = 24 + 0.25$
$Q1 = 24.25$

**Q 3(b)  [12 Marks]** 

Tachycardia is a condition that causes the heart to beat faster than normal at rest. The occurrence of tachycardia can have serious implications including increased risk of stroke or sudden cardiac arrest. An analytics consultant has been hired by a major hospital to build a predictive model that predicts the likelihood that a patient at a heart disease clinic will suffer from tachycardia in the month following a visit to the clinic. The hospital will use this model to make predictions for each patient when they visit the clinic and offer increased monitoring for those deemed to be at risk. The analytics consultant has generated an ABT to be used to train this model. 

The descriptive features in this dataset are defined as follows: 

- AGE: The patient’s age 
- GENDER: The patient’s gender (male or female) 
- WEIGHT: The patient’s weight 
- HEIGHT: The patient’s height 
- BMI: The patient’s body mass index (BMI) which is calculated as where weight is measured in kilograms and height in meters. 
- SYS. B.P.: The patient’s systolic blood pressure 
- DIA. B.P.: The patient’s diastolic blood pressure 
- HEART RATE: The patient’s heart rate 
- H.R. DIFF.: The difference between the patient’s heart rate at this visit and at their last visit to the clinic  
- PREV. TACHY.: Has the patient suffered from tachycardia before? 
- TACHYCARDIA: Is the patient at high risk of suffering from tachycardia in the next month? 

The consultant generated the following data quality report from the ABT. 

| Feature           | Count | % Missing | Cardinality | Mode  | Mode Freq | Mode % | 2nd Mode | 2nd Mode Freq | 2nd Mode % |
|-------------------|-------|----------:|------------:|-------|----------:|-------:|----------|--------------:|-----------:|
| Gender            | 2,440 |         0 |           4 | Male  |      1591 |   65.2 | Female   |           647 |      20.52 |
| Prev. Tachycardia | 2,440 |      4402 |           3 | FALSE |       714 |  52.27 | TRUE     |           652 |      47.73 |
| Tachycardia       | 2,440 |       201 |           3 | FALSE |      1205 |   50.4 | TRUE     |          1156 |       49.6 |


| Feature   | Count | % Missing | Cardinality |  Min | 1stQuartile |    Mean | Median | 3rd Quartile |       Max | Standard Deviation |
|-----------|------:|----------:|------------:|-----:|------------:|--------:|-------:|-------------:|----------:|-------------------:|
| Age       | 2,440 |         0 |           7 |    1 |           3 |    3.58 |      4 |            5 |         7 |               1.22 |
| Weight    | 2,440 |         0 |         174 |    0 |          81 |    95.3 |     95 |          100 |       157 |              20.89 |
| Height    | 2,440 |         0 |         109 | 1.47 |         162 |  162.21 |  171.5 |          179 |       204 |              41.05 |
| BMI       | 2,440 |         0 |        1383 |    0 |       27.64 | 18523.4 |  32.02 |        38.57 | 596495.31 |          77,08,839 |
| SYS. B.P. | 2,440 |         0 |         149 |   62 |         115 |  127.84 |    124 |          135 |      1144 |              29.11 |
| DIA. B.P. | 2,440 |         0 |         109 |   46 |          77 |   85.34 |     84 |           92 |     173.6 |              14.25 |
| Heartrate | 2,440 |         0 |         119 |   57 |       91.75 |  103.28 |    100 |          110 |     190.4 |              18.21 |
| H.R. Diff | 2,440 |     13.03 |          78 |  -50 |          -4 |       3 |      1 |            8 |        47 |              12.35 |

Discuss this data quality report in terms of the following, outline the implication of the result and advice in handling this result: 

1) Missing values
2) Irregular cardinality 
3) Outliers 

**Q 3(c)  [5 Marks]** 

Discuss the advantages of machine learning platforms versus the advantages of programming languages.

Advanced analytics is the use of mathematical techniques to identify patterns in data. These patterns can be used to predict future events or to identify opportunities and risks. Advanced analytics can be used to solve a wide range of business problems, from predicting customer behaviour to optimising supply chains. Programming languages such as Python and R are commonly used to perform advanced analytics.

***[End of Question 3]*** 

COMP08059 – Machine Learning 

Summer Examinations 2022/2023  Page 8 of 12 
***QUESTION 10  [TOTAL MARKS: 25]*** 

**Q 4(a)  [8 Marks]**

The table below shows a set of eight Scrabble pieces.  


|   |   |   |   |   |   |   |   |
|---|---|---|---|---|---|---|---|
| O | X | Y | M | O | R | O | N |

What is the Entropy in bits for the letters in this set? Clearly state the Entropy formula in your answer.  

$Entropy = -\sum_{i=1}^{n} p_i \log_2 p_i$

Where:

- $Entropy$ is the entropy of the dataset.
- $n$ is the number of classes in the dataset.
- $p_i$ is the probability of class $i$ in the dataset.

Frequency Table of each letter in the dataset:

| Letter       | Frequency | Probability | $p_i \log_2 p_i$           | $Entropy_i$ |
|--------------|----------:|------------:|----------------------------|------------:|
| O            |         3 |       $3/8$ | $(3/8 \times \log_2(3/8))$ |     - 0.531 |
| X            |         1 |       $1/8$ | $(1/8 \times \log_2(1/8))$ |     - 0.375 |
| Y            |         1 |       $1/8$ | $(1/8 \times \log_2(1/8))$ |     - 0.375 |
| M            |         1 |       $1/8$ | $(1/8 \times \log_2(1/8))$ |     - 0.375 |
| R            |         1 |       $1/8$ | $(1/8 \times \log_2(1/8))$ |     - 0.375 |
| N            |         1 |       $1/8$ | $(1/8 \times \log_2(1/8))$ |     - 0.375 |
| -            |         - |           - | -                          |           - |
| $-\sum(E_i)$ |         - |           - | -                          |       2.406 |

Entropy = 2.406 bits

**Q 4(b)  [9 Marks]** 

What would be the reduction in entropy (Information Gain) if you split the letters into two sets, vowels, and consonants? 

### Step 1: Calculate the frequency and probability of each set

1. **Vowels:** The only vowel in the set is O, which appears three times in the set of eight letters.
    - Probability of vowels set: $p_{\text{vowels}} = \frac{3}{8} = 0.375$.

2. **Consonants:** The consonants in the set are X, Y, M, R, and N. Each of them appears once.
    - Probability of consonants set: $p_{\text{consonants}} = \frac{5}{8} = 0.625$.

### Step 2: Calculate the entropy of each set

1. **Entropy of vowels set**: Since there is only one type of vowel (O) in the set, and it appears three times, we calculate its entropy:

    - Probability of O: $p_O = \frac{3}{3} = 1$.
    - $E_{\text{vowels}} = -p_O \log_2 p_O = -1 \times \log_2 1 = 0$ bits.
    - Therefore, the entropy of the vowels set is 0 bits.

2. **Entropy of consonants set**: Each consonant (X, Y, M, R, N) appears once.

    - Each consonant has a probability of $p = \frac{1}{5} = 0.2$.
    - Calculate the entropy of consonants:
        - $E_{\text{consonants}} = - \sum_{i=1}^{5} p \log_2 p$
        - $E_{\text{consonants}} = -5 \times \left(0.2 \times \log_2 0.2\right)$
        - $E_{\text{consonants}} = -5 \times (0.2 \times -2.322)$
        - $E_{\text{consonants}} = 1.160$ bits.

### Step 3: Calculate the weighted entropy after the split

- Weighted entropy = $p_{\text{vowels}} \cdot E_{\text{vowels}} + p_{\text{consonants}} \cdot E_{\text{consonants}}$
- Weighted entropy = $\frac{3}{8} \times 0 + \frac{5}{8} \times 1.160$
- Weighted entropy = $0 + 0.725$ bits.

### Step 4: Calculate the information gain

- **Original entropy**: The original entropy, calculated previously, is approximately $2.406$ bits.
- Information gain is the reduction in entropy that results from splitting the data.
- Information gain = Original entropy - Weighted entropy after split
- Information gain = $2.406 - 0.725$
- Information gain = $1.681$ bits.

Therefore, the reduction in entropy (information gain) if you split the letters into two sets, vowels (O) and consonants (X, Y, M, R, N), is approximately $1.681$ bits.

**Q 4(c)  [8 Marks]**

### Maximum Possible Entropy in Bits for a Set of Eight Scrabble Pieces

Entropy measures the uncertainty or randomness in a set of data. In the context of a set of eight Scrabble pieces, the maximum possible entropy would occur when each letter is unique, and therefore, each letter appears once in the set.

In this case, the probability $p_i$ for each of the eight letters would be equal, specifically $\frac{1}{8}$. The entropy is calculated using the formula:

$\text{Entropy} = -\sum_{i=1}^{n} p_i \log_2 p_i$

Given $n = 8$, and $p_i = \frac{1}{8}$:

$\text{Entropy} = -8 \left(\frac{1}{8} \log_2 \frac{1}{8}\right)$
$\text{Entropy} = -8 \left(\frac{1}{8} \times -3\right)$
$\text{Entropy} = 3 \text{ bits}$

Therefore, the maximum possible entropy for a set of eight Scrabble pieces is 3 bits.

### High Entropy vs. Low Entropy in Scrabble

When playing Scrabble, the preference for a set of letters with high entropy or low entropy depends on the game strategy and the stage of the game.

- **High Entropy:** A set of letters with high entropy implies a greater variety of letters. This increases the probability of having a diverse set of letters, which can offer more options for forming words. It may be preferable in the early stages of the game when you want to form longer words or take advantage of more board positions.

- **Low Entropy:** A set of letters with low entropy implies less variety, which can be beneficial if you have a set of letters that forms high-scoring words, especially with premium board positions such as triple word or triple letter scores. This may be preferable in the later stages of the game when the board is crowded, and scoring opportunities are limited.

In general, a set of letters with high entropy provides more flexibility and a higher chance of forming words, which is preferable for the player. However, having the right letters to form high-scoring words (even if entropy is lower) can be advantageous as well.

What is the maximum possible entropy in bits for a set of eight Scrabble pieces. In general, which is preferable when you are playing Scrabble: a set of letters with high entropy or a set of letters with low entropy? 

***[End of Question 4]***

## Question 5

### Question 5(a) [6 Marks]

The table below gives details of factors (Humidity, Cloudy, Windy) that impact whether it will rain or not.  All features have binary have binary values (True or False) 



| **ID** | **Humidity** | **Cloudy** | **Windy** | **Rain** |
|--------|--------------|------------|-----------|----------|
| 1      | True         | True       | False     | False    |
| 2      | False        | True       | False     | False    |
| 3      | True         | False      | True      | False    |
| 4      | True         | False      | True      | False    |
| 5      | False        | True       | False     | True     |
| 6      | True         | False      | True      | False    |
| 7      | True         | False      | True      | False    |
| 8      | True         | False      | True      | True     |
| 9      | False        | True       | False     | False    |
| 10     | True         | False      | True      | True     |

Using the above dataset calculate the following probabilities.

1) P(Windy = True)

$P(Windy = True) = \frac{\text{Number of instances where Windy = True}}{\text{Total number of instances}} = \frac{6}{10} = 0.6$

2) P(Humidity = True, windy = False))

$P(Humidity = True, Windy = False) = \frac{\text{Number of instances where Humidity = True and Windy = False}}{\text{Total number of instances}} = \frac{1}{10} = 0.1$

3) P(windy = False | Humidity = True)

$$P(A|B) = \frac{P(A \cap B)}{P(B)}$$

$P(Windy = False | Humidity = True) = \frac{P(Windy = False, Humidity = True)}{P(Humidity = True)} = \frac{1/10}{7/10} = \frac{1}{7} \approx 0.1429$

**Q 5(b)  [13 Marks]** 

The following Analytic Based Table has three (3) descriptive features that impact whether  a  student  will  pass  a  module.  The  description  features  StudyHard, AttendLectures and DoCA all impact the target feature PassModule.   



| **ID** | **StudyHard** | **AttendLectures** | **DoesCA** | **PassModule** |
|--------|---------------|--------------------|-------------|----------------|
| 1      | True          | True               | False       | False          |
| 2      | False         | True               | False       | False          |
| 3      | True          | False              | True        | False          |
| 4      | True          | False              | True        | False          |
| 5      | False         | True               | False       | True           |
| 6      | True          | False              | True        | False          |
| 7      | True          | False              | True        | False          |
| 8      | True          | False              | True        | True           |
| 9      | False         | True               | False       | False          |
| 10     | True          | False              | True        | True           |

Clearly state Bayes theorem. Using Bayes Theorem determine the probability of a student passing a module given that they StudyHard, do **not** AttendLectures and DoCA.  

Bays Theorem states that the probability of an event based on prior knowledge of conditions that might be related to the event. Mathematically, it is expressed as:

$$P(A|B) = \frac{P(B|A) \times P(A)}{P(B)}$$

$P(PassModule | (StudyHard,\overline{AttendLectures}, DoesCA))$

$$P(Pass | (StudyHard,\overline{AttendLectures}, DoCA)) = \frac{P((StudyHard,\overline{AttendLectures}, DoCA) | Pass) \times P(Pass)}{P(StudyHard,\overline{AttendLectures}, DoCA)}$$

COMP08059 – Machine Learning 

Summer Examinations 2022/2023  Page 11 of 12 
**Q 5(c)  [6 Marks]** 

The  Table  below  lists  a  dataset  containing  details  of  customers  at  a  transport company.  The  descriptive  features  are  ID,  Occupation,  Gender,  Age, ModeofTransport. The PrefSocialMedia is the target feature in this domain.  ![](Aspose.Words.17b57e7b-c820-4cb7-8c23-e01c907eeb7f.010.png)

**ID  Occupation  Gender  Age  ModeofTransport  PrefSocialMedia** 1  Painter  Female  43  Car  Email ![](Aspose.Words.17b57e7b-c820-4cb7-8c23-e01c907eeb7f.011.png)

2  Programmer  Female  57  Bike  Phone 

3  Manager  Male  21  Bike  Email 

4  Doctor  Female  47  Walk  Phone 

5  Nurse  Male  55  Car  Phone 

6  Policeman  Male  19  Bike  Email 

7  Teacher  Male  49  Car  Phone 

8  Fireman  Male  51  Walk  Email 

9  Radiographer  Female  18  Car  Phone 

1) Using equal-frequency binning transform the Age feature into a categorical feature with three levels youth, middle-aged and senior. Explain the process you apply.  
2) Examine the descriptive features in the dataset and list the features that your would exclude before you would use the dataset to build a predictive model. For each feature you chose to exclude explain why you made this decision. 

***[End of Question 5] [END OF EXAM]*** 
COMP08059 – Machine Learning 

Summer Examinations 2022/2023  Page 12 of 12 
