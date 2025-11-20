# TECH_CHECK — How to Verify the Project

## 1. Preconditions
- `notebook.ipynb` is opened in Colab or Jupyter
- Dependencies installed via `requirements.txt`
- Dataset file is available in CSV/XLSX format

## 2. Run Check
Steps:
1. Run all notebook cells
2. Upload a test dataset when prompted

Expected:
- Console prints detected columns
- A 3000-row sample is formed
- Both models train without errors
- Downloads appear:
  `reviews_scored.xlsx`, `model_lr.joblib`, `model_rf.joblib`, `vectorizer_meta.joblib`

## 3. Example Predictions Check
Steps:
1. Run the final `predict_one()` examples in the notebook

Expected:
- Reviews containing links/phones/contacts → label = 1
- Neutral short reviews → label = 0

## 4. Reproducibility Check
Steps:
1. Restart runtime/kernel
2. Re-run notebook with the same dataset

Expected:
- Same SAMPLE_N=3000 logic works
- Models train and metrics compute again without failures
