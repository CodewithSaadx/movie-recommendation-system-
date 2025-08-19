# movie-recommendation-system-
🎬 Movie Recommendation System built with Python &amp; Scikit-learn. Uses K-Means clustering on MovieLens movies.csv dataset to group films by genres. Demonstrates preprocessing (one-hot encoding), clustering, and visualization. Future work: content-based &amp; collaborative filtering.
# 🎬 Movie Recommendation System (Clustering + Future Upgrades)

## 📌 Project Overview
This project was built as part of my AI assignment.  
It uses **unsupervised learning (K-Means Clustering)** to group movies by genres.  
Although clustering is not a full recommendation system, it forms the foundation for one.  

## 🎯 Objectives
- Explore unsupervised machine learning
- Apply K-Means clustering to a real dataset
- Understand the difference between clustering and recommendation
- Lay the groundwork for a future **Content-Based Recommendation System**

## 📊 Dataset
- File: `movies.csv`
- Columns:
  - `movieId` → Unique ID for each movie
  - `title` → Movie title + release year
  - `genres` → One or multiple genres separated by `|`

(Source: [MovieLens Dataset](https://grouplens.org/datasets/movielens/))

## 🛠️ Preprocessing
- Split genres into lists
- Applied **One-Hot Encoding** using `MultiLabelBinarizer`
- Dropped non-numeric columns for clustering

## 🤖 Algorithm
- **K-Means Clustering** from `sklearn.cluster`
- Used the **Elbow Method** to determine optimal number of clusters
- Assigned each movie to a cluster based on its genre vector

## 📈 Results
- Movies grouped into clusters by genre
- Visualized clusters and inertia values
- Example: Action/Adventure movies grouped together, Romance/Drama in another

## ✅ Next Steps
- Add **cosine similarity** to turn clustering into a **Content-Based Recommender**
- Incorporate user ratings (`ratings.csv`) for **Collaborative Filtering**
- Experiment with PCA for dimensionality reduction

## 📦 Requirements
```bash
pip install pandas scikit-learn matplotlib seaborn
