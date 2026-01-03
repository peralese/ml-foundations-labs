 Tier 2 — Tabular ML Playground

## Purpose

This project is a **hands-on sandbox for classical machine learning on tabular data**.

The goal is **intuition over optimization**:
- Understand how different ML models behave
- Learn what actually improves performance
- Build comfort with the full ML workflow

This project intentionally avoids:
- Deep learning
- Domain-specific or enterprise use cases
- Over-engineering

---

## Learning Objectives

By completing this project, you should be able to:

- Load and explore a tabular dataset using Pandas
- Identify features and target variables
- Establish a simple baseline model
- Train and evaluate multiple classical ML models
- Compare results using appropriate metrics
- Explain *why* one model performs better than another

---

## Dataset

Use **one clean, well-known tabular dataset**.

Recommended options (pick **one**):

- **California Housing Dataset** (`sklearn.datasets`)
- **UCI Wine Quality Dataset**
- **UCI Heart Disease Dataset**
- A small, clean Kaggle dataset (≤ 50k rows)

**Rule:**  
Do *not* spend time cleaning a messy dataset.  
This project focuses on **models and evaluation**, not data wrangling.

---

## Project Structure

```
tier2_tabular_ml_playground/
├─ README.md
├─ notebooks/
│  └─ 01_tabular_baselines.ipynb
├─ src/
│  ├─ data_prep.py
│  ├─ train.py
│  └─ evaluate.py
└─ outputs/
   ├─ figures/
   └─ models/
```

You may complete the entire project inside the notebook.  
Moving logic into `src/` is optional.

---

## Baseline Workflow

### Step 1 — Data Exploration
- Load the dataset
- Inspect shape, columns, and basic statistics
- Identify:
  - Feature columns
  - Target variable
- Check for:
  - Missing values
  - Incorrect data types

---

### Step 2 — Train/Test Split
- Split the data into training and test sets
- Typical split: `80 / 20`
- Use a fixed `random_state` for reproducibility

---

### Step 3 — Baseline Model

Start with **one simple model**:

- Regression task → **Linear Regression**
- Classification task → **Logistic Regression**

Evaluate using appropriate metrics:

- **Regression**
  - RMSE
  - MAE
  - R²
- **Classification**
  - Accuracy
  - Precision
  - Recall
  - F1-score

This establishes your baseline.

---

## Model Experiments

Train **at least two additional models**, such as:

- Decision Tree
- Random Forest
- Gradient Boosting
- Support Vector Machine

Guidelines:
- Start with default hyperparameters
- Use the *same* train/test split
- Evaluate using the *same* metrics

Avoid heavy tuning at this stage.

---

## Evaluation & Comparison

Create a simple comparison:

- Table of models vs metrics
- Optional bar chart of performance

Answer these questions:
- Which model performed best?
- Which model was easiest to reason about?
- Which model would you choose in practice, and why?

---

## Stretch Goals (Optional)

Only attempt if you feel comfortable:

- Feature scaling
- Simple cross-validation
- Minimal hyperparameter tuning (1–2 parameters)

These are *nice to have*, not required.

---

## Deliverables

At minimum, this project should produce:

- `01_tabular_baselines.ipynb`
- A short written summary answering:
  - What worked?
  - What didn’t?
  - What surprised you?

Optional:
- Saved model artifacts in `outputs/models/`
- Plots in `outputs/figures/`

---

## Completion Criteria

You can mark this project **COMPLETE** when:

- You trained **three or more models**
- You compared them using correct metrics
- You can explain your results without referencing the code

No polish required.

---

## Notes

This project is meant to be:
- Low pressure
- Fast to complete
- Confidence building

Perfection is not the goal.  
**Understanding is.**


