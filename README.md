🦎 Lizard Abundance Prediction Using Random Forest
Overview
This project explores the application of machine learning techniques to predict the abundance of lizards based on environmental and ecological data. The model used is Random Forest, which is effective for handling complex, non-linear relationships and allows for analysis of feature importance.

🎯 Key Objectives
Predict the abundance of lizards using machine learning.

Understand the influence of various environmental and ecological features on lizard populations.

Provide species-specific modeling and explainability insights.

Optionally explore the effect of chemical features on lizard abundance.

📊 Data
The dataset is sourced from Dryad: 10.5061/dryad.83bk3j9nr
It contains 58 rows and various features including:

Environmental Factors: Bio1 (Annual Mean Temp), Bio4 (Seasonality), Bio6 (Precipitation), etc.

Species Information: Sceloporus_species, Abundance, Richness, etc.

Sample Metadata: Sample_mass, Elevation, Latitude, etc.

Chemical Compounds (optional): Acids, alcohols, and other biochemical features (e.g., Octadecanoic acid, 1-Nonanol).

🧠 Approach
1. Data Preprocessing
Loaded and explored dataset in Google Colab.

Removed or imputed missing data.

Selected relevant features for modeling.

2. Modeling with Random Forest
Trained a Random Forest Regressor on the data.

Evaluated using R² Score and Mean Squared Error (MSE).

R² Score: 0.396

MSE: 4.63

3. Feature Importance & Correlation
Generated feature importance plots for top predictors.

Created a correlation heatmap to assess relationships between features.

4. Species-Specific Modeling
Grouped data by each lizard species.

Visualized sample count and abundance patterns.

Performed correlation analysis per species.

5. 🔬 Chemical Feature Analysis (Optional & Fun!)
Selected only chemical compounds (acids, alcohols, etc.) as features.

Trained a separate Random Forest model to predict abundance.

Compared performance to full-feature model.

Visualized chemical-specific feature importances.

📁 File Structure
bash
Copy
Edit
📂 lizard-abundance-prediction/
│
├── lizard_abundance_colab.ipynb     # Main analysis and model notebook (Google Colab)
├── chemical_feature_importance.png  # Feature importance plot for chemical model
├── visualizations/                  # Folder with model evaluation & SHAP plots
└── README.md                        # This file
▶️ Usage
To run the project:

Open the Colab notebook:
Google Colab Notebook Link

Run all cells to load the data, train models, and generate plots.

All outputs (plots, metrics, SHAP values) will be saved or displayed in the notebook.

🔮 Future Work
Integrate additional features (e.g., genetic or spatial data).

Try other models like XGBoost or Gradient Boosting.

Extend the approach to other species or ecosystems.

👤 Contributors
Laiba Asif – Data science, modeling, visualization

Feel free to fork, star ⭐, or contribute via pull requests or issues!


