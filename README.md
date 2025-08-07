# SVM Classification for Mobile Price Prediction

## 🎯 Problem Statement and Goal of Project

This project demonstrates how a **Support Vector Machine (SVM)** classifier can be used to predict the **price range** of a mobile phone based on its specifications. The goal is not just to build a high-performing model, but to understand how SVM handles **multi-class classification** with structured tabular data.

---

## 🛠 Solution Approach

The project follows a full end-to-end machine learning workflow:

1. **Data Loading**:

   * Dataset: `mobile_prices.csv`
   * Target variable: `price_range` (0 to 3)

2. **EDA & Preprocessing**:

   * Checked for missing values (none found).
   * Performed correlation analysis using a heatmap.
   * Verified balanced distribution of price classes.

3. **Feature Selection**:

   * All columns except `price_range` were used as features (`X`).

4. **Train-Test Split**:

   * Used 80/20 split for training and evaluation.

5. **Modeling**:

   * Applied `sklearn.svm.SVC` for classification.
   * Used default kernel and hyperparameters for initial experimentation.

6. **Evaluation**:

   * Calculated **accuracy score** on the test set.
   * Achieved **94% accuracy** on unseen data.

---

## 🧰 Technologies & Libraries

* Python 3
* `pandas`, `numpy` — data preprocessing
* `matplotlib`, `seaborn` — EDA and correlation visualization
* `scikit-learn` — model training and evaluation

---

## 📁 Dataset Description

* **File:** `mobile_prices.csv`
* **Samples:** 2000 rows
* **Features:** 20 features such as battery power, RAM, camera specs, etc.
* **Target:** `price_range` (0 = low cost, 3 = very high cost)

All features are numerical, making it ideal for SVM input.

---

## ⚙️ Installation & Execution Guide

1. Ensure `mobile_prices.csv` is in the working directory.
2. Install required packages:

   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
3. Launch the notebook:

   ```bash
   jupyter notebook SVM.ipynb
   ```

---

## 📊 Key Results / Performance

* **SVM Classifier Accuracy**: **94%**
* Dataset was clean and well-distributed, ideal for classification.
* Strong correlation observed between RAM and price range — confirmed by the model's effectiveness.

---

## 📸 Screenshots / Sample Outputs

* 🧩 Correlation heatmap (using `sns.heatmap`)
* ✅ Value counts of `price_range`
* 📋 Model accuracy printed on test data

---

## 📚 Additional Learnings / Reflections

* This notebook primarily focuses on understanding **how SVM works** in multi-class problems.
* Emphasis was placed on **data exploration and preparation**, not hyperparameter tuning.
* Excellent for building intuition around **margin-based classifiers** like SVMs.
* Accuracy was achieved with **no parameter optimization**, showcasing how well SVM performs with clean, structured data.

---

## 👤 Author

## Mehran Asgari

**Email:** [imehranasgari@gmail.com](mailto:imehranasgari@gmail.com)
**GitHub:** [https://github.com/imehranasgari](https://github.com/imehranasgari)

---

## 📄 License

This project is licensed under the MIT License – see the `LICENSE` file for details.

---

> 💡 *Some interactive outputs (e.g., plots, widgets) may not display correctly on GitHub. If so, please view this notebook via [nbviewer.org](https://nbviewer.org) for full rendering.*

---
