# Diabetes Risk Prediction — Exploratory Analysis and Machine Learning

[![R Version](https://img.shields.io/badge/R-%3E%3D4.0-blue)](https://www.r-project.org/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)
[![Machine Learning](https://img.shields.io/badge/ML-Logistic%20Regression%20%7C%20Random%20Forest-orange)]()

## 📊 Project Overview

This project develops and evaluates machine learning models for **type 2 diabetes risk prediction** using clinical, biochemical, and anthropometric data from 403 patients. The central question is whether routinely available parameters — blood glucose, lipid profile, BMI, blood pressure, and waist-to-hip ratio — can reliably identify individuals at high risk of diabetes in **community pharmacy settings**.

**Key contributions:**
- Comprehensive exploratory data analysis of metabolic risk factors
- Binary classification models (logistic regression & random forest)
- Clinical interpretation with sensitivity/specificity trade-offs
- Interactive Shiny application for data exploration

---

## 🎯 Clinical Motivation

Type 2 diabetes affects over 400 million adults worldwide, with one-third of cases undiagnosed. Community pharmacies are uniquely positioned for **early detection** due to frequent patient interactions and access to metabolic measurements (blood glucose, cholesterol, blood pressure). However, pharmacists need **interpretable, evidence-based tools** to identify high-risk individuals for referral.

This project demonstrates that machine learning can complement clinical judgment, with models achieving **>86% accuracy** using only measurements available in a typical pharmacy consultation.

---

## 🛠️ Technologies & Skills Demonstrated

### Languages & Environment
- **R 4.x** — Core analysis language
- **RMarkdown** — Reproducible reporting (HTML + GitHub output)
- **Shiny** — Interactive dashboard development

### Key Libraries

| Domain | Packages |
|--------|----------|
| **Data wrangling** | `dplyr`, `readr` |
| **Visualization** | `ggplot2` |
| **Machine learning** | `caret` (model training), `randomForest`, `pROC` (AUC) |
| **Statistical modeling** | `glm` (logistic regression) |
| **Model evaluation** | `confusionMatrix`, variable importance |

---

## 📁 Dataset Description

**Source:** [hbiostat.org/data](https://hbiostat.org/data) — publicly available clinical dataset

| Characteristic | Details |
|----------------|---------|
| **Sample size** | 403 patients |
| **Variables** | 19 clinical, biochemical, anthropometric |
| **Outcome** | `glyhb` (glycated haemoglobin) — diabetes defined as ≥6.5% |

### Variable Categories

| Category | Variables |
|----------|----------|
| **Demographic / ID** | id, age, gender, location, frame |
| **Biochemical** | chol (total cholesterol), stab.glu (glucose), hdl (HDL cholesterol), ratio (chol/HDL), glyhb (HbA1c) |
| **Anthropometric** | height, weight, waist, hip, BMI (derived), waist/hip ratio (derived) |
| **Vital signs** | bp.1s, bp.1d, bp.2s, bp.2d (duplicate measurements) |

---

## 🔬 Analysis Workflow
