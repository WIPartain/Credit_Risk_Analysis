# Credit_Risk_Analysis
## Overview

## Analysis

### RandomOversampler Method

![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/Naive_Random_Sampling.png)

The balanced accuracy score is 65%.
The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

### Smote Method

![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/Smote_Oversampling.png)
The results are pretty similar to the previous model.
The balanced accuracy score is 64%.
The high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.
Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 66%.

### ClusterCentroids Method
![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/Cluster_Centroids.png)
Here the balanced accuracy score is down to about 52%.
The high_risk precision is still 1% only with 63% sensitivity which makes a F1 of 1%.
Due to the high number of false positives, the low_risk sensitivity is only 40%.

### Smoteenn Model

![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/Smoteenn.png)
The balanced accuracy score is about 62%.
The high_risk precision is still 1% only with 68% sensitivity which makes a F1 of only 2%.
Due to the high number of false positives, the low_risk sensitivity is 57%.

### BalancedRandomForestClassifier Model

![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/Balanced_Random_Forest_Classifier.png)
The balanced accuracy score improved to about 79%.
The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

### EasyEnsembleClassifier Model

![](https://github.com/WIPartain/Credit_Risk_Analysis/blob/main/images/AdaBoost_Classifier.png)
Now, the balanced accuracy score is high to about 93%.
The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.
## Summary
