🎵 Music Analytics & Machine Learning System
A Complete End-to-End ML Project with Streamlit Dashboard


📌 Overview

This project is a fully implemented Music Analytics & Machine Learning System built with Python, Scikit-Learn, Matplotlib, Seaborn, and Streamlit.
It includes:

🎼 A synthetic dataset (music_dataset.csv)
🤖 Popularity Prediction ML Model (Regression)
🎭 Mood Classification ML Model (Classification)
🎧 Content-Based Song Recommendation System
📊 Full Data Analysis & Visualization Module
🌐 Streamlit Dashboard for user interaction


🎼 Dataset Details

The dataset (music_dataset.csv) contains synthetic but realistic music metadata:
| Column           | Description                               |
| ---------------- | ----------------------------------------- |
| Track_ID         | Unique ID                                 |
| Song_Name        | Name of the track                         |
| Artist           | Artist name                               |
| Genre            | Genre category                            |
| Language         | Track language                            |
| Duration_Sec     | Song duration in seconds                  |
| Release_Year     | Year of release                           |
| Popularity_Score | Popularity metric (target for regression) |

🤖 Machine Learning Models
1️⃣ Popularity Prediction Model
File: music_ml/train_popularity.py
Model: RandomForestRegressor
Predicts: Popularity_Score
Input features: Genre, Language, Artist, Duration, Streams, Release Year
Outputs metrics: MAE
                 RMSE
                R² Score

 Run:

python music_ml/train_popularity.py
| Stream_Count     | Number of streams                         |
| Mood             | Mood label (for classification)           |


2️⃣ Mood Classification Model
File: music_ml/train_mood.py
Model: RandomForestClassifier
Predicts mood (Happy / Sad / Calm / Energetic / Romantic / Melancholic)
Prints classification report (Precision / Recall / F1)

Run:

python music_ml/train_mood.py


3️⃣ Content-Based Song Recommender

File: music_ml/recommender.py
Recommends songs similar to a given Track_ID using:
Cosine similarity
Genre one-hot encoding
Language encoding
Duration, Popularity, Streams

Run:

python music_ml/recommender.py


📊 Data Visualization (5 Graphs)

File: music_ml/trend_analysis.py
Includes:
Genre popularity over years
Top 15 artists
Popularity score distribution
Streams vs popularity scatter plot
Mood distribution pie chart

Run:

python music_ml/trend_analysis.py


🌐 Streamlit Web Application

File: app/streamlit_app.py

Features:

Explore dataset
Genre distribution chart
Predict song popularity
Get song recommendations
Mood classification info

Run:

streamlit run app/streamlit_app.py

🛠 Installation

Clone the repository:

git clone https://github.com/yourusername/music_project.git
cd music_project


Install dependencies:

pip install -r requirements.txt

🚀 Technologies Used

Python
Pandas
NumPy
Scikit-Learn
Matplotlib
Seaborn
Streamlit
Joblib

📘 Future Enhancements

Integrate Spotify API
Add Deep Learning models (TensorFlow/PyTorch)
Deploy Streamlit app online
Add lyric-based sentiment analysis
