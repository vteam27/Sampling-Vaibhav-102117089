# SamplingAssignment (102117089-Vaibhav)
## Sampling
Sampling is a method used to gather insights about a population by analyzing statistics from a representative subset, avoiding the need to analyze every individual. To address an initial dataset imbalance—763 non-fraudulent cases and only 9 fraudulent cases—an oversampling method was used. This involved creating additional instances of the minority class (fraudulent cases) to match the majority class (non-fraudulent cases), resulting in a balanced dataset combined into a single dataframe.

Various sampling techniques were employed:

- Simple Random Sampling: Choosing samples randomly from the population.
- Systematic Sampling: Selecting at regular intervals after a random start.
- Cluster Sampling: Randomly picking clusters from the population.
- Stratified Sampling: Dividing the population into subgroups based on specific criteria.
- Bootstrap Sampling: Repeatedly sampling with replacement to generate multiple samples from the original dataset.

After generating five distinct samples using these techniques, five models were applied to each sample. The accuracies of each model for a given sample are summarized in the table below:

| Sampling Technique     | Random Forest | Logistic Regression | Naive Bayes | Decision Trees | KNN |
|------------------------|---------------|---------------------|-------------|----------------|-----|
| Simple Random Sampling | 0.9870        | 0.8831              | 0.7013      | 0.9610         | 0.8701 |
| Systematic Sampling    | 1.0000        | 0.8926              | 0.7450      | 1.0000         | 0.9329 |
| Cluster Sampling       | 1.0000        | 0.9670              | 1.0000      | 1.0000         | 0.9890 |
| Stratified Sampling    | 1.0000        | 0.9030              | 0.7239      | 0.9925         | 0.9552 |
| Bootstrap Sampling     | 1.0000        | 0.9250              | 0.7500      | 0.9625         | 0.9375 |

In the table above, each row represents a sampling technique, and each column shows the accuracy achieved by each model when applied to the respective sample generated using that technique.
### The Random Forest model outperformed all others when applied to the Stratified Sampling Technique.