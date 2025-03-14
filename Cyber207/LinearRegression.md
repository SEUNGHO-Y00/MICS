# Linear Regression & Gradient Descent

* Agenda
  - Questions about async sessions
  - Discussion ["The Unreasonable Effectiveness of Data"](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/35179.pdf)
  - Train/test splits
  - Code: Nearest Neighbor classifier implementation

## Part 1.

* The Unreasonable Effectiveness of Data
  - Shared cognitive and cultural context, linguistic expression
  - Unsupervised learning on unlabeled data is more plentiful than labeled data
  - Machine Learning Data Competition [Kaggle](https://www.kaggle.com/)
  - Machine Learning Data Competition [Tacotron](https://google.github.io/tacotron/) (/täkōˌträn/): An end-to-end speech synthesis system by Google

## Part 2.

* All models are wrong, but some models are useful - George Box
  - Machine learning data are simple mathematical data and general ideas
  - The model should be intelligent enough to trust the data

* Train / test splits
  - Train Data
  - Validation Data
  - Test Data
  - Original set => Trainingset + test set => Training set + Validation set + Test set => ML Algorithm => Predictive model

## Part 3.

* KNN Model
  - k-nearest neighbors (KNN) algorithm
  - A simple, versatile machine learning method used for both classification and regression tasks, based on the principle that similar data points are located near each other.
  - [sklearn.neighbors.KNeighborsClassifier](https://scikit-learn.org/0.15/modules/generated/sklearn.neighbors.KNeighborsClassifier.html)

* W2 - KNN usage.ipynb
* W2 - KNN implementation.ipynb

```python
class NearestNeighbors:
    # Initialize an instance of the class.
    def __init__(self, metric=EuclideanDistance):
        self.metric = metric

    # No training for Nearest Neighbors. Just store the data.
    def fit(self, train_data, train_labels):
        self.train_data = train_data
        self.train_labels = train_labels

    # Make predictions for each test example and return results.
    def predict(self, test_data):
        results = []
        for item in test_data:
            results.append(self._predict_item(item))
        return results

    # Private function for making a single prediction.
    def _predict_item(self, item):
        best_dist, best_label = 1.0e10, None
        for i in range(len(self.train_data)):
            dist = self.metric(self.train_data[i], item)
            if dist < best_dist:
                best_label = self.train_labels[i]
                best_dist = dist
        return best_label
```

## Class Supporting Video

2.1 Learning by Optimization

2.2 Linear Regression

2.3 The Loss Function

2.4 Gradient Descent: Intuition

2.5 Gradient Descent: Derivation
