# Sampling_Assignment
This repository contains the solution for the Sampling Assignment, focusing on evaluating the impact of different sampling techniques on machine learning models.

Overview:

*Dataset:

Balanced the given dataset using class-balancing techniques.

*Sampling Techniques:

Applied five techniques:

1.Simple Random Sampling: Selecting random subsets.

2.Systematic Sampling: Picking every nth data point.

3.Stratified Sampling: Ensuring class representation in samples.

4.Cluster Sampling: Selecting random groups of data points.

5.Oversampling/Undersampling: Adjusting class distributions by either duplicating minority class records or reducing majority class records.

*Machine Learning Models:

Five different machine learning models were used to evaluate the impact of various sampling techniques on model performance. These models were chosen to represent a diverse range of algorithms, from simple linear models to more complex ensemble methods, providing comprehensive insights into sampling effects. Below is a brief description of each:

Decision Tree:

A tree-based algorithm that splits the dataset into subsets based on feature conditions.
Works well with imbalanced datasets but can overfit smaller or unbalanced samples.
Provides interpretable results, making it a baseline for comparison.

Logistic Regression:

A linear model for binary or multiclass classification.
Sensitive to imbalanced data, making it an interesting case for evaluating the effectiveness of balancing techniques like Oversampling or Stratified Sampling.
Suitable for datasets where the relationship between features and target is linear.

Gradient Boosting:

An ensemble method combining weak learners (Decision Trees) to improve performance.
Configured with 100 estimators, learning rate of 0.1, and maximum tree depth of 3.
Highly effective at handling complex relationships and moderately imbalanced data, but performance can vary depending on the quality of samples.

k-Nearest Neighbors (k-NN):

A distance-based algorithm that classifies data based on the majority class of its nearest neighbors.
Sensitive to data distribution and class imbalance, where sampling techniques significantly affect performance.
Works well with well-distributed and balanced data.

Support Vector Machine (SVM):

A powerful algorithm that finds an optimal hyperplane to separate classes.
Performs best with balanced datasets, where class overlap is minimized.
Particularly sensitive to data scaling and sampling quality, making it a key model to assess the effects of techniques like Stratified Sampling.

*Findings:

->Sampling techniques significantly impacted model performance.

->Stratified sampling and oversampling yielded higher accuracy across most models.

->Model M3 performed consistently better with Sampling1 and Sampling2.

->Sampling3 and Sampling5 techniques were less effective for some models, indicating sensitivity to data preparation.

->The maximum accuracy in the case of sample 3 using decision tree .But this is not practical ,means that our model is overfitting in this case. It may seem to work amazingly with train data but fails to give 
good results with train data.Other than that, the best models for each samples are:

sample1: logistic regression

sample2: gradient boosting

sample3: logistic regression

sample4: decision tree,logistic

sample5: Gradient boosting
