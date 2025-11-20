# Weak-Fraud Detector for Reviews (Colab / Jupyter)

## 1. Project Summary
This project detects suspicious/fraud-like user reviews (links, phone numbers,
requests to contact outside the platform, etc.) using review text and weak heuristics.
Two models are trained: Logistic Regression and Random Forest, and the best model
is selected by ROC-AUC.

## 2. Team 
- Abylaikhan Sekerbek, Aziz Abdulin, Arsen Bayakhmet
- Astana IT University, Group: SE-2329

## 3. Technologies
- Python 3.10+ (Google Colab / Jupyter Notebook)
- pandas, numpy, scikit-learn, scipy, matplotlib, joblib, openpyxl

## 4. How to Run

### Option A: Google Colab
1. Open `notebook.ipynb` in Google Colab
2. Run all cells top-to-bottom
3. When prompted, upload a `.csv` or `.xlsx` file with reviews

### Option B: Local Jupyter
```bash
pip install -r requirements.txt
jupyter notebook notebook.ipynb
