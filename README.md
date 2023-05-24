# Mug Material Classifier(KNN)

**Description:** This machine learning project is designed to predict the type of material of a mug. This prediction is based on four measurements: height, diameter, weight, and hue (color). There are three types of material that a mug can be predicted to be made of.

**Note:** We have 3 datasets here:

**train_dataset.csv:** 

![pd.read_csv('train_dataset.csv').head()](https://raw.githubusercontent.com/EliteArrow/Mug-Material-Type-Prediction/main/Screenshots/Untitled.png)


**test_dataset.csv:**

![pd.read_csv('test_dataset.csv').head()](https://raw.githubusercontent.com/EliteArrow/Mug-Material-Type-Prediction/main/Screenshots/Untitled%201.png)


## Project Structure

- a) Data loading and preprocessing
- b) Implementation of K-Nearest Neighbors (KNN) algorithm
- c) Performance evaluation using Leave-One-Out (LOO) cross-validation
- d) Modification of KNN algorithm to use Manhattan distance as the similarity measure
- e) Prediction with KNN and Cartesian distance without the fourth attribute

### Libraries Required

This project requires `pandas` for data manipulation, `sklearn.neighbors` for the KNN classifier, `sklearn.model_selection` for the LeaveOneOut function, `sklearn.preprocessing` for encoding class labels, and `sklearn.metrics` for computing the accuracy score.

## How to Run the Code

Ensure that the `train_dataset.csv`, `test_dataset.csv`, and `program_dataset.csv` files are in the correct location and the path to them is correctly mentioned in the code. (also need to be in correct format as shown above)

1. You need to have the necessary Python libraries installed (if not installed just run first cell)
2. Then run the each cell one by one.

## Results Interpretation

The results are interpreted in terms of the accuracy of predictions. In the LOO cross-validation process, each data point is removed from the training set, the algorithm is trained on the remaining data, and then tested on the removed point to see if the predicted label matches the actual label or not. This process is repeated for each data point and gives an estimate of the accuracy of the algorithm.

The project compares the performance of the algorithm using Cartesian and Manhattan distance measures, and with different numbers of features. This comparison helps in understanding which distance measure and feature set gives better performance.

## Modifying the Code

You can modify this code to use different algorithms, distance measures, cross-validation techniques, or datasets. The K value in KNN can be adjusted to experiment with the results. Different preprocessing techniques can be applied to the data to further improve the results.
