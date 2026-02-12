# AI-ML-INTENSHIP-TASK--15
End-to-End Machine Learning Pipeline
#  Breast Cancer Classification using ML Pipeline

##  Project Overview
This project demonstrates how to build a complete **Machine Learning Pipeline** using Scikit-learn for Breast Cancer classification.

The pipeline includes:
- Feature preprocessing (Scaling + Encoding)
- ColumnTransformer
- Logistic Regression model
- Model evaluation
- Saved trained pipeline model

---

##  Dataset
- Dataset file: `breast-cancer.csv`
- Target variable: `diagnosis`
- Problem Type: **Binary Classification**

---

## ⚙️ Project Workflow

### 1️ Load Dataset
- Load dataset using Pandas.
- Separate features (X) and target variable (y).

### 2️ Feature Identification
- Identify numerical features
- Identify categorical features

### 3️ Preprocessing (ColumnTransformer)
- Apply `StandardScaler` to numerical features
- Apply `OneHotEncoder` to categorical features

### 4️ ML Pipeline
- Combine preprocessing and Logistic Regression model using `Pipeline`

### 5️ Train-Test Split
- Split dataset using `train_test_split`
- Stratified sampling applied

### 6️ Model Training
- Train pipeline using training data

### 7️ Evaluation Metrics
Model evaluated using:
-  Accuracy
-  Precision
-  Recall
-  F1-score

---

##  Evaluation Metrics

Example Output:

```
Accuracy : 0.97+
Precision: 0.97+
Recall   : 0.97+
F1-score : 0.97+
```

> Note: Exact values may vary slightly depending on random state.

---

##  Technologies Used

- Python
- Pandas
- Scikit-learn
- Jupyter Notebook

---

##  Project Structure

```
│── ML_Pipeline_Breast_Cancer.ipynb
│── breast_cancer_pipeline.pkl
│── breast-cancer.csv
│── README.md
```

---

##  Saved Model

The trained pipeline model is saved as:

```
breast_cancer_pipeline.pkl
```

###  Load Saved Model

```python
import pickle

with open("breast_cancer_pipeline.pkl", "rb") as f:
    model = pickle.load(f)

predictions = model.predict(X_new)
```

---

##  How to Run

1. Clone this repository
2. Install dependencies:

```bash
pip install pandas scikit-learn
```

3. Run the notebook:

```bash
jupyter notebook ML_Pipeline_Breast_Cancer.ipynb
```

---

##  Key Learning Outcomes

- End-to-end ML Pipeline creation
- ColumnTransformer usage
- Combining preprocessing + model
- Proper model evaluation
- Saving and loading trained models

---

##  Author
**Jaasiel Mark**

