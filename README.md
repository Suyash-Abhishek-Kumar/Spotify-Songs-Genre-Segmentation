# 🎵 Spotify Song Genre Segmentation

This project explores the classification of songs into genres using machine learning models trained on audio feature data from Spotify. It aims to analyze how well various algorithms can distinguish between genres based on numerical attributes extracted from songs.

---

## 📌 Project Objective

The goal is to **predict the genre of a song** using key audio features like energy, danceability, tempo, and others. This helps in organizing large music datasets, building recommendation systems, and enhancing user experience in music platforms.

---

## 📂 Dataset

- **Source**: [Kaggle - Spotify Dataset 1921–2020, 160k+ Tracks](https://www.kaggle.com/datasets/mrmorj/spotify-dataset-19212020-160k-tracks)
- **Attributes Used**:  
  `danceability`, `energy`, `key`, `loudness`, `mode`, `speechiness`, `acousticness`, `instrumentalness`, `liveness`, `valence`, `tempo`, `duration_ms`

- **Target**: `track_genre` (Genre label)

---

## 🧠 Machine Learning Models

Several classification models were tested and compared:

| Model                  | Accuracy |
|-----------------------|----------|
| Logistic Regression   | ~54%     |
| K-Nearest Neighbors   | ~64%     |
| Decision Tree         | ~66%     |
| Random Forest         | ~73%     |
| Support Vector Machine| ~68%     |

> ✅ **Random Forest** performed the best with ~73% accuracy on test data.

---

## ⚙️ Project Workflow

1. **Data Cleaning & Preprocessing**
   - Removed nulls and duplicates
   - Selected numeric columns only
   - Encoded genres using Label Encoding
   - Normalized features using `StandardScaler`

2. **Model Training & Evaluation**
   - Split data into 80:20 train-test
   - Applied 5 ML models and compared accuracy
   - Visualized results using bar plots

3. **Genre Prediction**
   - A custom input form allows users to input values manually
   - Predicts the genre using the trained Random Forest model

---

## 📊 Visualization

- Heatmaps to show feature correlation
- Distribution plots for audio features
- Accuracy comparison bar chart

---

## 🛠️ Tech Stack

- Python 🐍  
- Jupyter Notebook 📒  
- Scikit-learn ⚙️  
- Pandas, NumPy, Matplotlib, Seaborn 📈

---

## 🚀 How to Run

1. Clone the repo  
   ```bash
   git clone https://github.com/yourusername/spotify-genre-segmentation.git
   cd spotify-genre-segmentation
2. Install dependencies
   ```bash
   pip install -r requirements.txt
3. Run the notebook
Open Minor_Project_SuyashAbhishekKumar.ipynb in Jupyter and run all cells.

