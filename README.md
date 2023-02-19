# sampling-assignment
# Comparing Sampling Techniques for 5 Machine Learning Models

## Introduction

This project explores the effectiveness of different sampling techniques for creating a balanced dataset for a machine learning model. The dataset used is initially unbalanced, so random over-sampling and under-sampling techniques are used to create a balanced dataset. Five different sampling techniques are then applied to this balanced dataset, and the accuracies of the resulting samples are compared using five different machine learning models.

## Sampling Techniques

The following five sampling techniques were used in this project:

1. **Simple Random Sampling:** A basic sampling technique where each data point in the dataset has an equal probability of being selected in the sample.

2. **Stratified Sampling:** A sampling technique where the population is divided into subgroups (strata) based on a specific characteristic, and samples are taken from each stratum in proportion to the population.

3. **Systematic Sampling:** A sampling technique where every nth element in the population is selected for the sample, with n being a fixed interval.

4. **Cluster Sampling:** A sampling technique where the population is divided into clusters, and a sample of clusters is randomly selected. Then, all members of the selected clusters are included in the sample.

5. **CQuota Sampling:** A non-probability sampling technique where the sample is chosen based on its convenience to the researcher.

## Comparison Table

The table below shows the accuracies of each sampling technique on five different machine learning models. The dataset used for all models is a balanced version of the original unbalanced dataset using random over-sampling and under-sampling techniques.

| Sampling Technique | Simple Random Sampling | Systematic Sampling| Stratified Sampling| Cluster Sampling | Quota Sampling |
|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|:---------------:|
| Random Forest Classifier | 0.974193548387096 | **1.0000** | 0.974025974025974 | 0.993548387096774 | 0.974025974025974 |
| Ridge Classifier | 0.978448275862069 | **1.00000** | 0.982758620689655 | 0.987068965517241 | 0.982758620689655 |
| Dummy Classifier | 0.974193548387096 | **1.00000** | 0.974025974025974 | 0.993548387096774 | 0.974025974025974 |
| Linear Discriminant Analysis | 0.967741935483871 | **1.00000** | 0.987012987012987 | 0.993548387096774 | 0.974025974025974 |
| SVM | 0.967741935483871 | **1.00000** | 0.974025974025974 | 0.993548387096774 | 0.974025974025974 |

Based on these results, it can be concluded that Systematic Sampling performs the best on all five models. Simple random sampling performs the worst on all five models. The other sampling techniques have varying performance depending on the model. The model which gives the best accuracy for all 5 samples is SVM.

## Conclusion

It is recommended to use systematic sampling for this dataset, as it consistently gives the best performance across all models. However, other sampling techniques may be worth considering for different datasets or models.
 
