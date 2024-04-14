
# Information Based Learning - ID3 Algorithm

The dataset below describes the predictive annual income of individuals based on the descriptive features `Age`, `Education`, `Marital Status` and `Occupation`.

| Id | Age | Education   | Marital Status | Occupation   | Annual Income |
|----|-----|-------------|----------------|--------------|---------------|
| 1  | 39  | bachelors   | never married  | transport    | 25K-50K       |
| 2  | 50  | bachelors   | married        | professional | 25K-50K       |
| 3  | 18  | high school | never married  | agriculture  | <25K          |
| 4  | 28  | bachelors   | married        | professional | 25K-50K       |
| 5  | 37  | high school | married        | agriculture  | 25K-50K       |
| 6  | 24  | high school | never married  | armed forces | <25K          |
| 7  | 52  | high school | divorced       | transport    | 25K-50K       |
| 8  | 40  | doctorate   | married        | professional | >50K          |

## Question 1

Calculate the entropy for the entire dataset. The `Annual Income` is the target feature.

### Answer 1

The entropy of the entire dataset is calculated as follows:

$$ \text{Entropy(\text{Annual Income})} = - \sum_{i=1}^{n} p_i \log_2 p_i $$

where $p_i$ is the probability of the $i$th class.

The probability of each class of `Annual Income` is calculated as follows:

$p(\text{<25K}) = \frac{2}{8} = 0.25$  
$p(\text{25K-50K}) = \frac{5}{8} = 0.625$  
$p(\text{>50K}) = \frac{1}{8} = 0.125$  

The entropy of the entire dataset is calculated as follows:

$\text{H(\text{AI})} = - (\text{H(\text{AI=<25K})} + \text{H(\text{AI=25K-50K})} + \text{H(\text{AI=>50K})})$  
$\text{H(\text{AI})} = - ((0.25 \log_2 0.25) + (0.625 \log_2 0.625) + (0.125 \log_2 0.125))$  

$\text{H(\text{AI})} = - ((0.25 \times -2) + (0.625 \times 0.6781) + (0.125 \times -3))$  
$\text{H(\text{AI})} = - (-0.5 + -0.4238 + -0.375)$  
$\text{H(\text{AI})} = - (-1.2988)$  
$\text{H(\text{AI})} = 1.2988$

## Question 2

Using this dataset construct the decision tree that would be generated by the ID3 algorithm: using entropy-based information gain. (only use the `Education` `Marital Status`, `Occupation` descriptive features)

Clearly show the entropy and information gain for each feature that was generated by the ID3 algorithm.

### Answer 2

The decision tree generated by the ID3 algorithm is as follows:

1. **Root Node**: The root node is the feature with the highest information gain.  
   - Calculate the information gain for each feature: `Education`, `Marital Status`, and `Occupation`.

$$ \text{IG} = \text{H(\text{D})} - \text{Entropy(\text{Annual Income} | \text{Feature})} $$

\[ IG(Education) = H(D) - \sum_{j} \frac{|D_j|}{|D|} \cdot H(D_j) \]

- Calculate the weighted average entropy for `Education`.

$H(E, D) = \frac{|E_{\text{bachelors}}|}{|D|} H(E_{\text{bachelors}}) + \frac{|E_{\text{highschool}}|}{|D|} H(E_{\text{highschool}})+ \frac{|E_{\text{doctorate}}|}{|D|} H(E_{\text{doctorate}})$  
$H(E, D) = \frac{3}{8} H(E_{\text{bachelors}}) + \frac{4}{8} H(E_{\text{highschool}}) + \frac{1}{8} H(E_{\text{doctorate}})$  
$H(E_{\text{bachelors}}) = ((\frac{3}{3} \log_2 \frac{3}{3}) + (\frac{0}{3} \times \log_2 \frac{0}{3})+ (\frac{0}{3} \times \log_2 \frac{0}{3})) = 0$
$H(E_{\text{highschool}}) = ((\frac{2}{4} \log_2 \frac{2}{4}) + (\frac{2}{4} \times \log_2 \frac{2}{4})+ (\frac{0}{4} \times \log_2 \frac{0}{4})) = -0.5 - 0.5 + 0 = -1$
$H(E_{\text{doctorate}}) = ((\frac{1}{1} \log_2 \frac{1}{1}) + (\frac{0}{1} \times \log_2 \frac{0}{1})+ (\frac{0}{1} \times \log_2 \frac{0}{1})) = 0$

$H(E, D) = \frac{3}{8} \times 0 + \frac{4}{8} \times -1 + \frac{1}{8} \times 0$
$H(E, D) = 0 - 0.5 + 0 = -0.5$
$I(Education) = 1.2988 - (-0.5) = 1.7988$


---








 - **Education**:
   - Calculate the entropy for each class of `Education`.
   - Calculate the information gain for `Education`.
   - $p(\text{bachelors}) = \frac{3}{8} = 0.375$
   - $p(\text{high school}) = \frac{4}{8} = 0.5$
   - $p(\text{doctorate}) = \frac{1}{8} = 0.125$
   - $ \text{Entropy(\text{AI | Education})} = - \sum_{i=1}^{n} p_i \text{Entropy(\text{AI=class})} $
   - $ \text{Entropy(\text{AI | Education})} = -(\text{Entropy(\text{AI=bachelors})} + \text{Entropy(\text{AI=high school})} + \text{Entropy(\text{AI=doctorate})})$
   - $\text{Entropy(\text{AI | Education})} = - (0.375 \times log_2 0.375) + (0.5 \times log_2 0.5) + (0.125 \times log_2 0.125)$
   - $\text{Entropy(\text{AI | Education})} = - (0.375 \times -1.415) + (0.5 \times -1) + (0.125 \times -3)$
   - $\text{Entropy(\text{AI | Education})} = - (-0.5306 - 0.5 - 0.375)$  
   - $\text{Entropy(\text{AI | Education})} = -(-1.4056) = 1.4056$  


$ \text{Information Gain} = \text{Entropy(\text{Annual Income})} - \text{Entropy(\text{Education})} $  
$ \text{Information Gain} = 1.2988 - 1.4056 = -0.1068 $  


## Question 3

A colleague suggests that the feature `Marital Status` should be the root of the tree. Would you agree with this? Clearly explain your reasoning.