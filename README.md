# Differentiated Thyroid Cancer Analysis

## About
This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on Differentiated Thyroid Cancer Recurrence from UCI Machine Learning Repository. For detailed walkthrough, please view the source code in order from:

1. [Data Preparations] - Link
3. [Data Visualization] - Link
4. [Data Splitting] - Link
5. [ML: Decision Tree Classification] - Link
6. [ML: Random Forest Classification and K-Clustering] - Link
  
## Contributors
- Claire Chia Wan Ni (CLAI0011@e.ntu.edu.sg, @clairewanni): 
  - Exploratory Data Analysis
  - Data Cleaning
  - Insights
  
- Narmandakh Nomt (nomt001@e.ntu.edu.sg, @nomtt):
  - Machine Learning
  - Data Splitting
  - Recommendations

## Problem Definition

### Rationale
Differentiated Thyroid Cancer (DTC), the most common thyroid cancer type, makes up over 90% of all cases. A key challenge is its unpredictability. Despite treatment, up to 30% of patients face recurrence. Current risk assessments rely on physician experience and generalized clinical guidelines, which may miss individual-specific factors affecting recurrence.

### Problem Statement
- __Are we able to predict recurrence of Thyroid Cancer based on individuals’ physical attributes?__
  - Which model would be the best to predict it?

## Models Used
- Decision Tree Classifier
- Random Forest Classifier
- K-means clustering

## Insights
- Initial treatment response, is the most influential factor in likelihood of recurrence. if some cancer cells survive the initial treatment, they can eventually grow and lead to a recurrence. Therefore, patients who had severe responses should be given rigorous follow-ups.
- Patients presenting with lymphatic spread (Adenopathy) or aggressive tumor types should be considered high-risk from the beginning, even before recurrence signs emerge.
- Recurrence risk increases with age. Greater monitoring and intervention should be prioritized for older individuals, even if their initial diagnosis appears mild.
- While more females were diagnosed overall, males experienced more severe complications and higher recurrence, suggesting that more rigorous follow-up protocols might be necessary for male patients.
- Although most patients were non-smokers, smokers consistently showed poorer recovery and higher recurrence rates, hence smoking as a lifestyle factor may warrant tighter follow-up treatments or additional counseling during and after treatment.

## Conclusion
- We were able to develop a predictive model for Differentiated Thyroid Cancer Recurrences using the Random Forest trained on Dataset X3 with tuned hyperparameters.
- Through iterative improvement from training 15 machine learning models, we successfully increased the accuracy of our model from as low as 66% at the beginning to 98% eventually.

## What did we learn from this project?
- Visualising and managing categorical data
- Decision Tree Classification, Random Forest Classification (LEARNT), k-clustering (LEARNT)
- Understanding and usage of Accuracy and Hyperparameters

## Future Improvements
- Improve data balance
  -  While our model performed well, its predictive power could be further improved with more balanced datasets and additional clinical features like post-operative hormone levels.
- Explore time-based models
  - Since recurrence can happen years after treatment, future models could benefit from time-series analysis or longitudinal tracking to better capture recurrence timing.
- Embed model outputs into clinical settings
  - With minimal tuning, the model can serve as a real-time tool to help clinicians identify high-risk patients—such as older males with aggressive tumors—and customize their follow-up plans .

## References
-https://archive.ics.uci.edu/dataset/915/differentiated+thyroid+cancer+recurrence 
- https://www.geeksforgeeks.org/random-forest-regression-in-python/
- https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html
