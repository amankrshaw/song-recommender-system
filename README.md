<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Song Recommender System - Overview</title>
  <style>
    body { font-family: Arial, sans-serif; line-height: 1.6; margin: 32px; color: #111; }
    header { margin-bottom: 20px; }
    h1 { font-size: 24px; margin: 0 0 8px 0; }
    h2 { font-size: 18px; margin: 18px 0 8px 0; }
    p { margin: 6px 0 12px 0; }
    ul { margin: 6px 0 12px 24px; }
    code { background:#f4f4f4; padding:4px 6px; border-radius:4px; font-family: monospace; }
    .box { max-width: 800px; }
  </style>
</head>
<body>
  <div class="box">
    <header>
      <h1>Song Recommender System</h1>
      <p>Simple content-based recommendation system that suggests songs similar to a given input using song features.</p>
    </header>

    <section>
      <h2>What it does</h2>
      <p>Given a song name, the system finds its features in the dataset, computes similarity with other songs, and returns the most similar items.</p>
    </section>

    <section>
      <h2>Main components</h2>
      <ul>
        <li>Python</li>
        <li>Pandas for data loading and cleaning</li>
        <li>NumPy for numeric operations</li>
        <li>Scikit-learn for similarity computation (cosine similarity)</li>
        <li>Streamlit for a simple web UI</li>
        <li>CSV dataset containing song features (for example: name, artist, genre, popularity, acousticness, danceability)</li>
      </ul>
    </section>

    <section>
      <h2>How it works</h2>
      <ol>
        <li>Load the dataset.</li>
        <li>Choose and preprocess useful features (numericize categorical features, normalize audio feature columns).</li>
        <li>Combine features into a feature vector for each song.</li>
        <li>Compute cosine similarity between vectors.</li>
        <li>For a query song, pick the top N most similar songs and show them in the UI.</li>
      </ol>
    </section>

    <section>
      <h2>How to run</h2>
      <p>Install required packages and start the Streamlit app:</p>
      <pre><code>pip install -r requirements.txt
streamlit run app.py</code></pre>
    </section>

    <section>
      <h2>Key notes</h2>
      <ul>
        <li>This is a content-based approach (no user history required).</li>
        <li>Dataset quality and chosen features strongly affect recommendation quality.</li>
        <li>Future improvements: add collaborative filtering, user profiles, or hybrid methods.</li>
      </ul>
    </section>
  </div>
</body>
</html>
