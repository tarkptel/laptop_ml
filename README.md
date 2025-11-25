<h1 align="center">💻 Laptop Price Predictor</h1>
<p align="center">
  A Machine Learning project that predicts laptop prices based on specifications such as brand, RAM, CPU, storage, OS, and more.
</p>
<br>

<h2>📌 Project Overview</h2>
<p>
This repository contains a complete end-to-end ML project that predicts laptop prices.  
It includes:
</p>

<ul>
  <li>Data cleaning & preprocessing</li>
  <li>Feature engineering</li>
  <li>Model training & evaluation</li>
  <li>Saving ML pipeline (<code>pipe.pkl</code>)</li>
  <li>Interactive prediction app (<code>app.py</code>)</li>
  <li>Deployment files (Dockerfile, Procfile)</li>
</ul>

<br>

<h2>📁 Repository Structure</h2>

<pre>
├── laptop-price-predictor.ipynb   → Full ML workflow (EDA, preprocessing, model training)
├── laptop_data.csv                → Dataset used for training
├── pipe.pkl                       → Trained ML pipeline (model + preprocessing)
├── df.pkl                         → Processed dataset used in the app
├── app.py                         → Web application for predictions (Streamlit/Flask UI)
├── requirements.txt               → Required dependencies
├── Dockerfile                     → For containerizing the app
├── Procfile                       → For deployment platforms like Heroku
└── setup.sh                       → Helper script for deployment
</pre>

<br>

<h2>🚀 How to Run the App Locally</h2>

<h3>1️⃣ Clone the Repository</h3>
<pre><code>git clone https://github.com/tarkptel/laptop_ml.git
cd laptop_ml
</code></pre>

<h3>2️⃣ Install Dependencies</h3>
<pre><code>pip install -r requirements.txt
</code></pre>

<h3>3️⃣ Run the Web App</h3>

If the project uses <strong>Streamlit</strong>:
<pre><code>streamlit run app.py
</code></pre>

If the project uses <strong>Flask</strong>:
<pre><code>python app.py
</code></pre>

<p>The app will open in your browser and allow you to select laptop specifications to get the predicted price.</p>

<br>

<h2>🧠 Model Details</h2>
<ul>
  <li>Machine Learning model trained using Scikit-learn</li>
  <li>Preprocessing + model combined into one pipeline (<code>pipe.pkl</code>)</li>
  <li>Supports categorical + numerical features</li>
  <li>Notebook explains full training steps</li>
</ul>

<br>

<h2>📊 Dataset</h2>
<p>
The dataset (<code>laptop_data.csv</code>) contains laptop attributes like brand, processor, RAM, storage, display type, OS, weight, etc.  
The notebook performs:
</p>
<ul>
  <li>Missing value handling</li>
  <li>Categorical encoding</li>
  <li>Feature extraction from text fields</li>
  <li>Model evaluation & selection</li>
</ul>

<br>

<h2>🐳 Run with Docker</h2>

<h3>Build Docker Image</h3>
<pre><code>docker build -t laptop-price-predictor .
</code></pre>

<h3>Run the Container</h3>
<pre><code>docker run -p 5000:5000 laptop-price-predictor
</code></pre>

<p>(If Streamlit is used, the port might be <code>8501</code>)</p>

<br>

<h2>☁️ Deploying (Heroku / Render / HF Spaces)</h2>

<p>This repo includes a <code>Procfile</code> for easy deployment.</p>

<p>The app will automatically start using Gunicorn/Streamlit based on your <code>Procfile</code>.</p>

<br>

<h2>✨ Features</h2>
<ul>
  <li>Clean and simple UI for selecting laptop specs</li>
  <li>Real-time price prediction</li>
  <li>Fully reproducible ML pipeline</li>
  <li>Ready for deployment using Docker</li>
</ul>

<br>

<h2>📞 Contact</h2>
<p>
<strong>Author:</strong> Tark Patel  
<br>
For issues or improvements, feel free to open a GitHub Issue.
</p>

<hr>

<p align="center">⭐ If you like this project, don't forget to star the repository!</p>
