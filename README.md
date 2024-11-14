Vertebral Column Classification with K-Nearest Neighbors
This project demonstrates classification on a biomedical dataset, focusing on the Vertebral Column Data Set. The dataset includes six biomechanical attributes derived from the shape and orientation of the pelvis and lumbar spine, used here to classify vertebral conditions as Normal (Class 0) or Abnormal (Class 1).

This work was completed as part of Homework 1 for the DSCI 552 course, highlighting various concepts in classification, distance metrics, and model evaluation.

Table of Contents
Project Overview
Data Preprocessing
Classification Using K-Nearest Neighbors
Distance Metrics
Weighted Voting
Results and Analysis
Requirements
Project Overview
The goal of this project is to perform binary classification on the Vertebral Column Data Set. Using K-Nearest Neighbors (KNN) as the primary classifier, the project explores various configurations and distance metrics to evaluate their impact on model performance.

Data Preprocessing
The Vertebral Column Data Set was split into a training and test set. Each class was visualized:

Scatterplots and Boxplots were created for each feature to compare distributions across classes.
The training set consisted of 70 samples of Class 0 and 140 samples of Class 1, with the remaining data for testing.
Classification Using K-Nearest Neighbors
The KNN model was implemented with the Euclidean distance metric, and performance was evaluated with:

A range of k values.
Confusion matrix, true positive rate, true negative rate, precision, and F1-score for the optimal k.
Distance Metrics
Various distance metrics were evaluated to assess their effect on classification:

Minkowski Distance: Manhattan Distance (p=1), Log-scaled variations, and Chebyshev Distance.
Mahalanobis Distance: Addressed covariance concerns, transforming features into a linear subspace when required.
Weighted Voting
The KNN voting mechanism was modified to include distance-weighted voting, giving greater influence to nearer neighbors. Weighted voting was tested with:

Euclidean, Manhattan, and Chebyshev distances.
The optimal k for each configuration.
Results and Analysis
The project concludes with a summary of the optimal parameters and configurations that achieved the lowest error rates, including:

Optimal k value.
Best distance metric and weighted voting configuration.
Learning curves showing the relationship between training set size and test error rate.
Requirements
The project requires:

Python
Libraries: numpy, pandas, matplotlib, sklearn