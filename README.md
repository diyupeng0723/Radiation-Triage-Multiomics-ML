# Multi-Omics and Machine Learning Pipeline for Early Radiation Injury Triage (PBI vs TBI)

This repository contains the official R code implementation and standardized multi-omics dataset to replicate all figure evaluations (Figure 1 through Figure 6) presented in our manuscript.

## Overview
Diagnostic differentiation between partial-body irradiation (PBI) with bone marrow sparing and total-body irradiation (TBI) is critical during radiological emergency triage. This pipeline integrates:
* **DIA LC-MS/MS Proteomics** and **UPLC-QTOF Metabolomics** from non-human primate (NHP) cohorts.
* Feature selection using **LASSO** and **Random Forest**.
* Diagnostic utility modeling using **Logistic Regression**, **CART Decision Trees**, and **Clinical Nomograms**.

## Repository Structure
* `data_standardized_final.csv`: Normalized relative abundance matrix of serum proteins and metabolites across multiple time points.
* `Rcode0623.R`: The complete R pipeline script generating Figures 1-6.

## Getting Started
### System Requirements
This pipeline is written in R (>= 4.0.0). The script automatically checks and installs the following required R libraries:
```R
dplyr, tidyr, ggplot2, ggpubr, pheatmap, glmnet, randomForest, pROC, rms, rpart, rpart.plot, fmsb, scales, gridExtra
