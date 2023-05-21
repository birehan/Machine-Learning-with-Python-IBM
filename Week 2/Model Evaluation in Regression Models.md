# Model Evaluation in Regression
After building a regression model, it is essential to evaluate its accuracy in predicting unknown cases. In this section, we will explore two evaluation approaches: "Train and Test on the Same Dataset" and "Train/Test Split." We will discuss the advantages and disadvantages of each approach and introduce metrics for assessing the accuracy of regression models.

## Train and Test on the Same Dataset
The first approach involves training the model on the entire dataset and then testing it using a portion of the same dataset. This approach provides a percentage of accurate predictions based on the known target values. However, it is important to note that this method may result in a high training accuracy but a low out-of-sample accuracy. Overfitting is a common issue where the model becomes overly trained on the dataset, leading to poor performance on new, unseen data.

## Train/Test Split
To improve out-of-sample accuracy, the train/test split approach is employed. In this approach, the dataset is divided into a training set and a testing set. The model is trained on the training set, and then the testing set is used for prediction. By evaluating the predicted values against the actual values in the testing set, we obtain a more realistic assessment of the model's performance on unknown data. It is crucial to avoid disregarding valuable data by training the model with the testing set as well.

## Evaluating Model Accuracy
To measure the accuracy of regression models, various metrics are available. One simple metric involves comparing the predicted values (denoted as y hat) with the actual values (y) in the testing set. The error of the model is calculated as the average difference between the predicted and actual values across all rows. This metric provides a basic understanding of the model's performance.

## K-Fold Cross-Validation
Another evaluation model called K-fold cross-validation addresses some of the limitations of the previous approaches. It involves splitting the dataset into multiple folds, training and testing the model on different subsets of the data, and then averaging the results. This technique helps reduce the dependency on specific training and testing datasets, resulting in a more consistent out-of-sample accuracy. However, a detailed explanation of K-fold cross-validation is beyond the scope of this course.