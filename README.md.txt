# 🎵 Spotify Song Mood Classifier

A deep learning project that classifies songs into moods — **Happy, Sad, Angry, Calm** — using audio features from Spotify.

## 📌 Overview
Built a feedforward neural network trained on 114,000 Spotify tracks to predict the mood of any song based on its audio characteristics.
Mood labels were rule-derived from valence and energy thresholds (e.g., high valence + high energy → "happy"), rather than manually annotated. This project demonstrates the network's ability to learn and approximate that decision boundary from raw audio features.

## 🎯 Accuracy
99.52% on 22,800 unseen songs — expected to be high since the labeling rule was itself a function of two of the input features (valence, energy).

## 🧠 Model Architecture
- Input Layer: 9 audio features
- Hidden Layer 1: 128 neurons (ReLU)
- Hidden Layer 2: 64 neurons (ReLU)
- Hidden Layer 3: 32 neurons (ReLU)
- Output Layer: 4 neurons (Softmax)

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

⚠️ Notes
Since mood labels were derived directly from valence and energy, the model partially learns to reconstruct a known rule rather than solving a fully independent prediction problem. A harder, leakage-free variant (excluding valence/energy from inputs) is a planned future iteration.

## 👤 Author
**Pratap** — [GitHub](https://github.com/me-pratap)
