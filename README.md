# Global Pollution & Energy Analysis

This repository contains notebooks and documentation for analyzing global environmental metrics, predicting renewable energy recovery capacities, and classifying country threat levels. The project is structured sequentially into chronological version directories to show progression from baseline models to hyperparameter-tuned classifiers.

---

## 📁 Repository Structure

The files are organized into sequential version folders:

```directory
Global-Pollution-Energy-Analysis/
├── evolve_v1/
│   ├── baseline_workflow.ipynb                   # Preprocessing & baseline regression models (Version 1)
│   ├── Global_Pollution_Analysis.csv               # Global environmental index dataset
│   └── README.md                                 # Baseline regression details & EDA
├── evolve_v2/
│   ├── advanced_workflow.ipynb                   # Multi-class classification & hyperparameter tuning (Version 2)
│   └── README.md                                 # Tuned classification benchmarks & GridSearchCV results
└── README.md                                       # Repository project overview
```

---

## 🗺️ Project Progression Flowchart

```mermaid
graph TD
    A["Global Environmental Data"] --> B["Data Preprocessing & Imputation"]
    B --> C["Feature Engineering: Eco_Efficiency_Ratio"]
    
    subgraph v1_sub ["Version 1: Baseline Environmental Models (evolve_v1)"]
        C --> D1["Linear Regression: GWh Prediction"]
        C --> D2["Logistic Regression: Severity Classification"]
        D1 --> E1["Findings: Country-specific baselines dominate weights"]
    end

    subgraph v2_sub ["Version 2: Classification & Tuning (evolve_v2)"]
        C --> F1["Gaussian Naive Bayes"]
        C --> F2["K-Nearest Neighbors"]
        C --> F3["Decision Tree Classifier"]
        F2 --> G["GridSearchCV Tuning"]
        F3 --> G
        G --> H["Findings: Multi-class split thresholds & tuned boundaries"]
    end

    E1 --> I["Policy Insights & Infrastructure Planning"]
    H --> I
```

---

## 🔬 Subfolder Documentation & Notebooks

Detailed information on the preprocessing, models, and findings for each phase is documented inside the version folders:

1. **[evolve_v1/](file:///c:/Users/admin/VSCode/ML/Global-Pollution-Energy-Analysis/evolve_v1)**: Baseline Regression Modeling & Environmental Metrics Preprocessing.
   - Notebook: [baseline_workflow.ipynb](file:///c:/Users/admin/VSCode/ML/Global-Pollution-Energy-Analysis/evolve_v1/baseline_workflow.ipynb)
   - Phase Document: [evolve_v1/README.md](file:///c:/Users/admin/VSCode/ML/Global-Pollution-Energy-Analysis/evolve_v1/README.md)
2. **[evolve_v2/](file:///c:/Users/admin/VSCode/ML/Global-Pollution-Energy-Analysis/evolve_v2)**: Advanced Multi-Class Classification & Hyperparameter Tuning.
   - Notebook: [advanced_workflow.ipynb](file:///c:/Users/admin/VSCode/ML/Global-Pollution-Energy-Analysis/evolve_v2/advanced_workflow.ipynb)
   - Phase Document: [evolve_v2/README.md](file:///c:/Users/admin/VSCode/ML/Global-Pollution-Energy-Analysis/evolve_v2/README.md)
