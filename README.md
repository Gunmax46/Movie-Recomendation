🎬 Movie Recommendation System

A Hybrid Movie Recommendation System built using Flask that provides personalized movie suggestions by combining content-based filtering and external API recommendations.

🚀 Features
🔍 Search movies using TMDB API
🎯 Hybrid recommendation engine (Content + TMDB API)
⭐ User rating system
🎭 Browse movies by genre
📊 Top-rated movie listings
📺 Streaming platform availability
💻 Responsive UI with modern design
🧠 Recommendation System

This project uses a Hybrid Recommendation Approach:

1. Content-Based Filtering
Uses TF-IDF Vectorization on:
Movie title
Overview
Genres
Computes similarity using cosine similarity
2. Additional Features
Genre-based encoding
Popularity, rating, and vote count normalization
3. Hybrid Strategy
Local recommendations from dataset
Fallback to TMDB API recommendations when needed

Implemented in:
HybridRecommender class

🏗️ Tech Stack
Backend: Flask
Database: SQLite
Machine Learning: Scikit-learn
Frontend: HTML, CSS, JavaScript
API: TMDB (The Movie Database)
Libraries:
pandas
numpy
scikit-learn
requests
surprise
movie-recommender/
│
├── app.py                 # Main Flask application
├── database.py           # Database handling (SQLite)
├── recommendation.py     # Hybrid recommender system
│
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── search.html
│   ├── genre.html
│   └── recommendations.html
│
├── static/
│   ├── css/style.css
│   └── js/main.js
│
├── movies.db             # SQLite database
├── requirements.txt
└── README.md
⚙️ Installation & Setup
1. Clone the Repository
git clone https://github.com/your-username/movie-recommender.git
cd movie-recommender
2. Create Virtual Environment
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
3. Install Dependencies
pip install -r requirements.txt
4. Setup Environment Variables

Create a .env file:

TMDB_API_KEY=your_tmdb_api_key

(Used in Flask app for API calls )

5. Run the Application
python app.py

App will run on:

http://127.0.0.1:5000/
🗄️ Database

SQLite database includes:

Movies Table
id
title
overview
genres
rating
popularity
vote_count
User Ratings Table
user_id
movie_id
rating

Defined in:

🌐 API Integration
Uses TMDB API for:
Movie search
Top-rated movies
Genre-based movies
Streaming providers
External recommendations
📸 UI Highlights
Clean Netflix-style UI
Dynamic movie cards
Genre browsing
Search functionality
Rating system via AJAX
📌 Future Improvements
🔐 User authentication system
🤖 Collaborative filtering (user-based)
📈 Better ranking using deep learning
🎥 Trailer integration
📱 Mobile app version
🤝 Contributing

Contributions are welcome!
Feel free to fork the repo and submit a pull request.

📄 License

This project is licensed under the MIT License.

👨‍💻 Author

Ganesh Nemmaluri
