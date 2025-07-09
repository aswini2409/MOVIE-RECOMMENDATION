# 🎬 Simple Movie Recommendation System (No CSV Required)

This is a simple **content-based movie recommender system** built using **Python**, `pandas`, and `scikit-learn`. It suggests similar movies based on **genre similarity** using **cosine similarity**, without the need for any external datasets (no CSV files required).

---

## 📌 Features

- Recommends top similar movies based on genre.
- Uses `CountVectorizer` and `cosine_similarity` from scikit-learn.
- Movie dataset is defined directly in the Python code.
- Lightweight, clean, and easy to understand.
- Perfect for learning recommendation system fundamentals.

---

## 🛠️ Technologies Used

| Technology     | Purpose                            |
|----------------|------------------------------------|
| Python         | Core programming language          |
| pandas         | For data handling and manipulation |
| scikit-learn   | For vectorization and similarity   |
| Jupyter / VSCode / Terminal | Development & Execution    |

---

## 🚀 How to Run

1. **Install Required Packages** (if not already installed):
   ```bash
   pip install pandas scikit-learn
2.  Save the script as movie_recommender.py.
3.  Run the script:
    python movie_recommender.py
4. You’ll see movie recommendations printed in the terminal for predefined titles.


🧠 How It Works

1.A small movie dataset (title + genres) is manually created in a list.

2.The genres are converted into vectors using CountVectorizer.

3.Cosine similarity measures how close each movie is to the input.

4.The function recommend(movie_title) prints the top 5 most similar movies.


**📋 Sample Output**
**
Movie Dataset:**
               title                    genres
0            Titanic             Romance Drama
1  Avengers: Endgame     Action Adventure Sci-Fi
2      The Notebook             Romance Drama
3         John Wick            Action Thriller
4       Interstellar     Adventure Sci-Fi Drama
5      The Conjuring            Horror Thriller
6           Deadpool           Action Comedy
7         La La Land      Romance Music Drama
8          Inception      Action Sci-Fi Thriller
9       The Godfather               Crime Drama

**Recommendations for 'Titanic':**
- The Notebook (Similarity: 1.00)
- La La Land (Similarity: 0.71)
- Interstellar (Similarity: 0.50)
- The Godfather (Similarity: 0.50)
- Avengers: Endgame (Similarity: 0.00)

