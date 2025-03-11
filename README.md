# Movie Recommender System

## Project Overview
This project is a **Movie Recommender System** that suggests movies based on a selected movie. It utilizes **content-based filtering** to find similar movies and displays their posters. The project is built using **Streamlit** for the interactive user interface, **pickle** for loading precomputed data, and **TMDB API** to fetch movie posters.

## Goals and Importance
### Goals:
- Develop a **user-friendly** movie recommendation system.
- Provide **personalized** movie suggestions based on user input.
- Display **movie posters** for visual engagement.
- Utilize **content-based similarity** for recommendations.

### Importance:
- Enhances **user experience** by offering intuitive movie suggestions.
- Demonstrates **practical application** of machine learning in entertainment.
- Showcases **efficient use of APIs** to enrich recommendations with visuals.

## Dataset
The dataset used for this project is sourced from **[Kaggle: TMDB Movie Metadata](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)**, which contains details about thousands of movies, including their genres, titles, and unique IDs.

## Technologies Used
- **Python**: Core programming language.
- **Streamlit**: Web framework for interactive UI.
- **Pandas**: Data manipulation and processing.
- **Pickle**: Serialization and deserialization of precomputed models.
- **TMDB API**: Fetching movie posters dynamically.
- **Scikit-learn**: Computing similarity scores.

## Project Structure
```
|-- model/
|   |-- movie_list.pkl  # Pickle file containing movie data
|   |-- similarity.pkl  # Pickle file with similarity scores
|
|-- app.py  # Streamlit app for recommendations
|-- README.md  # Project documentation
```

## How It Works
1. **Load Data**: Precomputed movie list and similarity matrix are loaded from `pickle` files.
2. **User Input**: The user selects a movie from the dropdown.
3. **Compute Recommendations**: The system finds the top 5 most similar movies.
4. **Fetch Posters**: The TMDB API retrieves posters for the recommended movies.
5. **Display Recommendations**: Movie names and posters are shown in the app.

## Installation and Setup
### Prerequisites
Ensure you have Python installed along with the required libraries.

### Steps to Run the Application:
1. Clone the repository:
   ```bash
   git clone <repo_url>
   cd movie-recommender
   ```
2. Install dependencies:
   ```bash
   pip install streamlit pandas requests pickle5
   ```
3. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```
4. Select a movie from the dropdown and get recommendations!

## Future Enhancements
- Add **collaborative filtering** for better recommendations.
- Include **user ratings and reviews** for improved results.
- Implement **real-time movie search** using APIs.

## Credits
- **Dataset**: TMDB Movie Metadata from Kaggle.
- **Poster API**: TMDB API.
- **Libraries**: Streamlit, Pandas, Pickle, Requests.

## License
This project is for educational purposes and follows an open-source approach.

