## Data Drift

Data drift happens when the distribution of data used to train a model changes over time. 

### Types of Data Drift

1. Covariate Shift. 

This type of data shift occurs when independent variable (features) shift between the traning and production environment. 

- Example
X-rays trained for age 20-30 years old. But the production data is for age 40-50 years old.


- Solution
Increase the robustness of the model by using data augmentation. 


2. Label Shift

Label shift is a kind of distribution drift, where the distribution of the target variable changes over time. This is more possible when the target variables are imbalanced. 

This may work well in the training but when transferred to production, the model may not perform well.


- Solution 

Validate the scores. 
a. Drift Score
b. PSI
c. Sample per class
b. bounding box per image

3. Domain Shift/ Adaptation

If there no rich training data, it will affect the model performance while deployed in production.

- Example 
The input data used to train a model is from a specific region. But the production data is from a different region.


4. Sample Selection Bias

If the data provided is not representative of the population, it will affect the model performance while deployed in production.
It will affect the robustness of the model. 

- Solution

Monitor the variance how it varies for the new input dataset. When variance is high, the model fits more on the training data and not on the test set.
If we have good amount of data we can analyze with slice based learning. 

