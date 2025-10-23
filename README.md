# Movie Recommendation System

This project builds a user-based collaborative filtering system to recommend movies to users based on their past ratings. The workflow includes data preprocessing, train-test split, user similarity computation, rating prediction, and evaluation using Precision@5 as the main metric.

---

## Objective
Develop a recommendation system to suggest movies to users, evaluate performance using Precision@5, and explore improvements using user-based normalization.

---

## Project Structure
```
|- results/
   |- evaluation.csv
|- src/
   |- movie_recommendation_system.ipynb
|- .gitignore
|- README.md
|- requirements.txt
```

---

## Methodology
- **Dataset:** MovieLens 100K Dataset (via KaggleHub)  
- **Preprocessing:** Merge ratings with movie titles, create user-item matrices, fill missing ratings with 0  
- **Normalization:** Subtract each user’s mean rating to account for user bias  
- **Train-Test Split:** 80% train, 20% test  
- **User Similarity:** Cosine similarity between users based on normalized ratings  
- **Prediction:** Weighted average of ratings from top-N similar users  
- **Recommendation:** Top-K movies predicted for each user  
- **Evaluation:** Precision@5 for all users, with visualizations (histogram & boxplot)

---

## How to Run
1. Clone the repository:
   ```bash
   git clone <repo-url>
   cd <repo-name>
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the notebook:
   ```bash
   jupyter notebook src/movie_recommendation_system.ipynb
   ```

---

## Author
**Tasneem Helal**  
Mechatronics Engineer | Machine Learning & Recommender Systems Enthusiast  
[LinkedIn](https://linkedin.com/in/tasneemhelal) | [GitHub](https://github.com/Tasneem-Helal)
