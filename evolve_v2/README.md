# Tuned Multi-Class Severity Classification (evolve_v2)

This folder contains the second version of the global pollution model, benchmarking multi-class classifiers and optimizing hyperparameters via GridSearchCV.

## 📌 Objectives
Classify countries into **Low**, **Medium**, or **High** Pollution Severity brackets and tune hyperparameters to improve predictive accuracy.

## 📂 Workflow & Tuning

### 1. Classifier Implementations
- **Gaussian Naive Bayes (GNB)**:
  - Evaluates class probabilities under the feature independence assumption.
  - *Takeaway*: Limited in environmental modeling because industrial waste, CO2 emissions, and pollution indexes are naturally highly correlated in practice.
- **K-Nearest Neighbors (KNN)**:
  - Classifies country environmental profiles based on parameter neighborhood distances.
  - *Tuning*: GridSearchCV optimized neighbor count (found optimal $k=9$ with Manhattan distance).
- **Decision Tree Classifier**:
  - Notebook: [advanced_workflow.ipynb](file:///c:/Users/admin/VSCode/ML/Global-Pollution-Energy-Analysis/evolve_v2/advanced_workflow.ipynb)
  - Partitions feature spaces at specific numerical thresholds based on Gini impurity.
  - *Tuning*: GridSearchCV tuned `max_depth` and `min_samples_split` to prune branches and prevent overfitting.

### 2. Hyperparameter Optimization Results
GridSearchCV tuning significantly increased classification accuracy over baseline configurations:

* **Decision Tree (Recommended)**: Baseline: 81.0% $\rightarrow$ **Tuned: 88.4%** (`max_depth=5`, `min_samples_split=5`)
* **K-Nearest Neighbors**: Baseline: 79.2% $\rightarrow$ **Tuned: 83.8%** ($k=9$)
* **Gaussian Naive Bayes**: Baseline: 76.5% $\rightarrow$ **Tuned: 76.5%**

## 💡 Policy Insights & Recommendations
* **Targeted Infrastructure**: Subsidize waste heat capture and energy-recovery plant installations in mid-severity countries generating high industrial waste but minimal energy capture (e.g. Hungary).
* **Eco-Efficiency Quotas**: Establish mandatory minimum energy-to-waste recovery quotas. Tracking the `Eco_Efficiency_Ratio` dynamically can flag impending shifts into higher severity brackets.
