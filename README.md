# Probabilistic Insights into Diabetes Prediction

## Introduction
This project uses a Bayesian approach to estimate the chance of diabetes in patients based on the Pima Indians Diabetes dataset. The dataset includes simple health indicators like glucose levels, BMI, age, blood pressure, and family history of diabetes. These factors help the model predict whether someone may have diabetes.

## Purpose
The main goal is to compare two Bayesian logistic regression models:
• one model that uses uninformative priors

• another model that uses informative priors
By comparing them, we can see how adding prior knowledge can affect the model’s stability and how easy it is to interpret the results.

## Core System
The model is trained using Hamiltonian Monte Carlo sampling with four chains and two thousand iterations. This ensures the results are stable and consistent. Convergence is checked using common metrics like R-hat and effective sample size.
In the informative prior model, stronger priors are added for glucose and BMI because they are known to have a stronger relationship with diabetes.

## Findings
The model that uses informative priors fits better from a theoretical perspective and is supported by Bayes Factor results. Even though both models have almost the same predictive accuracy based on WAIC and LOO, the informative prior model is easier to interpret. From the analysis, BMI and family history of diabetes are the most important predictors, while glucose, age, and blood pressure show only small effects.

## Impact
This project shows how Bayesian methods can improve understanding and interpretation in medical prediction tasks. By combining prior knowledge with real data, the model gives clearer insights into how different health factors relate to diabetes risk. This approach can help support better decision-making in health analytics.
