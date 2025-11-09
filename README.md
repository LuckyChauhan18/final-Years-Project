# ML Classification Project

This project builds and evaluates multiple machine learning models on a binary classification dataset. The main objective is to handle **class imbalance**, improve **generalization**, and compare different algorithms.

---

## ✅ Models Implemented

We trained and evaluated the following models:

* **Logistic Regression**
* **Support Vector Machine (SVM)**
* **Random Forest Classifier**

Each model was tested after applying proper preprocessing.

---

## ✅ Handling Imbalanced Data

The dataset was imbalanced, so we used **SMOTE (Synthetic Minority Oversampling Technique)** to generate synthetic samples of the minority class.

SMOTE was applied **inside a Pipeline** to prevent data leakage.

---

## ✅ Preprocessing Steps

1. **Train-test split**
2. **Feature scaling** using StandardScaler
3. **SMOTE oversampling** on training data only (inside pipeline)
4. Model training and evaluation

---

## ✅ Evaluation Metrics

We use:

* Accuracy
* Precision
* Recall
* F1-score (macro & weighted)
* Confusion Matrix

These metrics help evaluate performance on both majority and minority classes.

---

## ✅ Results Summary

All models performed well after proper preprocessing. Random Forest achieved:

* **Training Accuracy:** ~97.9%
* **Testing Accuracy:** ~97.9%
* Perfectly balanced generalization (no overfitting)

---

## ✅ Best Performing Model

**Random Forest Classifier** gave the highest and most stable performance:

* Strong recall for minority class
* High precision
* No overfitting
* Robust on imbalanced data

---

## ✅ Future Improvements

* Implement XGBoost or LightGBM
* Add hyperparameter optimization using GridSearchCV/RandomizedSearchCV
* Experiment with SMOTENC or ADASYN
* Deploy the model via FastAPI or Flask

---

## ✅ Project Structure (Example)
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
```
project_folder/
│-- data/
│-- notebooks/
│-- src/
│   │-- preprocessing.py
│   │-- model_training.py
│   │-- evaluation.py
│-- models/
│-- README.md
```

---

## ✅ How to Run

Install dependencies:

```
pip install -r requirements.txt
```

Run training:

```
python src/model_training.py
```

---

If you want, I can improve the README further:
✅ Add code examples
✅ Add diagrams
✅ Add model comparison tables
✅ Make it GitHub-ready
