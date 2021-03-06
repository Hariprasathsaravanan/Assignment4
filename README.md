# Assignment4
Support-Vector-Machine-Social-Network-Ads
Using Support Vector Machine (SVM) with linear and non-linear kernel to make the prediction and compare the difference

Problem
Suppose a company is going to launch a new campaign for their new brand of car and want to know which category of people are likely to buy their brand new car so they can have the ads that target those peoples. For this they contacted a social network advertising company which have the data from another similar successful campaign. Now, they want to make a model which helps achieve their goal.

Dataset
The dataset contains 400 entries which contains the userId, gender, age, estimatedsalary and the purchased history. The matrix of features taken into account are age and estimated salary which are going to predict if the user is going to buy new car or not(1=Yes, 0=No).

Solution
First the pre-processing of data is done and then the prediction is done using Support Vector Machine (SVM) and kernel SVM. The confusion matrix and visualization clearly shows the prediction made by both models and the difference.. The dataset is split into 75/25 ratio (training set = 0.75 & test set = 0.25).

The confusion matrix with SVM (linear kernel) shows that our model predicts 90 correct and 10 wrong decisions which shows 90% accuracy.

cm_svm

The confusion matrix with kernle SVM shows that our model predicts 93 correct and 7 wrong decisions which shows 93% accuracy.

cm_kernel_svm

The data visualization of the training set and test set is given below. As in the svm the kernel was selected as linear, the graph is linear with a straight line whereas kerel svm deals with non-linear data, the graph is non-linear (curve). The green dots shows the people buying the car whereas red dots shows the people not buying the car. The green dots on the green region shows the true positive whereas the red dots on the red region shows the true negative. The wrongly classified are the green dots in the red region (false negative) and the red dots in the green region (false positive).

SVM (Training set)

SVM (Test set)

Kernel SVM (Training set)

Kernel SVM (Test set)

Conclusion
From the two models, it is clear that for this dataset, the non-linear kernel (default) is better than the linear kernel svm as it predicts more accurately and the graph illustrates it clearly.
