# House Prices — Advanced Regression Techniques  
*A tidy-verse, caret-driven walkthrough for the classic Kaggle dataset*

[![GitHub Pages](https://img.shields.io/badge/View%20HTML%20Report-green?logo=github)](https://KNNTech.github.io/House-Prices-Analysis/)

## Project Overview
This repository contains **`House Prices Advanced Regression Techniques.Rmd`**, an end-to-end R Markdown notebook that:

1. **Explores & cleans** the Kaggle 🏠 `train.csv` / `test.csv` data  
2. Encodes categorical features & imputes missing values  
3. **Builds, refines, and compares** multiple-linear-regression models (stepwise AIC, manual pruning)  
4. Diagnoses multicollinearity (VIF), residual assumptions, and overfitting  
5. Validates the final model with 10-fold cross-validation and hold-out metrics  
6. Presents results in an **HTML report** that is auto-published via GitHub Pages.

## Key results

| Metric                         | Value                                                  |
|--------------------------------|--------------------------------------------------------|
| **Final RMSE (10-fold CV)**    | ≈ **$18,950**                                          |
| **Adjusted R²**                | **0.92**                                               |
| **Top predictors**             | `OverallQual`, `GrLivArea`, `ExterQual`, `Neighborhood` dummy variables |

*See the “Model Evaluation” and “Residual Diagnostics” sections in the HTML report for full details.*

---

## Live report

The latest HTML build is automatically deployed at:  
<https://KNNTech.github.io/House-Prices-Analysis/>

---

## Re-producing the analysis

1. **Download** Kaggle’s *House Prices — Advanced Regression Techniques* dataset  
   <https://www.kaggle.com/c/house-prices-advanced-regression-techniques>

2. **Place** `train.csv` & `test.csv` in  
   `E:/DataSets/House prices advanced regression techniques/`  
   *(or change the `setwd()` path near the top of the notebook).*

3. **Knit** the R Markdown file; dependencies will load automatically.

---

## Built with

* **R 4.5**
* **Packages:** `tidyverse`, `caret`, `MASS`, `car`, `ggplot2`, `scales`
* **Deployment:** GitHub Actions & GitHub Pages (zero-cost hosting)
