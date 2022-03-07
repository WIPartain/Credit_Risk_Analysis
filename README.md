# Credit_Risk_Analysis
## Overview

For this challenge, we created and applied several machine learning models to determine the overall credit risk of a set of data. We will evaluate how well these models work and whether or not we should apply them to determine credit risk

The methodologies we used were:
oversampling the data through RandomOverSampler and SMOTE algorithms.
Undersampling the data through the ClusterCentroids algorithm.
We also used an ensemble approach of oversampling and undersampling using the SMOTEENN method as well as BalancedRandomForestClassifier and EasyEnsembleClassifier.

## Analysis

### RandomOversampler Method

![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/Naive_Random_Sampling.png)

The balanced accuracy score is roughly 63%.
The high risk precision is about 1% only with 55% sensitivity which makes a F1 of 2% only.
The large population of low risk credit boosts its precision to almost 100% with a sensitivity of 70%.

### Smote Method

![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/Smote_Oversampling.png)
Much like the previous model, the balanced accuracy score is roughly 63% as well.
The high risk precision is about 1% only with 60% sensitivit yand a F1 of only 2% .
Again, the vast number of low risk credit makes the low risk precision almost 100% with a sensitivity of 65%.

### ClusterCentroids Method

![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/Cluster_Centroids.png)

The balanced accuracy score is slightly over 50%.
The high risk precision is still 1% only with 49% sensitivity which leads to a F1 of 1%.
The low risk precision is 100%, and the low risk sensitivity is only 42%.

### Smoteenn Model

![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/Smoteenn.png)

The balanced accuracy score is over 66%.
The high risk precision is still 1% only with 71% sensitivity which makes a F1 of only 2%.
Again, the low risk precision is 100%, and the low_risk sensitivity is 62%.

### BalancedRandomForestClassifier Model

![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/Balanced_Random_Forest_Classifier.png)

The balanced accuracy score greatly improved over 81%.
The high_risk precision is still low at 4% only with 71% sensitivity which makes a F1 of only 8%.
Low risk precision is still 100%, and the low risk sensitivity is now 91% with 100% presicion.

### EasyEnsembleClassifier Model

![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/AdaBoost_Classifier.png)

Now, the balanced accuracy score is at its highest at about 93%.
The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of 14%.
Low risk percentage is again 100%, and the low risk sensitivity is now 94% with 100% presicion.

## Summary

Each of these models show perfect precision for determining low credit risk and almost no precision in determining high credit risk. The BalancedRandomForestClassifier and EasyEnsembleClassifier models show the highest balanced accuracy scores, and they also contained the highest sensitivity and F1 scores.  However, with low precision for high risk credit, there is a great chance that low risk credit could be identified as high risk.  Since that is the case with all 6 models.  It is hard to recommend the usage of any of these methods to determine risk.  
