# Breast Cancer Classification using Supervised Learning

This repository contains a machine learning project focused on applying **supervised learning algorithms** to classify breast cancer tumors as **malignant** or **benign** using the built-in dataset from `sklearn`.


## Objective :

To evaluate and compare the performance of five supervised classification algorithms on a real-world dataset to determine the most effective model for breast cancer detection.


## Dataset :

We use the **Breast Cancer Wisconsin Diagnostic Dataset** provided by `sklearn.datasets`.

- 569 instances
- 30 numeric features
- Binary classification target: `0` (malignant), `1` (benign)


## Preprocessing Steps :

- Loaded dataset using `sklearn.datasets.load_breast_cancer`.
- Checked and confirmed no missing values.
- Scaled features using **StandardScaler** to normalize the input data.


## Classification Algorithms Used :

1. **Logistic Regression**  
   A linear model for binary classification, best suited for linearly separable data.

2. **Decision Tree Classifier**  
   Tree-based model that splits features to make decisions; prone to overfitting.

3. **Random Forest Classifier**  
   Ensemble of decision trees that improves generalization and reduces overfitting.

4. **Support Vector Machine (SVM)**  
   Finds the optimal margin (hyperplane) for separating classes.

5. **k-Nearest Neighbors (k-NN)**  
   Classifies a sample based on the majority label of its `k` nearest neighbors.


## Model Evaluation :

Each model was evaluated using **accuracy score** on the test set.

| Algorithm           | Accuracy |
|---------------------|----------|
| Logistic Regression | ~97.4%   |
| Decision Tree       | ~92.9%   |
| Random Forest       | ~96.5%   |
| SVM                 | ~96.5%   |
| k-NN                | ~95.6%   |

 **Best Model**: Logistic Regression  
 **Lowest Performer**: Decision Tree (overfitting on training data)

## Conclusion :
This project applied five supervised learning models to classify breast cancer tumors using the sklearn dataset. Logistic Regression performed best in terms of accuracy and minimizing false negatives, making it the most reliable choice. The results highlight the effectiveness of simple, well-tuned models and the importance of careful evaluation in healthcare applications
