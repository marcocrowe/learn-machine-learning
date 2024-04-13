
# Information Theory

Information theory is a branch of applied mathematics that revolves around quantifying information.

## Entropy

Entropy is a measure of the uncertainty or randomness of a system. It is a measure of the average amount of information produced by a stochastic source of data.

> "Never ever judge a book by its cover... unless you're talking about entropy." - Mark Crowe (2024)

Information Gain

## Formula

The formula for Information Gain (IG) is used in decision tree algorithms to measure the effectiveness of a feature in partitioning the dataset. It's calculated as the difference between the entropy of the parent dataset \(H(D)\) and the weighted average of the entropies of the child datasets after splitting on a particular feature.

The formula for Information Gain is:

\[ IG(feature) = H(D) - \sum_{j} \frac{|D_j|}{|D|} \cdot H(D_j) \]

Where:

- $H(D)$ is the entropy of the parent dataset \(D\).
- $|D_j|$ is the number of instances in the $j$th child dataset after splitting on the feature.
- $|D|$ is the total number of instances in the parent dataset.
- $H(D_j)$ is the entropy of the $j$th child dataset.

This formula essentially measures the reduction in entropy or uncertainty achieved by splitting the dataset on a particular feature. A higher Information Gain indicates that the feature is more effective in distinguishing between the classes in the dataset.

 the term $\sum_{j} \frac{|D_j|}{|D|} \cdot H(D_j)$

is often referred to as the "weighted average entropy" or "average entropy" of the child datasets after splitting on a particular feature.

In the context of decision trees and information gain calculation, this term represents the expected entropy of the child datasets, weighted by the proportion of instances in each child dataset relative to the parent dataset. It measures the overall uncertainty present in the child datasets after splitting on the feature.

## Example

Given the dataset, the information gain is the reduction in entropy or surprise by splitting the data based on a feature.

An email spam prediction example:

| Id  | Suspicious Words | Unknown Sender | Contains Images | Result |
|-----|------------------|----------------|-----------------|-------|
| 376 | TRUE             | FALSE          | TRUE            | spam  |
| 489 | TRUE             | TRUE           | FALSE           | spam  |
| 541 | TRUE             | TRUE           | FALSE           | spam  |
| 693 | FALSE            | TRUE           | TRUE            | ham   |
| 782 | FALSE            | FALSE          | FALSE           | ham   |
| 976 | FALSE            | FALSE          | FALSE           | ham   |

Calculate the entropy of the entire dataset:
$H(\text{D}) = - \sum_{i=1}^{n} p_i \log_2 p_i$  
$\text{Result is the target variable i.e. spam or ham}$  
where $p_i$ is the probability of the $i$th class.  
$p(\text{spam}) = \frac{3}{6} = 0.5$
$p(\text{ham}) = \frac{3}{6} = 0.5$
$H(\text{D}) = - (0.5 \log_2 0.5 + 0.5 \log_2 0.5)$  
$H(\text{D}) = - (0.5 \times -1 + 0.5 \times -1)$
$H(\text{D}) = - (-0.5 + -0.5) = 1$

Step 2 - Calculate the information gain for each feature: `Suspicious Words`, `Unknown Sender`, and `Contains Images`.

Suspicious Words = SW, Unknown Sender = US, Contains Images = CI

In the partitioning of the dataset, when SW=TRUE, there are 3 spam and 0 ham.  
When SW=FALSE, there are 0 spam and 3 ham.
Total Records of Dataset |D| = 6

Entropy for SW is

$H(SW, D) = \frac{|SW_{\text{True}}|}{|D|} H(SW_{\text{True}}) + \frac{|SW_{\text{False}}|}{|D|} H(SW_{\text{False}})$  
$H(SW, D) = \frac{3}{6} H(SW_{\text{True}}) + \frac{3}{6} H(SW_{\text{False}})$  
$H(SW_{true}) = ((\frac{3}{3} \log_2 \frac{3}{3}) + (\frac{0}{3} \times \log_2 \frac{0}{3})) = 0$  
$H(SW_{false}) = ((\frac{0}{3} \log_2 \frac{0}{3}) + (\frac{3}{3} \times \log_2 \frac{3}{3})) = 0$  
$H(SW, D) = \frac{3}{6} \times 0 \times \frac{3}{6} \times 0 $  
$H(SW, D) = 0$ bits

Entropy for US is

$H(US, D) = \frac{|US_{\text{True}}|}{|D|} H(US_{\text{True}}) + \frac{|US_{\text{False}}|}{|D|} H(US_{\text{False}})$  
$H(US, D) = \frac{3}{6} H(US_{\text{True}}) + \frac{3}{6} H(US_{\text{False}})$  
$H(US_{true}) = ((\frac{2}{3} \log_2 \frac{2}{3}) + (\frac{1}{3} \times \log_2 \frac{1}{3})) = 0.9183$
$H(US_{false}) = ((\frac{1}{3} \log_2 \frac{1}{3}) + (\frac{2}{3} \times \log_2 \frac{2}{3})) = 0.9183$
$H(US, D) = \frac{3}{6} \times 0.9183 + \frac{3}{6} \times 0.9183$  
$H(US, D) = 0.9183$ bits

Entropy for CI is

$H(CI, D) = \frac{|CI_{\text{True}}|}{|D|} H(CI_{\text{True}}) + \frac{|CI_{\text{False}}|}{|D|} H(CI_{\text{False}})$  
$H(CI, D) = \frac{2}{6} H(CI_{\text{True}}) + \frac{4}{6} H(CI_{\text{False}})$  
$H(CI_{true}) = ((\frac{1}{2} \log_2 \frac{1}{2}) + (\frac{1}{2} \times \log_2 \frac{1}{2})) = 1$
$H(CI_{false}) = ((\frac{2}{4} \log_2 \frac{2}{4}) + (\frac{2}{4} \times \log_2 \frac{2}{4})) = 1$
$H(CI, D) = \frac{2}{6} \times 1 + \frac{4}{6} \times 1$  
$H(CI, D) = 1$ bits

Entropy for SW, US, and CI is 1, 0.9183, and 1 bits respectively.

$IG(SW) = H(D) - H(SW, D) = 1 - 0 = 1 bits$
$IG(US) = H(D) - H(US, D) = 1 - 0.9183 = 0.0817 bits$
$IG(CI) = H(D) - H(CI, D) = 1 - 1 = 0 bits$
