# Car-Policy-Claim-Prediction- Dataverse Hack
### Insurance Claim Prediction
Predict whether the policyholder will file a claim in the next 6 months or not.

### Evaluation metric
The evaluation metric for this hackathon was F1 score.

#### Approach:
+ Binary Classified Target 
+ Imbalanced Dataset
+ Almost all the features are Categorical
+ Different Encoding Technique:
   *columns that are boolean in nature so replaced the value of ‘Yes’ with 1 and ‘No’ with 0 (17 predictors)
   *columns independent of values carried one hot encoding.
   *Ordinal Categorical columns
   *columns with multiple type data(splitting of data for these features)
   *Feature Selection using different techniques : Statistical tests, scikit-learn library provides the SelectKBest
                                                 : Feature importance , inbuilt class that comes with Tree Based Classifiers

+ Scaling of data
+ SMOTE : undersampling and oversampling
+ Algorithms (f1 Score,accuracy)
    + XGBoost (0.16, 0.78)
    + RF (0.16, 0.59)
    + CatBoostClassifier (0.19,0.90)
    + XGBoost(0.17 , 0.74) , (No Overfitting with Feature Selection)
        
#### Source: https://datahack.analyticsvidhya.com/contest/dataverse/#ProblemStatement
#### AV Rank: 214/2156
