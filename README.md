# 🦎 Lizard Abundance Prediction Using Random Forest

## 🌍 Overview

This project applies machine learning techniques to predict the **abundance of Sceloporus lizards** using environmental, physiological, and chemical features. By training a **Random Forest Regressor**, we aim to uncover the most impactful variables influencing lizard populations, while leveraging interpretability techniques such as **SHAP** and **correlation analysis**. The insights contribute to eco-evolutionary studies by shedding light on species-specific responses to environmental and biochemical conditions.

---

## 🎯 Key Objectives

- Predict the abundance of lizards using machine learning.
- Understand the influence of various environmental and ecological features on lizard populations.
- Provide species-specific modeling and explainability insights.
- Explore the effect of chemical features on lizard abundance.

---

## 📊 Data

- **Source:** [Dryad Dataset](https://datadryad.org/dataset/doi:10.5061/dryad.83bk3j9nr)
- **Samples:** 58 rows
- **Feature Types:**
  - **Environmental Factors:** `Bio1` (Annual Mean Temp), `Bio4` (Seasonality), `Bio6` (Precipitation), etc.
  - **Species Information:** `Sceloporus_species`, `Abundance`, `Richness`, etc.
  - **Sample Metadata:** `Sample_mass`, `Elevation`, `Latitude`, etc.
  - **Chemical Compounds:** Acids, alcohols, and other biochemical features (e.g., `Octadecanoic acid`, `1-Nonanol`).

---

## 🧠 Approach

### 1. Data Preprocessing
- Loaded and explored dataset in **Google Colab**.
- Removed or imputed missing data.
- Selected relevant features for modeling.

### 2. Modeling with Random Forest
- Trained a **Random Forest Regressor** on the dataset.
- **Evaluation Metrics:**
  - 🧮 R² Score: `0.396`
  - 📉 MSE: `4.63`

### 3. Feature Importance & Correlation
- Generated feature importance plots for top predictors.
- Created a correlation heatmap to assess relationships between features.

### 4. Species-Specific Modeling
- Grouped data by each lizard species.
- Visualized sample count and abundance patterns.

### 5. 🔬 Chemical Feature Model
Focused solely on chemical compounds to understand their predictive power.

#### Selected Chemical Features:
- `'Nonanoic acid'`, `'Decanoic acid'`, `'Dodecanoic acid'`, `'Tridecanoic acid'`
- `'Tetradecanoic acid'`, `'Pentadecanoic acid'`, `'Hexadecanoic acid'`, `'Heptadecanoic acid'`
- `'Octadecanoic acid'`, `'9-Hexadecenoic acid'`, `'9,12-Octadecadienoic acid'`, `'Oleic acid'`

#### Model Results (Chemical-Only):
- 🧪 **R² Score:** `0.712`
- 📉 **MSE:** `2.21`

---

## ▶️ How to Use

To run the project:

1. Open the Colab notebook: **[Google Colab Notebook Link]** *(replace with your actual link)*
2. Run all cells to:
   - Load and preprocess the data
   - Train the Random Forest models
   - Generate visualizations (feature importance, SHAP plots, heatmaps)
3. Outputs will be displayed or saved in the notebook.

---

## 👩‍🔬 Contributor

**Laiba Asif** – Data science, modeling, visualization

Feel free to ⭐ star, 🍴 fork, or contribute via pull requests and issues!

---
