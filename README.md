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




























