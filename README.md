# Netfilx_Recommendation_System

# 🎬 Netflix Movie Recommender (Content-Based)

This project is a **Content-Based Movie Recommendation System** built using Python, Flask, and machine learning techniques. It recommends similar movies available on Netflix based on user input, using metadata such as title, cast, director, genre, and description.

## 📂 Project Structure

```
📦 netflix-recommender
├── app.py                   # Flask application for web interface
├── Content Based NRC.ipynb  # Jupyter notebook for EDA and model development
├── netflix_titles.csv       # Netflix movie and TV show metadata dataset
│── index.html           # HTML form to enter movie name
|── result.html          # HTML table for displaying recommendations
```
## 💡 How It Works

- **Data Cleaning:** Movie metadata (title, director, cast, genre, description) is cleaned and preprocessed.
- **Feature Engineering:** A "soup" of all text metadata is created for each movie.
- **Vectorization:** The `CountVectorizer` transforms text data into vectors.
- **Similarity Calculation:** Cosine similarity is used to find similar movies.
- **Web App:** Users can input a movie name, and the Flask app returns the top 10 most similar titles.

## 🚀 How to Run the Project

1. **Install Requirements**
   ```bash
   pip install flask pandas scikit-learn
   ```

2. **Run the App**
   ```bash
   python app.py
   ```

3. **Open in Browser**
   Navigate to `http://127.0.0.1:5000/` in your browser.

## 🧪 Notebook: `Content Based NRC.ipynb`

This notebook contains:
- Exploratory data analysis (EDA)
- Content-based filtering logic
- Visualizations and data profiling
- Development of the recommendation logic before deployment

## 📊 Dataset

- File: `netflix_titles.csv`
- Source: [Netflix Movies and TV Shows](https://www.kaggle.com/shivamb/netflix-shows)
- Contains metadata like `title`, `director`, `cast`, `listed_in`, `description`, etc.

## 📷 Sample Input

- User enters: `Inception`
- Output: Top 10 movies similar to "Inception" based on content metadata

## 🌐 Technologies Used

- Python
- Flask
- Pandas
- Scikit-learn
- HTML/CSS

## 📌 Note

- Make sure the movie name you enter matches one in the dataset.
- The recommendation is purely content-based (no user ratings or collaborative filtering involved).
