# Feature Engineering

* Agenda
  - Announcements
  - Questions about async sessions
  - Decision Trees
  - Gradient Descent

## Part 1.

* [A visual introduction to machine learning](http://www.r2d3.us/visual-intro-to-machine-learning-part-1/)

* Split Strategy

* [DecisionTreeClassifier](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html)
  -  It operates by recursively partitioning the data space based on feature values, creating a tree-like structure to predict the class label of a given input.
  -  Each internal node in the tree represents a decision based on a feature, branches represent the outcomes of the decision, and leaf nodes represent the final classification.
  -  Pro: White-box model, Works with numerical & categorical features, fast inference, not affected by non-independent features
  -  Con: Overfitting, Unstable, Incremental training difficulty

## Part 2.

* [Random Forest](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
  - A random forest is a meta estimator that fits a number of decision tree classifiers on various sub-samples of the dataset and uses averaging to improve the predictive accuracy and control over-fitting.

* W4 - Malware Simple.ipynb

* W5 - Decision Tree.ipynb

* [Naive Bayes](https://scikit-learn.org/stable/modules/naive_bayes.html)

## Class Supporting Video

4.1.1 Gradient Descent Review

4.2 Multivariate Regression

4.3 Features Overview

4.4 Feature Engineering I

4.5 Feature Engineering II

4.6 Case Study: Used Cars
