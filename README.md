# 🎬 Movie Recommendation System

A **content-based movie recommendation system** built using metadata such as genres, cast, crew, and keywords. This project utilizes NLP techniques and cosine similarity to recommend similar movies based on user input.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Tech Stack](#tech-stack)
- [Dataset](#dataset)
- [How It Works](#how-it-works)
- [Getting Started](#getting-started)
- [Results & Visuals](#results--visuals)
- [Future Improvements](#future-improvements)
- [License](#license)

---

## 📖 Overview

This project demonstrates how a machine learning model can be used to suggest similar movies to a given movie title using only its metadata. It is an example of a **content-based filtering** approach.

🔍 **Problem Statement:**  
Given a movie title, return a list of top 5 similar movies based on content features such as genres, keywords, cast, and crew.

---

## 🛠 Tech Stack

- Python 🐍
- Pandas, NumPy – data manipulation
- Scikit-learn – CountVectorizer, cosine similarity
- Matplotlib, Seaborn – visualization
- WordCloud – tag visualization
- Jupyter Notebook

---

## 🎯 Dataset

Dataset used: [TMDB 5000 Movie Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

Files:
- `tmdb_5000_movies.csv`
- `tmdb_5000_credits.csv`

---

## ⚙️ How It Works

1. **Data Cleaning**: Merge the movies and credits datasets and extract important fields.
2. **Feature Engineering**: Extract keywords, genres, cast, and crew information and combine into a single `tags` column.
3. **Text Vectorization**: Convert tags into numerical vectors using `CountVectorizer`.
4. **Similarity Calculation**: Compute cosine similarity between movie vectors.
5. **Recommendation Function**: Input a movie title to get top 5 most similar movies.

---

## 🚀 Getting Started

### 1. Clone this repository

```bash
git clone https://github.com/Sumanta049/Movie_Recommender_ML.git
cd Movie_Recommender_ML

```

## 📊 Results & Visuals

- **Tag WordCloud**: Visualizes common words in the movie metadata
- **Sample Output**:

```
recommend('Avatar')

Top 5 recommended movies:
1. Guardians of the Galaxy
2. John Carter
3. Pirates of the Caribbean: At World's End
4. Battleship
5. Fantastic Four
```

---

## 🔮 Future Improvements

- Add **TF-IDF** based similarity for better recommendations
- Deploy as a **Streamlit web app**
- Build a **hybrid recommender** using user ratings
- Add **genre filters** or user profiles

---

## 📜 License

This project is licensed under the MIT License.

---
