#  Movie Recommendation System

This project is a Movie Recommendation System built using Python, Streamlit, and machine learning techniques. It recommends movies similar to the one selected by the user, based on precomputed similarity scores and the TMDB API for fetching posters.

## Features
- Recommend top 5 similar movies based on the selected movie
- Display movie posters using the TMDB API
- Uses a precomputed similarity matrix
- Interactive UI with Streamlit
- Dynamic dropdown for movie selection

## Project Structure
MovieRecommendationSystem/
│── app.py
│── main.py
│── Main.ipynb
│── dataset.csv
│── movies_list.pkl
│── similarity.pkl
│── .gitignore
│── .gitattributes
│── README.md


## Installation & Setup
git clone https://github.com/shivanirao18/MovieRecommendationSystem.git
cd MovieRecommendationSystem
python -m venv venv
venv\Scripts\activate  #windows
source venv/bin/activate  #Mac/Linux
pip install -r requirements.txt
streamlit run app.py

## How It Works
The dataset (dataset.csv) contains movie information
Movies are vectorized and a similarity matrix is computed (similarity.pkl)
When a user selects a movie, the app fetches the top 5 most similar movies
Posters are retrieved via the TMDB API and displayed in the app

## Future Improvements
Hybrid recommendation (content + collaborative filtering)
More filters like genre, rating, release year
Deploy on Streamlit Cloud, Heroku, or AWS
