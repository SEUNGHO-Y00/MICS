# KNN, Decision Trees, and Ensembles

* Agenda
  - Questions about async sessions
  - kNN code examples
  - Code: Nearest Neighbor classifier implementation
  - Code: Going through Q1 & Q1 of Project1

## Part 1.

Using sklearn and k-NN to detect credit card fraud
* [Dataset description](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

W4 - Credit Card KNN.ipynb
* [Preprocessing and Normalization](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.normalize.html)
* [KNeighborsClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)
* Confusion Matrix = A table that is often used to describe the performance of a classification model on a set of test data for which the true values are known.
  - In machine learning, a confusion matrix is a table that visually summarizes the performance of a classification model by comparing its predicted labels to the actual labels, highlighting where the model makes mistakes and what types of errors it's making.
* Imagine a model predicting whether an email is spam or not spam.

|                 | Predicted: Spam     | Predicted: Not Spam |
| --------------- |:-------------------:| -------------------:|
|Actual: Spam     | TP (True Positive)  | FN (False Negative) |
|Actual: Not Spam | FP (False Positive) | TN (True Negative)  |

## Part 2.

* Naive Bayes
  - Pro: Computationally Fast, Simple to implement, Works well in high dimensions (relatively)
  - Cons: Relies on independence assumption and will perform badly if this assumption is not bad

* [An Introduction to Bayesian Modeling](https://naive-bayes-notebook.vercel.app/)
Pr(spam|words) = (Pr(words|spam)*Pr(spam))/Pr(words)

* [pandas.get_dummies](https://pandas.pydata.org/docs/reference/api/pandas.get_dummies.html)

## Class Supporting Video

3.1 Review

3.2 Nearest Neighbors

3.3 Decision Trees

3.4 Decision Tree Learning

3.5 Decision Tree Example

3.6 Trees to Forests
