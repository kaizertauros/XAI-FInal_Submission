# XAI Fraud Detection: SHAP vs DiCE

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
## Structure

### Section 1 - Imports
- Cell 1: Install dependencies (Colab only)
- Cell 2: Imports

### Section 2 - Original dataset (with risk scores)
- Cell 3: Load and preview dataset
- Cell 4: Preprocessing and train/test split
- Cell 5: Train baseline Random Forest and confusion matrix
- Cell 6: SHAP global explanation
- Cell 7: SHAP local explanation
- Cell 8: DiCE counterfactual explanations

### Section 3 - Reduced dataset (without risk scores, noise added)
- Cell 9: Drop risk score features, add noise, retrain
- Cell 10: SHAP global explanation
- Cell 11: SHAP local explanation
- Cell 12: DiCE counterfactual explanations
