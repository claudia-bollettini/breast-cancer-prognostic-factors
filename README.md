# Prognostic factors and treatment efficacy in the Rotterdam breast cancer cohort: a multi-model analysis

## Overview
This project was developed as the final exam for the "Statistical models for Healthcare data" course at Politecnico di Milano and Università Vita-Salute San Raffaele. It investigates how individual clinical and pathological characteristics impact the probability of breast cancer recurrence within six years from surgery and the probability of death within ten years. Furthermore, it evaluates the effectiveness of adjuvant therapies, highlighting the challenges of estimating treatment effects in observational settings where therapies are not randomly assigned.

## Dataset
The analysis was conducted on data from 2,982 primary breast cancer patients included in the Rotterdam tumour bank.

## Methodology
To address the research questions, a multi-model approach was implemented:
**Classification Models:** Binary logistic regression models (comprising a baseline full model alongside feature-selected and regularized variants) were developed to predict the dichotomous outcomes of tumor recurrence and long-term mortality.
**Survival Analysis:** Time-to-event models were utilized to estimate recurrence-free and overall survival. This included Kaplan-Meier estimators for non-parametric analysis and semi-parametric Cox Proportional Hazards models to estimate Hazard Ratios.
**Causal Inference:** To address confounding by indication, a causal inference framework was applied. This involved propensity score estimation and Inverse Probability of Treatment Weighting (IPTW) to calculate the Average Treatment Effect (ATE) of hormonal therapy.

## Key Findings
**Prognostic Drivers:** Lymph nodes involvement and histological grade emerged as critical risk factors, whereas smaller tumors demonstrated significant protective effects.
**Treatment Efficacy:** While standard observational models suggested a paradoxical harmful effect of hormonal therapy due to selection bias, causal analysis revealed its true benefit. Hormonal treatment reduces the probability of mortality by 24% and tumor recurrence by 15%.
**Methodological Insights:** The study demonstrates that standard predictive models can distort treatment efficacy due to confounding by indication, underscoring the absolute necessity of causal inference frameworks when evaluating treatments in observational healthcare settings.

## Author
**Claudia Bollettini**
