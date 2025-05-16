# Amini Canopy or Crop Challenge 🛰️🌿

This repository contains my Gold Medal-winning solution for the [Amini Canopy or Crop Challenge](https://zindi.africa/competitions/amini-canopy-or-crop-challenge) hosted by Zindi Africa. The goal was to classify agricultural plots as either **canopy**, **crop**, or **other** using aggregated features from satellite-derived datasets.

---

## 🧠 Problem Statement

Participants were provided with satellite-derived data over time for various agricultural zones. The task was to build a model that accurately classifies each zone based on its overall characteristics into one of three land cover classes.

---

## 🛠️ Approach Overview

- **Feature Aggregation:**
  - For each `ID`, computed statistical summaries (mean, std, min, max) across all available features.
  - Dropped irrelevant or redundant columns (e.g., timestamp-based features).

- **Model Training:**
  - Used **LightGBM** for classification.
  - Applied **Stratified K-Fold Cross-Validation**.
  - Handled class imbalance with **class weights**.
  - Optimized for **macro F1-score**.

---

## 📁 Files

- `Amini Canopy or Crop Challenge Notebook.ipynb`: Full training and inference pipeline.
- `submission.csv`: Example format for predictions.

---

