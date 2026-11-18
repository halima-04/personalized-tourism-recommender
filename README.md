# Personalized and Context-Aware Tourism Recommendation System

**Student:** Halima Mahdi Mohammed | **ID:** 670315

**Institution:** United States International University–Africa (USIU-Africa)

**Programme:** BSc Data Science and Analytics

## What this project is about

Online tourism platforms list many attractions, and travelers struggle to find ones that fit their own interests. This project builds a recommender that returns a ranked **Top-5 list of tourist attractions** for a traveler, using past user ratings, attraction characteristics and the traveler's current preferences (attraction type and visit mode). Each recommendation comes with a short explanation, for example "similar to an attraction you rated highly".

## Approaches

1. **Popularity baseline:** rank by interaction count and/or average rating.
2. **Content-based filtering:** recommend attractions similar (cosine similarity) to ones the user rated highly, using type and location features.
3. **Collaborative filtering with matrix factorization (SVD):** learn latent user and attraction patterns from the user-item rating matrix.
4. **Hybrid, context-aware:** `Hybrid Score = α · Content + (1 − α) · Collaborative`, then filter or re-rank by the selected attraction type and visit mode.

## Dataset

[Tourism Dataset from Historical Transactions for Recommender Systems](https://data.mendeley.com/datasets/h58s544674/1) (Mendeley Data): 9 Excel files, **52,930 transactions, 33,530 users, 30 attractions** in Bali, Malang and Yogyakarta, ratings 1–5, 2013–2022.



## Evaluation

Time-aware train/test split, comparing all models on the same split using Precision@K, Recall@K, NDCG@K and catalogue coverage.

## Tools

Python, Pandas, NumPy, Scikit-learn, Surprise/implicit (matrix factorization), Streamlit, Git/GitHub.

Repository: https://github.com/halima-04/personalized-tourism-recommender
