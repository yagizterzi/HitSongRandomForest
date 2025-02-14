# 🎵 Hit Song Prediction with Machine Learning  

## 📌 Project Overview  
This project aims to predict whether a song will be a **hit** or **not** based on its **audio features** from Spotify.  
A song is classified as a **hit** if its **popularity score is greater than 50**.  

We use **Random Forest Classifier**, a powerful machine learning model, to perform this classification.  

---

## 📊 Dataset Information
The dataset consists of **114,000 songs** with the following features:  

| Column Name       | Description |
|-------------------|-------------|
| `track_id`       | Unique Spotify ID for each track |
| `artists`        | Names of the artists who performed the track |
| `album_name`     | Name of the album in which the track appears |
| `track_name`     | Title of the track |
| `popularity`     | Popularity score (0-100) |
| `duration_ms`    | Length of the track in milliseconds |
| `explicit`       | Boolean (1 = explicit, 0 = clean) |
| `danceability`   | Suitability of a track for dancing (0.0 - 1.0) |
| `energy`         | Intensity and activity of a track (0.0 - 1.0) |
| `key`            | Musical key of the track |
| `loudness`       | Overall loudness in decibels (dB) |
| `mode`           | Modality (1 = Major, 0 = Minor) |
| `speechiness`    | Presence of spoken words (0.0 - 1.0) |
| `acousticness`   | Acoustic confidence (0.0 - 1.0) |
| `instrumentalness` | Probability of a track being instrumental (0.0 - 1.0) |
| `liveness`       | Presence of an audience (0.0 - 1.0) |
| `valence`        | Positivity of the track (0.0 - 1.0) |
| `tempo`          | Estimated tempo (beats per minute - BPM) |
| `time_signature` | Estimated time signature (3 to 7) |

---

## 🎯 Goal: Predicting Hit Songs
We define a **hit song** as one with a **popularity score > 50**.  
Thus, we create a new **binary target variable**:  
- `hit = 1` → If `popularity > 50`  
- `hit = 0` → Otherwise  

---

## ⚙️ Methodology  

1️⃣ **Data Preprocessing**  
- Numerical values are scaled for better model performance.  
- The dataset is split into **training (80%)** and **testing (20%)** sets.  

2️⃣ **Model Selection & Training**  
- A **Random Forest Classifier** is used to classify songs as "hit" or "not hit".  
- The model learns patterns from features like **danceability, energy, valence, tempo**, etc.  

3️⃣ **Model Evaluation**  
- The accuracy of the model is measured.  
- Feature importance is analyzed to see which factors influence a hit song the most.  

4️⃣ **Hyperparameter Tuning**  
- **Grid Search** is used to optimize model parameters for better accuracy.  

---

## 🚀 How to Run the Project  

# Hit Song Prediction

## 1️⃣ Clone the Repository and Install Dependencies

```bash
git clone https://github.com/yourusername/HitSongRandomForest.git
cd HitSongRandomForest
pip install -r requirements.txt


