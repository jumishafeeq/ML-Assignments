# California Housing Price Prediction - Regression Models

## Objective:
 The objective of this assignment is to evaluate your understanding of regression techniques in supervised learning by applying them to a real-world dataset.

## Dataset:
Use the California Housing dataset available in the sklearn library. This dataset contains information about various features of houses in California and their respective median prices.

## Key Components to be Fulfilled :
### 1.	Loading and Preprocessing :

* Load the California Housing dataset using the fetch_california_housing function from sklearn.  
*	Convert the dataset into a pandas DataFrame for easier handling.  
*	Handle missing values (if any) and perform necessary feature scaling (e.g., standardization).  
*	Explain the preprocessing steps you performed and justify why they are necessary for this dataset.

### 2.	Regression Algorithm Implementation :
 Implement the following regression algorithms:

*	Linear Regression  
*	Decision Tree Regressor  
*	Random Forest Regressor  
*	Gradient Boosting Regressor  
*	Support Vector Regressor (SVR)  

 For each algorithm:  
*	Provide a brief explanation of how it works.  
*	Explain why it might be suitable for this dataset.  

### 3.	Model Evaluation and Comparison :
Evaluate the performance of each algorithm using the following metrics:  
 *	Mean Squared Error (MSE)  
 *	Mean Absolute Error (MAE)  
 *	R-squared Score (R²)
   
Compare the results of all models and identify:  
* The best-performing algorithm with justification.
* The worst-performing algorithm with reasoning.

##  Conclusion :

-  **Best Model : Random Forest Regressor** – best performance across all metrics, robust and generalizable
-  **Weakest Model : Linear Regression** – limited by its assumption of linearity, underperformed in capturing complex patterns
-  Tree-based models (especially ensemble methods) are most suitable for this housing dataset due to their ability to model non-linear relationships.
