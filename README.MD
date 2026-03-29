## MOVIE RECOMMENDATION SYSTEM ##
Movie Recommender System
A content-based movie recommendation system that suggests similar movies based on their metadata, such as genres, keywords, cast, and crew. This project includes a machine learning backend and a web-based frontend built with Streamlit for an interactive user experience.

# Features
Search & Recommend: Select a movie from the database to get a list of top similar movie recommendations.

Content-Based Filtering: Uses movie overviews, genres, keywords, and cast/crew information to find matches.

Interactive UI: A clean and simple web interface powered by Streamlit.

# Data & Processing
The system uses the TMDB 5000 Movies Dataset. The following steps were performed to build the model:

Data Cleaning: Merged movie details with credits and handled missing values.

Feature Engineering: Extracted significant tags from JSON-formatted columns like genres, keywords, cast, and crew.

Text Preprocessing: Applied lemmatization and removed stop words to create a unified "tags" column for each movie.

Vectorization: Converted text tags into numerical vectors using techniques like CountVectorizer.

Similarity Measurement: Calculated Cosine Similarity between movie vectors to determine how closely related movies are to each other.

# Technologies Used
Python: Primary programming language.

Pandas & NumPy: For data manipulation and analysis.

Scikit-Learn: For text vectorization and computing similarity.

Streamlit: For building the web application.

Pickle: To save and load the trained model and movie data.