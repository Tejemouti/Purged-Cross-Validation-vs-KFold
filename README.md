# Financial ML: Purged Cross-Validation vs. Standard K-Fold

This repository demonstrates why standard K-Fold Cross-Validation fails in financial time series and provides a production-ready implementation of **Purged K-Fold with Embargo**, as proposed by Marcos López de Prado.

## 🚀 Why this matters?
In finance, data is not IID (Independent and Identically Distributed). Standard CV leads to "ghost accuracy" due to:
1. **Serial Correlation:** Markets have memory.
2. **Label Leakage:** Overlapping windows share future information.

## 🛠 Features
- **Scikit-Learn Compatible:** Can be used directly with `GridSearchCV`.
- **Purging & Embargo:** Complete elimination of look-ahead bias.
- **Visual Proof:** Comparison of AUC scores showing the "Accuracy Illusion".

## 📦 Installation
```bash
pip install -r requirements.txt
