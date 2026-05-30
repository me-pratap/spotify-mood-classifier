# 🎵 Spotify Song Mood Classifier

A deep learning project that classifies songs into moods — **Happy, Sad, Angry, Calm** — using audio features from Spotify.

## 📌 Overview
Built a feedforward neural network trained on 114,000 Spotify tracks to predict the mood of any song based on its audio characteristics.

## 🎯 Accuracy
**99.52%** on 22,800 unseen songs

## 🧠 Model Architecture
- Input Layer: 9 audio features
- Hidden Layer 1: 128 neurons (ReLU)
- Hidden Layer 2: 64 neurons (ReLU)
- Hidden Layer 3: 32 neurons (ReLU)
- Output Layer: 4 neurons (Softmax)

## 🧠 My Input
- epochs=10
- batch_size=120

## 📊 Features Used
- Danceability, Energy, Loudness, Speechiness
- Acousticness, Instrumentalness, Liveness, Valence, Tempo

## 🛠️ Tech Stack
- Python, TensorFlow/Keras
- Pandas, NumPy, Scikit-learn
- Matplotlib, Jupyter Notebook

## 📁 Dataset
[Spotify Tracks Dataset](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset) — 114,000 songs, 21 features

## 🚀 How to Run
1. Clone this repository
2. Install requirements: `pip install tensorflow pandas numpy scikit-learn matplotlib`
3. Open `spotify_mood_classifier.ipynb` in Jupyter Notebook
4. Run all cells

## 👤 Author
**Pratap** — [GitHub](https://github.com/me-pratap)
