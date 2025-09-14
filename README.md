# 🎬 Movie Recommendation System

[![Python](https://img.shields.io/badge/Python-3.12-blue)](https://www.python.org/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.30-orange)](https://streamlit.io/)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

A **content-based movie recommendation system** built with **Python, Streamlit, and machine learning**.  
Get personalized movie suggestions along with posters. Fully offline-ready once posters are cached locally.

---

## 📌 Features

- Select any movie from the dataset and get **top 10 similar movies**.
- Displays **movie posters** alongside movie titles.
- Fully **offline-ready** with pre-downloaded poster images.
- Easy-to-use **Streamlit interface** with a responsive 2x5 grid layout.
- Content-based recommendation using **cosine similarity** on movie **tags** (`overview + genres`).
- Compatible with **local datasets** and can handle large movie collections.

---

## 🛠 Tech Stack

- **Python 3.12**
- **Streamlit** – Frontend UI
- **Pandas** – Data manipulation
- **scikit-learn** – Cosine similarity computation
- **pickle** – Storing preprocessed movie data
- **Requests** – Fetching posters (optional, during preprocessing)
- **Git LFS** – Tracking large `.pkl` files

---

## ⚡ Setup Instructions

1. **Clone the repo**
git clone https://github.com/Eidaan/MRS.git
cd MRS
pip install -r requirements.txt
streamlit run app.py #run the streamlit app

---

## 🏞 Screenshot

<img width="1912" height="867" alt="image" src="https://github.com/user-attachments/assets/c827bc7a-8c67-4e82-8d21-6ca56b96413e" />

## 📁 Notes

- `movie_data.pkl` is a **large file (~178 MB)**. It is tracked using **Git LFS**. Make sure Git LFS is installed when cloning the repo.
- Once posters are downloaded via `prepare_data.py`, the system works **fully offline**.

### Optional Improvements

- Hybrid recommendation (content + collaborative filtering)
- Search bar with autocomplete
- Genre or year filters
- Ratings display

---

## 📜 References

- TMDB API: [https://www.themoviedb.org/documentation/api](https://www.themoviedb.org/documentation/api)
- scikit-learn Cosine Similarity: [https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html)
- Streamlit Docs: [https://docs.streamlit.io/](https://docs.)

## 🗂 Project Structure

