# Assignment Discussion
## Exploratory Data Analysis
From the output feature 'Class', it is clear that the following is a classification problem. The Credit Card dataset consisted of 772 entries out of which 9 were classified as positive and rest were classified as negative. \
It is clear that the dataset is highly imbalanced. Oversampling could be employed for balancing out the dataset. \
There are no null values or duplicate entries. All the features are numeric and continuous.
## Size of Sample:
### The size of the sample was calculated using the following formula:-
$$
n = Z^2 \cdot p \cdot (1-p) / E^2
$$
### Where, 
$$
n = \text{size of sample} \\
Z = \text{z-score of sample} \\
p = \text{std. deviation} \\
E = \text{margin of error}
$$

## Creating samples:
### In total of 4 samples of size 385 are created using sampling the following sampling techniques-
1. Simple Random Sampling
2. Systematic Sampling
3. Cluster Sampling
4. Bootstrap Sampling
### Each of the samples was scaled using the z-score normalization and then split into training and testing sets in the ratio 8:2.
$$
\begin{align*}
    Z = (x-\mu)/\sigma
\end{align*}
$$
## Model Selection
### The following classification models have been employed :-
1. Logistic Regression
2. KNN
3. Naive Bayes
4. Decision Trees
5. Random forest classifier

### Following are the accuracy scores for the models for each sample-
|          | Model 1 | Model 2 | Model 3 | Model 4 | Model 5 |
| ------   | ------ | ------- | ------- | ------- | ------- |
| Sample 1 |  0.88  | 0.87  | 0.83  |   0.93   |    0.97     |
| Sample 2 | 0.90   | 0.87  | 0.84  |   0.99   |    1 (overfit)    |
| Sample 3 | 0.92   | 0.87  | 0.79  |   0.97   |     0.98    |
| Sample 4 | 0.96   | 0.94  | 0.87  |   0.98   |      1 (overfit)   |

#### In general, Bootstrap sampling provides higher accuracy and the best performing model is Random Forest Classifier.