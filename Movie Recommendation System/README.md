# 🎬 Movie Recommendation System (MovieLens 100K — u1.base / u1.test)

## Project Overview
A Movie Recommendation System that suggests movies to users using similarity-based collaborative filtering and matrix factorization.  
This project uses the MovieLens 100K dataset (pre-split files `u1.base` and `u1.test`) and movie metadata (`u.item`) to:

- Build a **user–item rating matrix**,
- Implement **user-based** and **item-based** collaborative filtering (cosine similarity),
- Implement a **matrix factorization** baseline using SVD (TruncatedSVD),
- Evaluate models using **Precision@K**, and
- Produce top-K recommendations for any user.

---

## Covered Topics
- **NumPy** — array and numerical operations used for matrices and computations.  
- **Pandas** — data loading and preprocessing.  
- **Scikit-learn** — `cosine_similarity` and `TruncatedSVD` for SVD baseline.  
- **Recommendation systems** — collaborative filtering (user-based and item-based).  
- **Similarity-based modeling** — cosine similarity on the user-item matrix.  
- **Bonus implemented**:
  - Item-based collaborative filtering ✅  
  - Matrix factorization (SVD) ✅

---

## Dataset
Use the MovieLens 100K dataset. For this project we assume you have these files in the working directory (or uploaded to Google Colab):

- `u1.base` — training ratings (tab-separated: `user_id\titem_id\trating\ttimestamp`)  
- `u1.test` — test ratings (same format)  
- `u.item` — movie metadata (pipe-separated; first two columns are `movie_id|title|...`)

If you have the full `ml-100k` folder you can use `u1.base`/`u1.test` or merge other splits as needed.

---

## Repository Structure (suggested)
movie-recommender/
│
├── movie_recommendation_notebook.ipynb # Main notebook (Colab-ready)
├── README.md # This file
├── requirements.txt # pip install -r requirements.txt
├── data/
│ ├── u1.base
│ ├── u1.test
│ └── u.item
└── utils/
└── recommenders.py # Optional: functions for reuse

yaml
Copy
Edit

---

## Requirements
Python 3.8+ and these packages:
pandas
numpy
scikit-learn
matplotlib

csharp
Copy
Edit
Install with:
```bash
pip install -r requirements.txt
# or
pip install pandas numpy scikit-learn matplotlib
How to run (Google Colab / Local)
In Google Colab
Create a new Colab notebook.

Upload u1.base, u1.test, and u.item via the Files sidebar OR mount your Google Drive and copy files into /content/.

Copy the cells from movie_recommendation_notebook.ipynb (or paste code blocks from the provided notebook) and run cells in order.

Locally (Jupyter)
Place u1.base, u1.test, and u.item in the working directory (or update paths).

Open and run the notebook movie_recommendation_notebook.ipynb.

What the notebook does (high level)
Load data from u1.base (train) and u1.test (test), and u.item for movie titles.

EDA — ratings distribution and ratings-per-user histograms.

Build user–item matrices for train & test (dense NumPy arrays).

Compute similarities:

User–user cosine similarity (for user-based CF)

Item–item cosine similarity (for item-based CF)

Predict ratings with:

User-based CF (top-k similar users),

Item-based CF (top-k similar items),

SVD baseline (TruncatedSVD reconstruction).

Evaluate using Precision@K (treat ratings ≥ 4 as relevant).

Recommend top-K unseen movies for a user and map IDs to movie titles.

Key functions (examples)
Below are brief examples that are included in the notebook:

Load train/test

python
Copy
Edit
train = pd.read_csv('u1.base', sep='\t', names=['user_id','item_id','rating','timestamp'])
test  = pd.read_csv('u1.test',  sep='\t', names=['user_id','item_id','rating','timestamp'])
movies = pd.read_csv('u.item', sep='|', header=None, encoding='latin-1')[[0,1]].rename(columns={0:'movie_id',1:'title'})
Compute user similarity

python
Copy
Edit
from sklearn.metrics.pairwise import cosine_similarity
user_sim = cosine_similarity(R_train)
np.fill_diagonal(user_sim, 0.0)
Recommend top-K

python
Copy
Edit
def recommend_topk(pred_matrix, user_id, K=10):
    u = user_map[user_id]
    scores = pred_matrix[u]
    seen = R_train[u] > 0
    scores[seen] = -np.inf
    top_idx = np.argsort(scores)[-K:][::-1]
    return [inv_item_map[i] for i in top_idx]
Evaluation
Metric used: Precision@K (recommended top-K items — fraction relevant among top K).

Relevance threshold: rating ≥ 4 (adjustable).

The notebook prints Precision@5, Precision@10, Precision@20 for each method (userCF, itemCF, SVD).

Tips & Improvements (for better results)
Mean-centering: subtract user mean ratings before similarity to reduce bias.

Shrinkage: apply significance weighting to similarity (account for number of co-rated items).

Use surprise library for robust MF (SVD++), cross-validation, and RMSE evaluation.

Implicit feedback: use ALS (e.g., implicit library) if you only have implicit interactions.

Cross-fold evaluation: run across all u*.base / u*.test folds for stable results.

Example Output (sample)
mathematica
Copy
Edit
Precision@5: userCF=0.1200, itemCF=0.1050, SVD=0.1350
Top 10 recommendations for user 1:
1. Star Wars (1977)
2. Raiders of the Lost Ark (1981)
3. Back to the Future (1985)
...
(actual titles and scores will depend on your split and parameters)

Authors & Contact
Your Name (e.g., Hamna Munir)
Email: your.email@example.com
LinkedIn: https://www.linkedin.com/in/yourprofile
