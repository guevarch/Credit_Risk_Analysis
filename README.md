# Credit_Risk_Analysis
# Overview
 - In this analysis, I used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling, the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over and undersampling using the SMOTEENN algorithm. Next, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.
# Results
 ## Oversampling
 ### Naive Random Oversampling Results
  - ![image](https://user-images.githubusercontent.com/107594143/194962048-dea78e9c-8e97-429e-8870-efbf0c5d509e.png)
  - This model has a high risk precision score of 0.01, recal score of 0.62 and an f1 score of 0.02. The low risk precision score is 1, recal score of 0.65 and an f1 score of 0.79. Lastly, it has a balanced accuracy score of 0.636. This model is quite good a predicting low-risk credit. It is not a very good model for identifying high risk scores. 
 ### SMOTE Oversampling Results
  - ![image](https://user-images.githubusercontent.com/107594143/194962104-20de291e-2618-42da-8582-4ed3657a5ffa.png)
  - This model has a high risk precision score of 0.01, recal score of 0.62 and an f1 score of 0.02. The low risk precision score is 1, recal score of 0.43 and an f1 score of 0.6. Lastly, it has a balanced accuracy score of 0.51. Compared to the previous models,t his model is not good a predicting low-risk credit. It is not a very good model for identifying high risk scores. This is the least precise, accurate and sensitve model.
 ## Undersampling
 ### ClusterCentroids
  - ![image](https://user-images.githubusercontent.com/107594143/194962169-4f286687-9959-439e-a88a-abea37b14a7d.png)
  - This model has a high risk precision score of 0.01, recal score of 0.43 and an f1 score of 0.01. The low risk precision score is 1, recal score of 0.64 and an f1 score of 0.78. Lastly, it has a balanced accuracy score of 0.51. Similar to the model prior, this model is quite good a predicting low-risk credit. It is not a very good model for identifying high risk scores.
 ## Combination (Over and Under) Sampling
  - ![image](https://user-images.githubusercontent.com/107594143/194962247-0fa40947-1a74-4cb4-bb79-4588ce4f3cf8.png)
  - This model has a high risk precision score of 0.01, recal score of 0.71 and an f1 score of 0.02. The low risk precision score is 1, recal score of 0.59 and an f1 score of 0.74. Lastly, it has a balanced accuracy score of 0.65. This model is quite good a predicting low-risk credit. It is not a very good model for identifying high risk scores.
## Ensemble Learners
### Balanced Random Forest Classifier Results
 - ![image](https://user-images.githubusercontent.com/107594143/194962398-75ff96c4-2953-4b6e-82f2-f584c601e14f.png)
 - This model has a high risk precision score of 0.01, recal score of 0.67 and an f1 score of 0.07. The low risk precision score is 1, recal score of 0.91 and an f1 score of 0.95. Lastly, it has a balanced accuracy score of 0.78. This model is quite good a predicting low-risk credit. Compared to the other models, it is better for identifying high risk scores.
### Easy Ensemble AdaBoost Classifier Results
 -![image](https://user-images.githubusercontent.com/107594143/194962473-fa5e7ece-62b5-4379-8bf3-8468054afce6.png)
 - This model has a high risk precision score of 0.07, recal score of 0.9 and an f1 score of 0.14. The low risk precision score is 1, recal score of 0.9 and an f1 score of 0.97. Lastly, it has a balanced accuracy score of 0.91. This model is quite good a predicting low-risk credit. Compared to the other models, it is better for identifying high risk scores.

# Summary

In this analysis, I used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling, the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over and undersampling using the SMOTEENN algorithm. Next, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

Easy Ensemble AdaBoost Classifier had the best accuracy score vs the rest of the tests, In this case, the model's accuracy score was 0.916, meaning that the model was correct 91.6% of the time. The same model has the best f1 score of 0.14 for high risk and a 0.97 for low risk.

All the models have a very good low-risk precision score, which means that they can predict low-risk credit scores well. On the other hand, the best model for predicting high-risk scores is Easy Ensemble AdaBoost Classifier, but not by much (0.07 vs 0.01 for the others). 

The model with the best sensitivity score is the Easy Ensemble AdaBoost Classifier with a high risk score of 0.9 and and low risk score of 0.94. The least accurate model is the ClusterCentroids with a high risk score of 0.59 and a low risk score of 0.43. A highly sensitive test means that there are few false negative results.

For this type of data and results, Easy Ensemble AdaBoost Classifier is the better model for predicting low/high risk credit scores.

