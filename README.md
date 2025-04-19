**Lizard Abundance Prediction Using Random Forest**

**Overview**

This project applies machine learning techniques to predict the abundance of Sceloporus lizards using environmental, physiological, and chemical features. By training a Random Forest Regressor, we aim to uncover the most impactful variables influencing lizard populations, while leveraging interpretability techniques such as SHAP and correlation analysis. The insights contribute to eco-evolutionary studies by shedding light on species-specific responses to environmental and biochemical conditions.

**Key Objectives**

Predict the abundance of lizards using machine learning.

Understand the influence of environmental and physiological factors on abundance.

Perform species-specific modeling and visual exploration.

Provide interpretable insights using SHAP and feature importance.

**Data**

The dataset used in this project is from Dryad: https://datadryad.org/dataset/doi:10.5061/dryad.83bk3j9nr and contains 58 rows and several features, including environmental variables (temperature, elevation, etc.), species data, and chemical compounds.

**Main Feature Categories:**

**Environmental:**
Bio1, Bio4, Bio6, Bio12, Bio15, Elevation

**Physiological & Metadata:**
Sample_mass, Richness, Abundance, Sceloporus_species

**Approach**

**📁 Data Preprocessing
Loaded and explored data**

Cleaned and filtered relevant features

Computed a correlation heatmap to analyze feature relationships

**Modeling**
Trained a Random Forest Regressor on selected features

**Evaluation metrics:
**
R² Score: 0.396

Mean Squared Error (MSE): 4.63

**Predicted the Abundance column**

**📊 Analysis & Explainability**

Feature Importance Plot from the Random Forest model

SHAP (SHapley Additive exPlanations) for global/local feature impact

**Species-Specific Exploration:**

Count of samples per species

Summary statistics

Visualizations per species (e.g., abundance distributions)

**📈 Results**

Moderate model performance with R² = 0.396

**Important predictors:**

Sample_mass

Bio1 (Annual Mean Temperature)

Bio6 (Precipitation)

Visuals like feature importance, SHAP summaries, and correlation heatmap provide further insights

**How to Use**

Open the Google Colab Notebook

Upload the dataset: 12sppPCM_DRYAD.csv

Run the cells sequentially to:

Preprocess data

Train model

Visualize and interpret results

**Laiba Asif – Project Lead & Developer**
**Contributions and suggestions are welcome!**



