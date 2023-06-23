# Hari-Prakash_Portfolio
# Health Insurance Lead Prediction

## Abstract:

The company wants to increase its revenue by cross-selling health insurance to its existing customers
by collecting surveys to understand their requirements and suggest premium policies based on the survey
feedback. Once these leads are acquired, the sales advisors approach them to convert, and thus the company can sell proposed health insurance to these leads in a more efficient manner.

## Problem Statement:

The company needs your help in building a model to predict whether the person will be interested
in their proposed Health plan/policy given the information about Demographics (city, age, region, etc.) Information regarding holding policies of the customer Recommended Policy Information.

## Data Dictionary:

This organization that provides insurance to their customers wants to cross-sell health insurance to their existing customers hence the
dataset obtained from this organization is used for Health Insurance Lead Prediction.

![Images](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/c5260b5d-730e-47b0-8d53-77c7bfc4f940)

*From the above code we can see that there are 50882 records and 14 attributes in the dataset.

## Data Description:

![images2](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/41840e5a-b418-4005-9d39-9002ff52fb85)
![image3](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/193fd295-4c40-4a54-8695-3b0f829dd323)

## Data Pre-processing:

• Pre-Processing Data Analysis (count of missing/ null values, redundant columns, etc.)

• The dataset has missing values in most of the columns.

## Missing Value Analysis:

![image4](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/abee1dfa-85fb-42f1-8f14-b85c5302285e)

*We have null values in above mentioned three variables.


## Before missing value treatment:

![image5](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/a88c76f3-e617-404c-8379-87f074e515a6)

*The above figure shows missing values in the dataset.

## After Missing value treatment:

![image6](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/c83339a2-148e-4f3c-b2f8-dc8555c32c3c)

## Exploratory Data Analysis:

## Accommodation Type:

In the below plot, each distribution of Accommodation type w.r.t target variable is shown.

![image7](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/100ae84c-aff7-4875-87ab-f52efd05b4b7)

From the above plot, we can say that there are more people with their own accommodation. There are around 20000 people under-owned who do not show interest in recommended policy.
Around 6000 people with owned accommodation have shown interest in the policy. Whereas for people with accommodation type rented who show interest in policy is around 5000 and who do not show interest is around 17500.

## Holding Policy Type:

![image8](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/018ce4a3-21e7-408a-bcb6-49598c43b466)

There are 4 different types of policies provided by the company XYZ. Most of the customers prefer policy 3. Among policies 1, 2 & 4, people prefer policy 1 followed by policy 2, and policy 4 is the least preferred.

## Marital Status:

![image9](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/985fbde4-94ee-436a-9eb8-5d9570bcbded)

From the above plot, we can say that there are more customers unmarried. More than 30000 unmarried customers do not prefer the recommended policy, whereas around 10000 unmarried customers have shown interest in the policy. More than 5000 married customers have not shown interest in recommended policy, while around 2000 married customers prefer taking the recommended policy.

## Average Age vs Policy Premium:

![image10](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/d4a0ec00-07be-477d-b551-1ee53b3045a9)

The distribution of Average age between Upper age & Lower age w.r.t Recommended
policy premium has a positive correlation. As the Average age increases, the recommended policy premium also increases. We can see that, the response for the recommended policy is more scattered throughout the Average age.

## Feature Engineering:

Convert to numerical: Holding policy duration

Feature engineer long-term customers. Convert '14+' to '15'/ convert to numerical.

## Feature Selection:

![image11](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/31195b84-6658-43a0-8625-6dcf85ebea98)

*Features 'Accommodation Type', 'Reco Insurance Type', and 'Is Spouse' will be converted to binary (0 and 1).

## Train – Test Split:

![image12](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/705130c9-d520-4be0-8d93-ea21453679d2)

*Here we split the data into train and test sets, where 70% of the data is used for training and 30% data is used for testing with a random seed value of 0. The training dataset is used to train the model for prediction. The test dataset is used to test the model’s efficiency of prediction.

## Handling Imbalance Data (Resampling Technique):

![image13](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/c7dac73f-92bc-4113-a58f-3ce5ea152c8e)

*When observation in one class is higher than the observation in other classes then there exists a class imbalance. We can clearly see that there is a huge difference between the data set. To solve this issue we use the resampling technique.

## Model selection:

![image](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/3aed88a5-26af-4fda-b10a-5089947fc406)

From the above models created, we have achieved considerable results in models such
as Random Forest classifier, Gradient Boost, and XG Boost Classifier.

• Out of which Random Forest seems to be giving better results when compared to other
models with an Accuracy of 88%.

• We have Recall, Precision, F1 score, and AUC along with the ROC curve supporting our best-fit
model.

• Hence considering all the validation metrics along with scores, we choose Random Forest
as our best-fit model in classifying records.

## Feature Importance for Better Visualization:

![image](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/68a96350-f626-4575-9c50-3982878ab849)


## Validation:
Classification report:

![images16](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/58cd1327-f328-4971-a6eb-18808ba98868)

*The above classification report gives us the scores of the Random Forest model.

## ROC Curve:

![image](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/e9864bb8-2a1c-4fbc-8b25-910503b0d12e)

*The above ROC curve which is plotted between TPR (True Positive Rate) vs FPR (False Positive
Rate) lies far away from the axis.

*Due to the far presence of the ROC curve from the axis, we could say that the acquired AUC score
supports our Random forest model as the best-fit model.

## Confusion Matrix:

![image](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/5cd744f5-f83c-46c7-88ad-04a8d2841521)

*The above confusion matrix gives us the values for True Positive, False Positive, Recall, F1-score, Accuracy, and Specificity.

*With these validation metrics, we can validate our best-fit model.

## Recommendations:

Recommended Premium:

![image](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/7be933db-3f26-4e24-9f39-b9e823c1c54a)

![image19](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/eabf978d-6c6b-47dd-97a2-7500284cb4e5)

We suggest targeting customers whose recommended premium is between 15000 – 30000.

Reco Policy Category:

![image](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/0cbf1a81-bcd6-447f-8c35-9bb54a784ddc)

Positive to total response ratio

Policy category: 1

Policy category: 11

Policy category: 5

## Based On City Code:

![images21](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/62577edf-373f-4803-88e5-4a80f34e2a4e)

![image22](https://github.com/HariPrakash1504/Hari-Prakash_Portfolio/assets/113451743/244febd4-5aae-45d5-a169-f86d0b4718ea)






































