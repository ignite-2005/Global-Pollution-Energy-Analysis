# 🌍 Global Pollution Analysis & Energy Recovery
**Data Science | Environmental Impact & Resource Optimization**

## 📌 Project Objective
This project analyzes global pollution indices (Air, Water, and Soil) to develop strategies for pollution reduction and to predict the potential for converting pollutants into energy. It bridges the gap between environmental data and sustainable resource management.

## 🛠️ Tech Stack & Environment
- **Environment:** Google Colab
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn

## 📂 Project Phases

### Phase 1: Data Preprocessing & EDA
- **Normalization:** Scaled pollution indices for consistent model training across diverse environmental metrics.
- **Categorical Encoding:** Applied Label Encoding to handle `Country` and `Year` data.
- **Visualizations:** Created correlation heatmaps to observe relationships between CO2 emissions, Industrial Waste, and Energy Recovery.



### Phase 2: Predictive Modeling
- **Linear Regression:** Trained to predict the specific amount of **Energy Recovery (GWh)** based on industrial waste and pollution levels.
- **Logistic Regression:** Used to classify countries into **Pollution Severity Categories** (Low, Medium, High).

### Phase 3: Evaluation
- **Regression:** Evaluated using R-squared (R²) and Mean Squared Error (MSE).
- **Classification:** Verified via Confusion Matrices and Classification Reports to ensure accurate categorization of high-risk regions.

---

## 💡 Actionable Insights & Recommendations
Beyond the models, this notebook provides data-driven strategies for environmental policy:

* **Severity Mapping:** Identified how specific pollution levels directly correlate with energy recovery potential, allowing for better prioritization of resources.
* **Infrastructure Investment:** Highlighted specific countries and regions that would benefit most from immediate energy-recovery plant installations.
* **Waste Management Policy:** Provided recommendations for reducing industrial waste based on model coefficients, aiming to optimize the balance between industrial output and environmental health.

---

## 📈 Future Work
- **Advanced Classification:** Incorporating **SVM (Support Vector Machines)** with non-linear kernels to create more precise boundaries for pollution classification.
- **Time-Series Analysis:** Forecasting future pollution trends to help governments prepare infrastructure ahead of time.

---
> **Note:** To run this project, ensure `global_pollution_dataset.csv` is in the same directory as the notebook.
