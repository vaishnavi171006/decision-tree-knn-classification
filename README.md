# decision-tree-knn-classification
Implementation and comparison of Decision Tree and K-Nearest Neighbour (KNN) classification algorithms using Python, Scikit-learn, and the Iris dataset.
# Decision Tree and K-Nearest Neighbour (KNN) for Classification

## 📌 Project Overview
This project implements and compares two supervised machine learning algorithms: Decision Tree and K-Nearest Neighbour (KNN). Both algorithms are applied to the Iris dataset using Python and Scikit-learn to classify flowers into different species.

## 🎯 Aim
To understand and implement Decision Tree and KNN algorithms for classification and evaluate their performance using standard classification metrics.

## 🎯 Objectives
- Understand the basic concepts of Decision Tree and KNN.
- Learn how Decision Trees split data using Entropy and Information Gain.
- Understand distance metrics and majority voting in KNN.
- Implement both algorithms using Scikit-learn.
- Evaluate and compare model performance.
- Interpret classification results using standard evaluation metrics.

## 🛠️ Technologies Used
- Python
- Jupyter Notebook
- Pandas
- NumPy
- Scikit-learn

## 📂 Project Structure

```text
decision-tree-knn-classification/
│
├── decision_tree_knn.ipynb
└── README.md
```

## 📊 Dataset
This project uses the Iris dataset, which contains flower measurements for three species:

- Setosa
- Versicolor
- Virginica

### Input Features
- Sepal length
- Sepal width
- Petal length
- Petal width

### Target Variable
- Species

The dataset is loaded from an online CSV source.

## 📚 Theory

### 1. Decision Tree
A Decision Tree is a supervised learning algorithm that makes predictions by splitting data according to feature values. It has a tree-like structure consisting of decision nodes, branches, and leaf nodes.

#### Key Concepts
- **Entropy:** Measures the impurity or uncertainty in a dataset.
- **Information Gain:** Measures the reduction in entropy after splitting data using a feature.
- **Gini Index:** Measures the impurity of data and can be used to select splits.
- **Overfitting:** Occurs when a tree learns the training data too closely and performs poorly on unseen data.

#### Advantages
- Easy to understand and interpret.
- Requires little feature preprocessing.
- Can model non-linear decision boundaries.

#### Limitations
- Can overfit the training data.
- Small changes in data can produce a different tree.

### 2. K-Nearest Neighbour (KNN)
KNN is a supervised, instance-based learning algorithm that classifies a data point according to the majority class among its nearest neighbours.

#### Working Principle
1. Select the number of neighbours, K.
2. Calculate the distances between the test point and training points.
3. Identify the K nearest neighbours.
4. Use majority voting to assign the predicted class.

#### Euclidean Distance

d(x, y) = √Σ(xᵢ − yᵢ)²

#### Advantages
- Simple to understand and implement.
- No explicit model-training process is required.
- Can classify complex decision boundaries.

#### Limitations
- Prediction can be computationally expensive for large datasets.
- Sensitive to feature scaling and irrelevant features.
- Performance depends on the choice of K.

## ⚙️ Implementation Steps
1. Import the required libraries.
2. Load the Iris dataset.
3. Separate the input features and target labels.
4. Split the dataset into 80% training data and 20% testing data.
5. Standardize the features for KNN using StandardScaler.
6. Train the Decision Tree classifier using the Entropy criterion.
7. Train the KNN classifier using five neighbours.
8. Predict the species using both models.
9. Evaluate both models using accuracy, confusion matrix, precision, recall, and F1-score.
10. Compare the results of the two algorithms.

## 🚀 How to Run the Project
1. Install Python and Jupyter Notebook.
2. Install the required libraries if they are not already installed:

   ```bash
   pip install pandas numpy scikit-learn jupyter
   ```

3. Open Jupyter Notebook.
4. Open `decision_tree_knn.ipynb`.
5. Run all cells sequentially.
6. Observe the evaluation results for both classifiers.

**Note:** An internet connection is required to load the dataset from the online CSV source.

## 📈 Model Evaluation
The models are evaluated using:

- **Accuracy:** Percentage of correctly classified samples.
- **Confusion Matrix:** Shows correct and incorrect predictions for each species.
- **Precision:** Measures the correctness of positive predictions for each class.
- **Recall:** Measures how many actual instances of each class are correctly identified.
- **F1-score:** Combines precision and recall into a single metric.

## 🔍 Comparison of Algorithms

| Feature | Decision Tree | KNN |
|---|---|---|
| Learning approach | Tree-based | Distance-based |
| Training | Learns decision rules | Stores training examples |
| Feature scaling | Generally not required | Important |
| Interpretability | Easy to interpret | Less interpretable |
| Main parameter | Criterion and tree depth | Number of neighbours (K) |
| Main limitation | Overfitting | Expensive predictions on large datasets |

## 📈 Expected Output
- Sample rows from the Iris dataset.
- Decision Tree accuracy and classification report.
- Decision Tree confusion matrix.
- KNN accuracy and classification report.
- KNN confusion matrix.
- Performance comparison of both classifiers.

## 📚 Learning Outcomes
- Understand two important classification algorithms.
- Learn about Entropy and Information Gain.
- Understand distance calculations and majority voting.
- Apply feature scaling for KNN.
- Evaluate models using classification metrics.
- Compare the strengths and limitations of Decision Tree and KNN.
