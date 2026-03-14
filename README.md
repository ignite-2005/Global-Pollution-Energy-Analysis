# 🌍 Global Pollution Analysis & Energy Recovery
**Data Science | Environmental Impact Modeling**

## 📌 Project Objective
This project analyzes global pollution data (Air, Water, and Soil) to develop strategies for pollution reduction and to predict the potential for converting pollutants into energy.

## 🛠️ Tech Stack & Environment
- **Environment:** Google Colab
- **Language:** Python
- **Libraries:** Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn

## 📂 Project Phases

### Phase 1: Data Preprocessing & EDA
- **Normalization:** Scaled pollution indices (air, water, and soil) for consistent model training.
- **Categorical Encoding:** Applied Label Encoding to handle `Country` and `Year` data.
- **Visualizations:** Created heatmaps to observe correlations between CO2 emissions, Industrial Waste, and Energy Recovery.

### Phase 2: Predictive Modeling
- **Linear Regression:** Trained to predict the specific amount of **Energy Recovery** based on industrial waste and pollution levels.
- **Logistic Regression:** Used to classify countries into **Pollution Severity Categories** (Low, Medium, High).

### Phase 3: Evaluation
- Used **R-squared (R²)** and **Mean Squared Error (MSE)** to evaluate the regression model.
- Used **Confusion Matrices** and **Classification Reports** to verify the accuracy of pollution categorization.

## 📈 Future Work
- Incorporating my recent learning of **SVM (Support Vector Machines)** to create more precise boundaries for pollution classification between countries.
