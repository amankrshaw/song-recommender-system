# Song Recommender System

This project is a simple content-based song recommender system that suggests similar songs based on their features.

## What It Does
- Takes a song name as input
- Finds its features in the dataset
- Calculates similarity with other songs
- Returns the most similar songs

## Components Used
- Python
- Pandas (data loading and cleaning)
- NumPy (numeric operations)
- Scikit-Learn (cosine similarity)
- Streamlit (simple user interface)
- CSV dataset containing song information

## How It Works
1. Load dataset
2. Select and preprocess song features
3. Create feature vectors for all songs
4. Compute cosine similarity
5. Recommend top similar songs

## How to Run
```bash
pip install -r requirements.txt
streamlit run app.py
