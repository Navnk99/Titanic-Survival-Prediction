# Titanic-Survival-Prediction
This repository contains an implementation of Decision Tree, Random Forest, and AdaBoost algorithms for predicting the survival of passengers on the Titanic. The project uses the Titanic dataset from Kaggle, which provides information about the passengers, such as their age, gender, class, and whether they survived the tragic event.

## Dataset

The dataset used in this project is the Titanic dataset from Kaggle. It consists of two files:

- `train.csv`: This file contains the training data with information about the passengers and whether they survived or not.
- `test.csv`: This file contains the test data for which the survival prediction needs to be made.

## Preprocessing

The code performs several preprocessing steps on the data before training the models:

1. Handling missing values in the Age, Fare, and Embarked columns.
2. Creating new features, such as `Has_Cabin`, `FamilySize`, and `IsAlone`.
3. Encoding categorical features like Sex, Title, Embarked, and Fare.

## Algorithms

The following algorithms are implemented and evaluated:

1. **Decision Tree**: A decision tree classifier is implemented from scratch, with options to choose the criterion (entropy or Gini impurity), maximum depth, minimum samples for splitting, and minimum samples for leaf nodes.

2. **Random Forest**: A random forest classifier is implemented, utilizing the decision tree classifier as the base learner. It allows specifying the number of trees and the minimum number of features to consider for each split.

3. **AdaBoost**: An AdaBoost classifier is implemented, also using the decision tree classifier as the base learner. It allows setting the number of learners and the learning rate.

## Usage

1. Clone the repository.
2. Install the required dependencies (e.g., NumPy, Pandas, Matplotlib).
3. Run the Jupyter Notebook or Python script to preprocess the data, train the models, and evaluate their performance.

## Results

The code compares the performance of the three algorithms (Decision Tree, Random Forest, and AdaBoost) on the train and test sets. The accuracy scores for each model are printed, allowing for a comparison of their predictive capabilities.

## License

This project is licensed under the [MIT License](LICENSE).
