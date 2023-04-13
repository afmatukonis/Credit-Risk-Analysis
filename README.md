# Credit-Risk-Analysis

**Overview**

The purpose of this module was to use supervised machine learning to predict credit risk. Credit risk is an inherently unbalanced classification problem we used undersampling, oversampling, and a combination of both to find a model that would best predict credit risk. To oversample we used RandomOverSampler and SMOTE algorithms, and for undersampling we used the ClusterCentroids algorithm. 

**Results**

The following is the balanced accuracy score and precision /recall for determining high risk lones for each of the models used.

* RandomOverSampler:

    * Balanced accuracy score: 0.653
    
    * Precision: 0.01
    
    * Recall: 0.63

* SMOTE:

    * Balanced accuracy score: 0.651
    
    * Precision: 0.01
    
    * Recall: 0.64

* ClusterCentroids:

    * Balanced accuracy score: 0.651
    
    * Precision: 0.01
    
    * Recall: 0.61

* SMOTEEN:

    * Balanced accuracy score: 0.529
    
    * Precision: 0.01
    
    * Recall: 0.69

* BalancedRandomForestClassifier:

    * Balanced accuracy score: 0.788
    
    * Precision: 0.04
    
    * Recall: 0.67

* EasyEnsembleClassifier:

    * Balanced accuracy score: 0.925
    
    * Precision: 0.07
    
    * Recall: 0.91

**Summary**

After running the different models we found that we had very low precision but high recall. Because the data was extreemly unbalanced we had many more false positives that caused the precision to be low. The best performing model was the EasyEnsembleClassifier which had 93% of classified cases classified correctly and a 0.07 precison. Meaning that 7% were actually high risk. It had a recall of 0.91. Out of all the models used this one returned the best resutls. 
