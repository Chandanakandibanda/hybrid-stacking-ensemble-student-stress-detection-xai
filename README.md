# Hybrid Stacking Ensemble for Student Stress Detection with Explainable AI

A hybrid stacking ensemble learning framework for detecting university student stress levels, combining classical machine learning, deep learning, and Explainable AI (SHAP).

**Author:** Chandana Sruthi Kandibanda  
**Programme:** MSc Artificial Intelligence and Data Science  
**Institution:** Edinburgh Napier University  
**Year:** 2026

---

## Overview

Student stress is a multifactorial problem influenced by academic workload, lifestyle habits, social factors, and psychological conditions. This project proposes a **hybrid stacking ensemble** that leverages the complementary strengths of:

- **Random Forest**
- **XGBoost**
- **Multi-Layer Perceptron (MLP)**

as base learners, with **Logistic Regression** as the meta-learner.

The framework is evaluated against several strong baselines (Logistic Regression, Decision Tree, SVM, Random Forest, XGBoost, MLP, SimpleRNN, and ProtoNAM) and is made interpretable using **SHAP**.

### Key Results (Test Set)

| Model                              | Accuracy | Notes                          |
|------------------------------------|----------|--------------------------------|
| Hybrid Stacking (RF + XGB + MLP)  | **1.00** | Best overall                   |
| MLP / SimpleRNN                    | 1.00     | Strong deep learning baselines |
| Logistic Regression                | 0.98     |                                |
| ProtoNAM                           | 0.94     | Interpretable neural additive model |
| XGBoost                            | 0.93     |                                |
| SVM                                | 0.92     |                                |
| Random Forest                      | 0.87     |                                |
| Decision Tree                      | 0.71     |                                |

**Most important features** identified by SHAP:  
`Screen_Time`, `Assignment_Load`, `Family_Support`

---

## Dataset

**University Student Stress Dataset**  
- Source: [Mendeley Data](https://data.mendeley.com/datasets/rc5htd5dfr/1)  
- DOI: [10.17632/rc5htd5dfr.1](https://doi.org/10.17632/rc5htd5dfr.1)  
- Size: 3,000 undergraduate students (Public, Private & National universities in Bangladesh)  
- Target: `Stress_Level` → Low / Medium / High  
- License: **CC BY 4.0**

Please download the dataset from the link above and place the CSV file in a `data/` folder (or update the path in the notebook).

---

## Project Structure

```text
├── Code_with_ProtoNAM.ipynb     # Main experimental notebook
├── data/                        # Place the dataset CSV here
├── requirements.txt
└── README.md
