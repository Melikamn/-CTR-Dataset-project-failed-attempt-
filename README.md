# -CTR-Dataset-project-failed-attempt-
پروژه‌ی شکست‌خورده CTR Dataset (نسخه اول)
 ❌ CTR Prediction – Attempt 1 (With Public Mini Dataset)

Status: Discontinued
*Reason: Incomplete Dataset / Access Limitations

---

# 🧠 Project Goal

The goal was to build a machine learning model to predict Click-Through Rate (CTR) using a publicly available dataset with minimal features.

Initially, the idea was to use standard preprocessing (encoding, feature engineering), train a few models using `scikit-learn`, and evaluate the pipeline on a binary classification task (`click` or `not click`).



# 📉 Why This Project Was Discontinued

Despite a promising start, the project ran into several roadblocks:

# 🧱 Challenges Faced

| Challenge | Description |
|----------|-------------|
| 🇮🇷 Data Access Issues | Due to being in Iran, access to many standard ML datasets (Kaggle, Google Datasets, etc.) was restricted or unstable |
| 📦 Incomplete Dataset | The available dataset was a small sample with limited rows and columns, lacking the richness of real ad click logs |
| 🧪 Unrealistic Results | The small dataset caused models to **overfit** easily, returning unrealistic metrics like 100% accuracy |
| ❌ Generalization Impossible | The limited diversity of data made it impossible to generalize to a real-world CTR problem |
| 🧹 Missing Feature Engineering Room | Many ID-based or categorical features were already encoded, limiting opportunities for learning data prep techniques |



# 🧪 What Was Tried

 ✅ Initial Steps Taken:

- ✅ Data loading, inspection
- ✅ Checking for missing values
- ✅ Label Encoding of categorical features
- ✅ Basic feature engineering (splitting hour, etc.)
- ✅ Train/test split
- ✅ Logistic Regression and Random Forest
- ✅ Classification reports, confusion matrix, ROC AUC

# Why it still didn’t work:

- The dataset had too few rows (1,000) and pre-processed columns
- Most identifiers (like `site_id`, `app_id`) were already encoded into `0` and `1`
- Binary values were too clean → led to 100% accuracy without real learning


# 🧭 Lessons Learned

> Even failure teaches more than success — this project taught me the importance of dataset **richness**, **scale**, and **source authenticity**.

- Always validate the **size and complexity** of a dataset before investing full effort
- Be careful of datasets that are already too processed — they offer less value for learning
- Document failures to improve future decision-making and planning


# 🔄 Pivot to New Plan

After hitting the above limitations, I pivoted the project to a larger, more realistic dataset:  
➡️ **[Criteo Display Advertising Challenge Dataset](https://www.kaggle.com/c/criteo-display-ad-challenge)**

This dataset contains over 4GB of real-world ad click data and allowed for:

- Working with missing values
- Real-world feature engineering
- Managing high-cardinality categorical features
- Scalability and deep learning compatibility



 🧱 Final Thoughts

This repository remains here as a **reminder of the learning process**, and how sometimes knowing when to **pivot** is the most strategic decision in a project.

# 🗂 Repo Contents

| File/Folder | Description |
|-------------|-------------|
| `notebooks/` | Jupyter notebooks used for early exploration |
| `src/`       | Scripts for encoding and preprocessing |
| `README.md` | This file — documenting the attempt and failure |
