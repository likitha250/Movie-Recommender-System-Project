📘 README.md
# 🎬 Movie Recommender System

A **content-based movie recommendation system** built using Python and the TMDB movie metadata dataset.  
The system recommends movies similar to a given movie based on textual features such as genres, keywords, cast, and crew.

---

## 🚀 Features

- Content-based filtering
- Uses cosine similarity for recommendations
- Processes TMDB movies & credits datasets
- Recommends top 5 similar movies
- Saves trained data using pickle for reuse

---

## 🧠 How It Works

1. **Data Loading**
   - TMDB Movies Dataset
   - TMDB Credits Dataset

2. **Preprocessing**
   - Merge movies and credits
   - Extract:
     - Genres
     - Keywords
     - Top cast members
     - Director
   - Clean and normalize text data

3. **Feature Engineering**
   - Combine all features into a single `tags` column
   - Vectorize text using `CountVectorizer`

4. **Similarity Calculation**
   - Compute cosine similarity between movies

5. **Recommendation**
   - Given a movie title, return the top 5 most similar movies

---

## 📂 Project Structure



Movie_Recommender_System_Project.ipynb
movie_list.pkl
similarity.pkl
README.md


---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Pickle
- KaggleHub

---

## 📌 Usage

Run the notebook and use the recommendation function:

```python
recommend('Gandhi')

Output Example
Gandhi
The Legend of Bhagat Singh
Lagaan
Swades
Jodhaa Akbar

💾 Saved Files

movie_list.pkl → Processed movie data

similarity.pkl → Cosine similarity matrix

These can be used directly in a web app (e.g., Streamlit or Flask).

📊 Dataset

Source: TMDB Movie Metadata (via Kaggle)

Includes:

Movies

Credits

Genres

Keywords

🔮 Future Improvements

Add collaborative filtering

Deploy with Streamlit

Add poster images using TMDB API

Improve recommendations with TF-IDF or embeddings

👨‍💻 Author

Developed as a machine learning project for learning recommendation systems.
