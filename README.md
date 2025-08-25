# 🎬 Movies Recommendation

A **movie recommendation system** developed in Python within a *Jupyter Notebook*.  
The goal is to explore classic recommendation approaches (collaborative filtering and/or content-based) and build a reproducible pipeline for preprocessing, training, and evaluation.

> Repository: `TatisVivas/Movies-Recommendation`

---

## ✨ Features
- Data exploration and cleaning (ratings, movie metadata).
- Construction of user profiles and/or item similarities.
- Possible approaches:
  - **Content-based**: similarity by genres, keywords, or embeddings.
  - **Collaborative filtering**: *user–user*, *item–item*, or matrix factorization (SVD).
- Common evaluation metrics: RMSE, MAE, Precision@K, Recall@K.
- Self-explanatory notebook: `moviesRecommendation.ipynb`.

---

## 🗂️ Repository structure
```
.
├─ moviesRecommendation.ipynb   # Main notebook with the complete workflow
└─ .gitattributes
```

> If you add folders like `data/`, `src/` or `reports/`, update this block.

---

## 📦 Requirements

Make sure you have Python 3.9+ and Jupyter installed. Typical dependencies:

```bash
pip install numpy pandas scikit-learn scipy jupyter ipykernel
# Optional
pip install matplotlib seaborn implicit lightfm sentence-transformers
```

---

## 🚀 How to run

1. Clone the repo:
   ```bash
   git clone https://github.com/TatisVivas/Movies-Recommendation.git
   cd Movies-Recommendation
   ```

2. (Optional) Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   # Windows
   .venv\Scripts\activate
   # macOS/Linux
   source .venv/bin/activate
   ```

3. Install dependencies (see previous section).

4. Open the notebook:
   ```bash
   jupyter notebook moviesRecommendation.ipynb
   ```

5. Run all cells in order (Kernel → Restart & Run All).

---

## 🧠 Dataset

This project is designed to work with:
- **MovieLens** datasets (ML-100k / ML-1M) or any ratings dataset with the schema `userId, movieId, rating, timestamp`.  
- Movie metadata: title, genres, synopsis.  
- You can also use your own CSV file by adjusting paths and column names in the notebook.

---

## 📊 Evaluation

- **Rating prediction**: RMSE, MAE.  
- **Top-N recommendation**: Precision@K, Recall@K, MAP@K, NDCG@K.  
- **Baselines**: global average, per-user or per-item average.  

---
