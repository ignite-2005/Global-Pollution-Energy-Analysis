# Baseline Regression - Environmental Impact Analysis (evolve_v1)

This folder contains the initial version of the global pollution model, focusing on preprocessing raw environmental indexes, exploratory visualizations, and baseline regressions.

## 📌 Objectives
1. **Regression**: Predict specific **Energy Recovery (GWh)** capacities based on country-level waste and pollution metrics.
2. **Classification**: Categorize countries into baseline **Pollution Severity Categories** (Low, Medium, High).

## 📂 Workflow & Data Pipeline

### 1. Data Preprocessing & EDA
- **Normalization**: Scaled air, water, and soil pollution indices to maintain consistency across diverse environmental scales.
- **Categorical Encoding**: Applied label encoding to handle `Country` and `Year` factors.
- **Feature Engineering**: Formulated the `Eco_Efficiency_Ratio` (Energy Recovered / (Industrial Waste + 1)) to measure resource conversion performance.
- **Visualizations**: Created correlation heatmaps to observe structural relationships between industrial outputs and energy recovery.

### 2. Predictive Modeling
- **Linear Regression**:
  - Notebook: [baseline_workflow.ipynb](file:///c:/Users/admin/VSCode/ML/Global-Pollution-Energy-Analysis/evolve_v1/baseline_workflow.ipynb)
  - Trained to predict GWh energy recovery based on industrial waste, CO2 emissions, and pollution levels.
  - Evaluated using Mean Squared Error (MSE) and R-squared ($R^2$).
- **Logistic Regression**:
  - Used to classify countries into initial pollution severity categories.
  - Evaluated using Accuracy, Precision, Recall, and Confusion Matrices.

## 📈 Findings & Takeaways
* **Policy Influence**: Encoded country baseline trends dominated Linear Regression coefficients, indicating that geographic differences in infrastructure drive energy recovery far more than absolute pollutant numbers.
* **Feature Collinearity**: High correlations between Air, Water, and Soil indices caused collinearity in linear models, showing that environmental variables tend to degrade together under industrial load.
