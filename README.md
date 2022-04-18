# Credit_Risk_Analysis

## Project overview

In this project I am utilizing machine learning in order to develop a model that assists a bank in predicting the outcome of personal loans with the possibility of default. I used Python to build machine learning models to better predict credit risk and potential bad loans. Since the sample groups of bad loans are considerably smaller than good loans, I had to use both imbalanced-learn and scikit-learn libraries to resample the groups in order to make the models more accurate. RandomOverSampler, SMOTE, ClusterCentroids, and SMOTEENN algorithms are applied in an attempt to make the analysis more accurate. BlaancedRandomForestClassifier Model and the EasyEnsembleClassifier Model are used in the last set of analysis. Finally, all models are assessed on their effectiveness and I determine whether they should be used to predict credit risk. 

## Results

### Deliverable 1

-Originally the pool of high risk applications were significantly small compared to the number of low risk applications. Applications from the high risk class were added to the training set in order to make the two equal and allow for more balanced analysis. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable1.1.png)

-In this model the balanced accuracy score was 50.49%. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable1.2.png)

-High Risk precision rate was 33%, with a recall of 1% and an F1 score of 2%.

-Low Risk precision rate was 99%, a recall of 99% and an F1 score of 99%.

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable1.3.png)
![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable1.4.png)

-Utilizing the SMOTE method the smaller, high risk application group size is increased to match the low risk application group size by selecting applications that are close in feature space rather than randomly as done in the previous method. This time the balanced accuracy score increased to 66.2%.  

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable1.5.png)

-High risk applications had a precision score of only 1%, whith a recall of 63% and an F1 score of 2%, just as it had been in the previous model. 

-Low risk applications had a slightly higher precision score of 100%, a recall of rate of 69% and an overall F1 score of 82%. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable1.6.png)
![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable1.7.png)

### Deliverable 2

-For these next models I am focusing on undersampling in which cluster centroids are used to create synthetic data points representative of the clusters created. Equal sized groups from this process are created in which 246 data points are in each. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable2.1.png)

-In this model the balanced accuracy score was 66%.

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable2.2.png)

-The high risk group has a 1% precision score, with a recall of 69% and an F1 of 1%.

-The low risk group has a 99% precision score, with a recall of 40% and an overall 56% F1 score. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable2.3.png)
![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable2.4.png)

-In this next model I am utilizing SMOTEENN that uses a hybrid approach of both undersampling and oversampling in order to create comparable group sizes for analysis. In this case, high risk and low risk both have high numbers, with high risk coming in higher, but still mostly similar size. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable2.5.png)

-The balanced accuracy score is 54.47% for this first model. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable2.6.png)

-The high risk group has a 1% precision rate, a recall of 72%, and an F1 score of 2%.

-Low risk group has a 100% precision rate with a recall rate of 57% and an overall F1 score of 73%. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable2.7.png)
![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable2.8.png)

### Deliverable 3

-In deliverable 3 I am using ensemble classifiers to reduce bias in the sample groups. Initially the BalancedRandomForestClassifier is used and the balanced accuracy score is 75.55%, the highest score yet. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable3.1.png)

-The high risk group has a 3% precision rate, a recall rate of 63%, and an F1 score of 6%. These are all the highest scores yet for the high risk group. 

-The low risk group has a precision score of 100%, a recall of 88%, and a F1 score of 93%. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable3.2.png)
![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable3.3.png)

-In the final mode I am using the EasyEnsembleClassifier Model and the results are significantly stronger. This model produces a balanced accuracy score of 93.16%. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable3.4.png)

-The high risk group's precision score is 9%, the recall is 92%, and the F1 score is 16%. 

-The low risk group has a precision score of 100%, a recall of 94% and an F1 score of 97%. 

![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable3.5.png)
![alt text](https://github.com/bwengerDU/Credit_Risk_Analysis/blob/main/Module-17-Challenge-Resources/Deliverable%20Images/Deliverable3.6.png)

## Summary

Below is the overview of how each model performed for high risk applications. 

-RandomOverSampler: 50.49% balanced accuracy score, 33% precision score, 1% recall, and F1 of 2%.  

-SMOTE: 66% balanced accuracy score, 1% precision, 63% recall, and 2% F1. 

-ClusterCentroids: 66% balanced accuracy score, 1% precision, 69% recall, and 1% F1. 

-SMOTEENN:54.47% balanced accuracy score, 1% precision, 72% recall, and an F1 of 2%. 

-BalancedRandomForestClassifier: 75% balanced accuracy score, 3% precision, 63% recall, and an F1 of 6%. 

-EasyEnsembleClassifier: 93.17% balanced accuracy score, 9% precision, recall of 92% and an F1 of 16%. 

After running the testing across all 6 methods, the EasyEnsembleClassifier method was the best predictor. It produced a balanced accuracy score of 93%, a precision rate of 9% for high risk & 100% for low risk, recall scores of 92% for high risk & 94% for low risk, and an F1 score of 16% for high risk & 97% for low risk. The model may not be full-proof, but it does perform analysis at a very high level of accuracy. The bank must decide on the acceptable level of error, which is estimated around 7% with this model. 
