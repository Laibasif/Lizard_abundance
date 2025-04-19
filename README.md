🦎 Lizard Abundance Prediction Using Random Forest
🌍 Overview
This project applies machine learning techniques to predict the abundance of Sceloporus lizards using environmental, physiological, and chemical features. By training a Random Forest Regressor, we aim to uncover the most impactful variables influencing lizard populations, while leveraging interpretability techniques such as SHAP and correlation analysis. The insights contribute to eco-evolutionary studies by shedding light on species-specific responses to environmental and biochemical conditions.

🎯 Key Objectives
✅ Predict the abundance of lizards using machine learning.

✅ Understand the influence of environmental and chemical factors on lizard physiology.

✅ Perform species-specific modeling and visual exploration.

✅ Provide interpretable insights using SHAP and feature importance.

✅ Support eco-evolutionary biology research with data-driven insights.

📊 Dataset
Source: Dryad Repository

Rows: 58 samples

Features: Includes environmental variables, fatty acids, alcohols, salicylates, physiological data, and more.

📌 Main Feature Categories:
Environmental:
Bio1, Bio4, Bio6, Bio12, Bio15, Elevation

Species Metadata:
Sceloporus_species, Richness, Abundance, Sample_mass

Chemical Compounds:
Includes over 30 compounds (e.g., Hexadecanoic acid, Oleic acid, Decanal, 1-Octadecanol, etc.)

🔧 Approach
📁 Data Preprocessing
Loaded and explored data

Cleaned missing values

Selected relevant features

Computed correlation heatmap for multicollinearity analysis

🌲 Modeling
Trained a Random Forest Regressor

Evaluated using:

R² Score: 0.396

Mean Squared Error (MSE): 4.63

Trained model to predict Abundance

🔍 Interpretability
Feature Importance Visualization using sklearn

SHAP (SHapley Additive exPlanations) for individual feature contribution

Species-Specific Statistics & Plots:

Sample counts by species

Abundance distribution per species

Violin/Box plots for visual comparison

📈 Results
Moderate predictive performance with R² = 0.396

Most influential features:

Sample_mass

Bio1 (Annual Mean Temp)

Bio6 (Precipitation)

Specific chemical compounds (e.g., Hexadecanoic acid)

SHAP plots provided deep interpretability at global and local levels

📂 Repository Structure
bash
Copy
Edit
📁 data/
    └── 12sppPCM_DRYAD.csv           # Input dataset
📁 visualizations/
    ├── feature_importance.png       # Top features plot
    ├── correlation_heatmap.png      # Heatmap
    └── shap_summary.png             # SHAP explanations
📁 results/
    └── model_output.csv             # Predictions and actual values
📄 model.py                          # Training + Evaluation script
📄 requirements.txt                  # Python dependencies
📄 README.md                         # Project overview
▶️ How to Run
Clone this repo

bash
Copy
Edit
git clone https://github.com/your-username/lizard-abundance-prediction.git
cd lizard-abundance-prediction
Install dependencies

bash
Copy
Edit
pip install -r requirements.txt
Run the model

bash
Copy
Edit
python model.py
Check outputs

Results in: results/

Visuals in: visualizations/

🔭 Future Work
🔄 Try other models (e.g., XGBoost, CatBoost, Gradient Boosting)

➕ Add more data or engineered features (e.g., interactions, seasonality)

🌐 Extend analysis to other reptile species or broader ecological datasets

🧪 Integrate statistical tests to support biological hypotheses

👩‍🔬 Contributors
Laiba Asif – Author and Data Science Lead

Open for collaboration! Feel free to fork, star, or open an issue ✨








