# Movie Recommendation System

This project implements a **Content-Based Movie Recommendation System** using Machine Learning. The system leverages the **cosine similarity** technique to compute the similarity between movies and provides personalized recommendations based on user preferences.

```

## Features

- **Content-Based Filtering**: Recommends movies similar to a given movie based on their content.
- **Cosine Similarity**: Measures the distance between movie vectors to identify similarities.
- **Efficient Recommendation**: Provides accurate recommendations using a scalable approach.
- **Dataset**: Data sourced from Kaggle for building and training the model.

## Dataset

The dataset for this project is downloaded from [Kaggle](https://www.kaggle.com). It contains metadata about movies, including features such as:

- Movie Title
- Genre
- Description
- Keywords
- Cast
- Crew

## How It Works

1. **Data Preprocessing**:
   - Load and clean the dataset.
   - Extract meaningful features such as genres, keywords, and descriptions.
   - Create a combined feature set for each movie.

2. **Vectorization**:
   - Use a text vectorization technique (e.g., TF-IDF or Count Vectorizer) to convert movie features into numerical vectors.

3. **Cosine Similarity**:
   - Calculate cosine similarity scores between all movie vectors to determine their similarity.

4. **Recommendation**:
   - For a given movie, find its closest matches based on cosine similarity scores.
   - Return the top N recommended movies.

## Project Structure

```
movie-recommendation-system
├── dataset/
│   └── movies.csv                            # Kaggle dataset
│   └── credits.csv                           # Kaggle dataset
│   ├── movie-recomendation-system.py         # Python API for recommendations
├── README.md                                 # Project documentation
└── tests/
    └── test_recommend.py                     # Unit tests for the recommendation system
```

## Technologies Used

- **Python**:
  - pandas, NumPy (Data manipulation)
  - scikit-learn (Cosine similarity computation)
- **Flask**:
  - REST API to expose the recommendation engine.
- **Dataset Source**:
  - Kaggle (Movie metadata).

## How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/movie-recommendation-system.git
cd movie-recommendation-system
```

### 2. Install Dependencies
```bash
pip install -r app/requirements.txt
```

The API will be available at `http://127.0.0.1:5000`.

### 3. Test 
```json
{
    "movie_name": "Inception"
}
```

## Future Enhancements

- Add support for collaborative filtering.
- Integrate with a front-end application (React.js).
- Deploy the system on cloud platforms like AWS or Heroku.
- Enhance the dataset with additional features like ratings and reviews.

## Contributing

Contributions are welcome! Please fork the repository and create a pull request for any feature enhancements or bug fixes.


## Acknowledgements

- [Kaggle](https://www.kaggle.com) for providing the movie dataset.
- The Python and Machine Learning communities for their amazing tools and support.

---
