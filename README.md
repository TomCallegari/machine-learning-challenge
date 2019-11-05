# machine-learning-challenge

The purpose of this assignment was to explore, manipulate and build and then compare multiple machine learning models from the [NASA Kepler Space Telescope](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)
dataset.

This Github Repository contains Jupyter Notebook files for each model and the data wrangling process used to build the algorithm ready dataset.

* [Data Wrangling](https://github.com/TomCallegari/machine-learning-challenge/blob/master/Wrangling.ipynb)
* [Random Forest](https://github.com/TomCallegari/machine-learning-challenge/blob/master/RandomForest.ipynb)
* [Gradient Boosting Machine (GBM)](https://github.com/TomCallegari/machine-learning-challenge/blob/master/GBM.ipynb)
* [Tensorflow.Keras Dense Deep Neural Network](https://github.com/TomCallegari/machine-learning-challenge/blob/master/Deep_NN.ipynb)

## Results Comparison

- Random Forest: .90 Weighted Average Accuracy
- GBM: .91 Weighted Average Accuracy
- DNN: .905 Accuracy

Additionally, different versions of data transformations were conducted during the project and run using the 3 chosen algorithms.  A variable by variable squared transformation, sin transformation and log transformation were each used to compare model accuracy with a final log then zscore transformation outputting the greatest accuracy. Prior to model ingestion a 0 < x < 1 min-max data scaling was also used to ensure variable magnitudes were relative for euclidean based distance measures and to speed gradient descent convergence.