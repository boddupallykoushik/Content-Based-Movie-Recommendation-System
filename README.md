# Movie Recommendation System

This is a simple movie recommendation system I built using Python. It suggests movies based on the *genre* and *overview* (description) of a selected movie.

When you pick a movie, the system compares its genre and overview with other movies in the dataset and recommends a few that are most similar. I used Streamlit for the web interface, pickle to store the processed data, and requests to optionally fetch movie posters or extra details from an external API like TMDb.

---

## Why I Made This

I’ve always been curious about how platforms like Netflix or YouTube suggest content. So I tried building my own basic version using content-based filtering. This project helped me understand how to process text data, calculate similarity between items, and build an end-to-end ML-powered web app.

---

## Tools & Libraries Used

- Python  
- Pandas  
- Scikit-learn  
- Streamlit  
- Pickle (for saving/loading vectorizer and similarity matrix)  
- *Requests* (for fetching movie posters or external info)

---

## How It Works

1. Loads a dataset with movie titles, genres, and overviews.
2. Combines the genre and overview into a single string for each movie.
3. Uses CountVectorizer to turn this combined text into numerical vectors.
4. Computes cosine similarity between all movie vectors.
5. Saves the vectorizer and similarity matrix using pickle for faster loading.
6. When a user selects a movie, the app recommends the top 5 most similar ones.
7. Optionally, it uses the requests library to fetch movie posters or metadata from APIs (like TMDb).

---

## How to Run the App

1. *Clone the repository:*
   bash
   git clone https://github.com/your-username/movie-recommender.git
   cd movie-recommender

2. Install the dependencies:

pip install -r requirements.txt


3. Run the app:

streamlit run app.py


4. Open your browser at http://localhost:8501




---
Features:

Suggests movies using genre + overview similarity

Uses cosine similarity and CountVectorizer

Pre-processed with pickle for fast loading

Optionally fetches posters using requests

Clean, interactive UI built with Streamlit



---
Future Improvements:

Display posters and more movie info in the UI

Add filters like release year, rating, or language

Try TF-IDF or embeddings for smarter recommendations

Explore collaborative filtering or hybrid approaches

Deploy publicly using Streamlit Cloud



---
About Me:

Hi! I'm Koushik Boddupally, a B.Tech student in Computer Science (AI & ML) from Hyderabad. I enjoy learning by building projects that apply what I learn in a practical way. This one helped me explore how simple NLP techniques can create useful tools.

LinkedIn: linkedin.com/in/koushik-boddupally-2a2a39286



---

Thanks for checking out my project!
Feel free to try it, fork it, or suggest improvements 😊

---

### Final To-Do Checklist for You:

- Save this as `README.md` in your repo.
- Replace `your-username` with your actual GitHub username.
- Add a `requirements.txt` with:
  txt
  streamlit
  pandas
  scikit-learn
  requests

Make sure your repo contains:

app.py (Streamlit app)

vectorizer.pkl, similarity.pkl (if used)

movies.csv (your dataset)



Let me know if you want help:

Writing or organizing your actual code files

Deploying it to Streamlit Cloud

Creating a nice GitHub banner or preview GIF


Ready when you are!
