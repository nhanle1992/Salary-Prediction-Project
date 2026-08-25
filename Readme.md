# Project: Salary Prediction using Linear Regression

## Overview
This repository showcases a machine learning project focused on predicting an individual's salary based on their years of professional experience. The project demonstrates a complete end-to-end workflow, from initial data exploration and cleaning to model building, validation, and interpretation. It emphasizes best practices in machine learning, including robust model comparison using cross-validation and the importance of model interpretability.

## Learning and Practice Highlights
*   **Data Understanding:** Extensive use of descriptive statistics and various visualization techniques (histograms, box plots, scatter plots, correlation heatmaps, pair plots) for univariate, bivariate, and multivariate analysis.
*   **Data Pre-processing:** Hands-on experience with handling missing values, duplicate entries, and feature scaling (`StandardScaler`) to prepare data for modeling.
*   **Model Building & Selection:** Implemented and compared a Simple Linear Regression model with a Polynomial Regression alternative. Utilized `Pipeline` for efficient workflow and `KFold` cross-validation for robust performance evaluation and model selection based on meaningful improvements in RMSE.
*   **Model Evaluation:** Applied key regression metrics (MSE, RMSE, R2 Score) and diagnostic plots (Actual vs. Predicted, Residual Plot) to assess model performance and validate assumptions.
*   **Interpretability:** Focused on selecting the simplest model that meets performance criteria, highlighting the importance of interpretability in business contexts.

## Project Information

**Problem:** Accurately predicting an individual's salary given their years of experience.

**Objective:** To develop a machine learning model that provides reliable and interpretable salary predictions.

**Dataset:** `Salary_dataset.csv` - Contains 'YearsExperience' and 'Salary' for a set of individuals.

## Repository Structure

```
.  
├── Salary_Prediction_Project.ipynb  # Main Jupyter Notebook with all the code and analysis
├── data/  
│   └── Salary_dataset.csv           # The raw dataset used for the project
├── README.md                      # This file
└── Practice Salary analysis - report.html # Final report
```

## Key Findings
*   A **very strong positive linear relationship** exists between 'YearsExperience' and 'Salary' (Pearson correlation: `0.9782`).
*   The **Simple Linear Regression model** was selected as the optimal choice after rigorous comparison with a Polynomial Regression model using 5-fold cross-validation. The polynomial model did not offer a *meaningful* improvement in prediction accuracy to justify its increased complexity.
*   The chosen model demonstrates excellent predictive performance:
    *   **Root Mean Squared Error (RMSE):** Approximately `${:.2f}` (indicating the average prediction error is within a reasonable range for the salary scale).
    *   **R-squared (R2 Score):** Approximately `{:.4f}` (meaning over 90% of the variance in salary can be explained by years of experience).
*   Diagnostic plots confirm the model's assumptions and reliability, showing predicted salaries closely align with actual values and residuals are randomly distributed.

## Usage
To run this project:
1.  Clone the repository.
2.  Ensure you have the necessary Python libraries installed (see `requirements.txt` if provided, otherwise check notebook imports).
3.  Open and run the `Salary_Prediction_Project.ipynb` notebook in a Jupyter environment (e.g., Google Colab, Jupyter Lab).

## Technologies Used
*   Python
*   Pandas (for data manipulation)
*   NumPy (for numerical operations)
*   Matplotlib & Seaborn (for data visualization)
*   Scikit-learn (for machine learning models and utilities)
