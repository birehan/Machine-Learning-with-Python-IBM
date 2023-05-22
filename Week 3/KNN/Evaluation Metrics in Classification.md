# Evaluation Metrics for Classifiers

This repository provides an overview of evaluation metrics used to assess the performance of classification models. Evaluation metrics play a crucial role in model development as they offer valuable insights into areas that require improvement. This guide focuses on three key metrics: Jaccard index, F1-score, and Log Loss.

## Jaccard Index

The Jaccard index, also known as the Jaccard similarity coefficient, measures the accuracy of a classifier. It compares the predicted labels by the classifier (y_hat) with the true labels (y) in the dataset. The index is calculated as the size of the intersection divided by the size of the union of the two label sets.

Jaccard Index = |y ∩ y_hat| / |y ∪ y_hat|

## Confusion Matrix

A confusion matrix provides a detailed view of a classifier's accuracy by illustrating the correct and incorrect predictions in comparison with the actual labels. Each row in the matrix represents the actual/true labels in the test set, while the columns represent the predicted labels by the classifier. It allows us to calculate metrics such as precision and recall for each class, based on the count of true positives (TP), false negatives (FN), true negatives (TN), and false positives (FP).

## Precision, Recall, and F1-Score

Precision measures the accuracy of a class label prediction, while recall represents the true positive rate. These metrics can be calculated using the counts from the confusion matrix:

Precision = TP / (TP + FP)

Recall = TP / (TP + FN)

The F1-score is the harmonic average of precision and recall, providing a balanced evaluation metric that considers both precision and recall. It reaches its best value at 1, indicating perfect precision and recall.

F1-score = 2 * (Precision * Recall) / (Precision + Recall)

## Log Loss

In some cases, classifiers provide the probability of class labels instead of the labels themselves. Logarithmic loss, also known as Log Loss, is an evaluation metric used when the predicted output is a probability value between 0 and 1. It measures the distance between each prediction and the actual label, with smaller values indicating better accuracy.

Log Loss = -(1/N) * Σ [y * log(y_hat) + (1-y) * log(1-y_hat)]

Here, N is the number of samples in the test set, y is the true label (0 or 1), and y_hat is the predicted probability.

Please note that both the Jaccard index and F1-score can be utilized for multi-class classifiers as well. This repository focuses on binary classifiers, but the concepts can be extended to handle multi-class classification scenarios.