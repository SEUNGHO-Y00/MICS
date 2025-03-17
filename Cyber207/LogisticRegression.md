# Logistic Regression

* Agenda
  - Questions about async sessions
  - Feature Engineering
  - Gradient Descent

## Part 1.

* Generating features from raw data
  - Types of features: Non-continuous, Continuous

* [CountVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html)

* Spam classification with Naive Bayes
  - [“WhyShould I Trust You?” Explaining the Predictions of Any Classifier](https://arxiv.org/pdf/1602.04938v1)
  - Tokenization

## Part 2.

* Local Minimum:
  - A point where the function value is lower than the values at nearby points.
  - It's a "valley" or low point within a specific region of the function's graph.
  - A function can have multiple local minima.
  - Example: Imagine a landscape with multiple valleys; a local minimum is a valley that's the lowest point in its immediate area, but not necessarily the lowest overall.

* Global Minimum:
  - A point where the function value is lower than at any other point in the entire domain of the function.
  - It's the absolute lowest point of the function's graph.
  - A function can have only one global minimum.
  - Example: In the same landscape, the global minimum would be the absolute lowest valley, regardless of where it is located.

* Importance in Machine Learning:
  - In machine learning, optimization algorithms aim to find the global minimum of a loss function (a function that measures how well a model is performing).
  - However, algorithms can sometimes get "stuck" in local minima, preventing them from finding the true global minimum.
  - This is a significant challenge in training complex models, as the global minimum represents the best possible solution.

* Gradient Descent (aka Batch Gradient Descent)
* Incremental/Stochastic Descent

W6 - Gradient Descent Algorithms.ipynb

## Class Supporting Video

5.1 Classification

5.2 The Logistic Function

5.3 Classification Example

5.4 The Decision Boundary

5.5 Logistic Loss

5.6 Gradient Descent With Log Loss
