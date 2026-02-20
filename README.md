# Final Project: Subsampling vs Ridge vs Lasso vs Elastic Net  
Pranav Senthilkumaran  
Master’s in Data Science  
Rutgers University  

---

##  Project Overview

This project investigates the theoretical and empirical relationship between:

- Ridge Regression (ℓ2 Regularization)  
- Lasso Regression (ℓ1 Regularization)  
- Elastic Net (Convex combination of ℓ1 and ℓ2)  
- Subsampling-based Ensemble Linear Models  

Using controlled high-dimensional simulations (n = 200, p = 100), the study evaluates:

- Test Mean Squared Error (MSE)  
- Bias–Variance Decomposition  
- Model Stability  
- Sensitivity to Subsampling Ratios  
- Model Complexity vs Regularization Strength  

The goal is to understand how shrinkage methods compare to naive subsampling in high-dimensional linear settings.

---

## 📊 Key Contributions

- High-dimensional synthetic data simulation  
- Empirical Bias² + Variance + Noise decomposition  
- Cross-validated regularization comparison  
- Subsampling instability analysis  
- PCA and diagnostic visualizations  
- Model complexity analysis across λ grid  

---

## 📂 Repository Structure

```
pranavssss/
│
├── Final Project Files/
│   ├── Project first draft.Rmd
│   ├── First Draft Final Project Report.pdf
│
├── Data Mining 2025 Old Project Submission Files/
│   ├── Data Mining Project Report.pdf
│   ├── Data Mining RMDProject Report.pdf
│   ├── CodeRMD_Ganesh_Goli_Senthilkumaran.Rmd
│   ├── PresentationSlides.pdf
│
└── README.md
```

---

## Technologies Used

- R  
- glmnet  
- caret  
- ggplot2  
- dplyr  
- corrplot  
- GGally  

---

## Theoretical Framework

The project empirically validates the classical prediction error decomposition:

\[
\mathbb{E}[(Y - \hat{f}(X))^2] =
\text{Bias}^2 + \text{Variance} + \sigma^2
\]

Regularization introduces bias intentionally to reduce variance and improve generalization in high-dimensional settings.

---

## How to Run

1. Open `Project first draft.Rmd` in RStudio  
2. Install required packages:

```r
install.packages(c("glmnet","ggplot2","dplyr","caret","corrplot","GGally","zoo"))
```

3. Knit to PDF (requires LaTeX / xelatex)

---

##  Future Work

- Sparse coefficient simulations  
- Correlated predictor structures  
- Real-world dataset validation  

---

