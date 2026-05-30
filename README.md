# 🌸 Data Classification Using AI — Iris Species Classifier
### DecodeLabs AI Engineering Internship | Project 2 | Batch 2026

---

## 📌 Project Overview

Every intelligent system that makes decisions is — at its core — a classification engine.

This project moves beyond rule-based logic into the world of **Supervised Machine Learning.** Using the legendary Iris benchmark dataset, a full end-to-end ML pipeline was built from scratch — from raw data ingestion to model evaluation — using the **K-Nearest Neighbors (KNN) algorithm** to classify three species of Iris flowers with **100% accuracy.**

This project proves that machines can learn to make intelligent decisions not from hardcoded rules, but from **patterns in data.**

---

## 🎯 Project Goal

Build a supervised machine learning classification model that:
- Loads and explores a real dataset
- Visualizes feature relationships to inform algorithm selection
- Scales features for fair distance-based computation
- Splits data into training and testing sets
- Trains a KNN classifier to predict flower species
- Evaluates performance using Classification Report and Confusion Matrix

---

## 📊 Dataset — The Iris Benchmark

| Property | Details |
|---|---|
| 📦 Source | Built into scikit-learn (`sklearn.datasets`) |
| 🌸 Samples | 150 flowers |
| 🏷️ Classes | 3 (Setosa, Versicolor, Virginica) |
| 📐 Features | 4 (Sepal Length, Sepal Width, Petal Length, Petal Width) |
| ⚖️ Balance | Perfectly balanced — 50 samples per class |

No external download needed. The dataset is loaded directly from scikit-learn.

---

## 🏗️ ML Pipeline Architecture

```
RAW DATA (Iris Dataset)
        ↓
EXPLORATORY DATA ANALYSIS
— Shape, Info, Correlation
        ↓
VISUALIZATION
— Scatter Plot: Petal Length vs Petal Width
— Confirms class separability
        ↓
FEATURE SCALING
— StandardScaler (Mean=0, Variance=1)
— Scale only features, not target label
        ↓
TRAIN-TEST SPLIT
— 80% Training (120 samples)
— 20% Testing  (30 samples)
        ↓
MODEL TRAINING
— KNN Classifier (K=5)
        ↓
EVALUATION
— Classification Report
— Confusion Matrix
        ↓
RESULT: 100% Accuracy
```

---

## 🧠 Why KNN Was Chosen

During exploratory analysis, a scatter plot of petal length vs petal width revealed that the three flower classes form **completely distinct clusters** — each class is tightly grouped and surrounded exclusively by members of the same class.

This makes KNN the ideal algorithm because:

> *"If the closest data points to any given point are of the same color, they belong to the same class. KNN leverages this proximity principle — identifying which class a new data point belongs to based on the class of its nearest neighbors."*

KNN is a **distance-based algorithm** — it doesn't draw lines, it reads neighborhoods. For clearly separated clusters, this is the most natural and effective approach.

---

## 📈 Model Results

| Metric | Setosa | Versicolor | Virginica |
|---|---|---|---|
| Precision | 1.00 | 1.00 | 1.00 |
| Recall | 1.00 | 1.00 | 1.00 |
| F1 Score | 1.00 | 1.00 | 1.00 |

**Overall Accuracy: 100%**

The Confusion Matrix confirmed **zero misclassifications** across all 30 test samples.

This perfect result is consistent with the scatter plot analysis — the three classes are so distinctly separated that KNN (K=5) classified every single flower correctly.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core programming language |
| scikit-learn | Dataset, scaling, splitting, KNN, evaluation |
| pandas | Data manipulation and DataFrame operations |
| matplotlib | Data visualization (scatter plot, confusion matrix) |
| Jupyter Notebook | Interactive development environment |

---

## 🚀 How to Run

**Step 1 — Install required libraries**
```bash
pip install scikit-learn pandas matplotlib jupyter
```

**Step 2 — Clone this repository**
```bash
git clone https://github.com/yourusername/DecodeLabs-Project2-DataClassification.git
```

**Step 3 — Navigate to the folder**
```bash
cd DecodeLabs-Project2-DataClassification
```

**Step 4 — Launch Jupyter Notebook**
```bash
jupyter notebook
```

**Step 5 — Open and run**
```
Project_2_DecodeLabs.ipynb
```

Run all cells from top to bottom.

---

## 📂 Project Structure

```
DecodeLabs-Project2-DataClassification/
│
├── Project_2_DecodeLabs.ipynb   # Main notebook with full pipeline
└── README.md                    # Project documentation
```

---

## 🔍 Key Concepts Demonstrated

- **Supervised Learning** — model learns from labeled training data
- **Feature Scaling** — StandardScaler ensures fair distance computation
- **Train-Test Split** — 80/20 split for unbiased model evaluation
- **KNN Algorithm** — proximity-based classification
- **Confusion Matrix** — visual performance evaluation
- **F1 Score** — harmonic mean of precision and recall
- **EDA** — exploratory analysis to inform algorithm selection

---

## 📖 What I Learned

This project taught me that choosing the right algorithm is not guesswork — it comes from **understanding your data first.** By visualizing the scatter plot before writing a single line of model code, I was able to reason my way to KNN as the best algorithm based on what the data itself was showing me.

The most important skill in machine learning is not knowing every algorithm — it is knowing how to **read your data and let it guide your decisions.**

---

## 👩‍💻 Built By

**Mercy Inameti**
AI Engineering Intern — DecodeLabs Batch 2026
Project 2 | Data Classification Using AI 

---

*"We do not write the rules. We provide history, and the machine derives the logic." — DecodeLabs*

