### README.md

```markdown
# Movie Recommendation System 🎬

A live, interactive machine learning application that suggests movies based on content similarity. This project leverages Natural Language Processing (NLP) to analyze movie metadata and provides a seamless user experience through a web-based interface.

**🔗 Live Demo:**  
👉 [Try the Movie Recommendation App](https://movierecommendation-4bn6n5byk3akrxdjtsrssr.streamlit.app)


## 🚀 Overview
This system identifies the relationship between movies using metadata such as genres, keywords, cast, and crew. By calculating the mathematical "distance" between films, it can suggest titles that are most similar to a user's selection.

## 🛠️ Tech Stack
- **Frontend & Deployment:** Streamlit, Streamlit Cloud
- **Machine Learning:** Scikit-learn (CountVectorizer, Cosine Similarity)
- **Data Manipulation:** Pandas, NumPy, Python
- **Natural Language Processing:** NLTK (Stemming)
- **External API:** The Movie Database (TMDB) for real-time poster fetching

## 📂 Key Files
- `app.py`: The core Streamlit application handling the UI and API calls.
- `movie_recommender.ipynb`: The end-to-end data science pipeline from raw CSV to a similarity matrix.
- `similarity.pkl`: Compressed similarity scores for optimized performance on the web.
- `movie_dict.pkl`: Processed movie data used for the search and selection interface.

## ⚙️ How It Works
1.  **Vectorization:** Movie tags are converted into a 5,000-dimensional vector space using `Bag of Words`.
2.  **Similarity Analysis:** The app utilizes **Cosine Similarity** instead of Euclidean distance to measure the angle between movie vectors, ensuring accuracy regardless of tag length.
3.  **Real-time Fetching:** When a recommendation is generated, the app calls the TMDB API to retrieve high-resolution posters for a more visual user experience.

## 💻 Local Setup

1. **Clone the repo:**
   ```bash
   git clone [https://github.com/AashishBedi/Movie_Recommendation.git](https://github.com/AashishBedi/Movie_Recommendation.git)

```

2. **Install dependencies:**
```bash
pip install -r requirements.txt

```


3. **Run the app:**
```bash
streamlit run app.py

```



## 🤝 Contact

Developed by **Aashish Bedi** *Computer Science & Engineering Student*
https://www.linkedin.com/in/aashishbedi/
