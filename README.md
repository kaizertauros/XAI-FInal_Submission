# XAI Fraud Detection — SHAP vs DiCE

This is the final course assignment for the course "Explainable AI", of the Artificial Intelligence study at Radboud University. This project compares two explainability methods (SHAP and DiCE) applied to a fraud detection model.

## Requirements

Install the required libraries before running the notebook:

pip install shap dice-ml scikit-learn pandas numpy matplotlib

If running on Google Colab, the first cell of the notebook handles this automatically.

## Dataset

Download the dataset from Kaggle and place it in the same folder as the notebook:
https://www.kaggle.com/datasets/umitka/synthetic-financial-fraud-dataset

The file should be named: `synthetic_fraud_dataset.csv`

## How to run

Open `XAI_Notebook.ipynb` and run all cells in order from top to bottom.

## Structure

- Cell 1: Install dependencies (Colab only)
- Cell 2: Imports
- Cell 3: Load and explore dataset
- Cell 4: Preprocessing
- Cell 5: Train baseline Random Forest
- Cell 6: Address synthetic data limitations, retrain
- Cell 7: SHAP global explanation
- Cell 8: SHAP local explanation
- Cell 9: DiCE counterfactual explanations
