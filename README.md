# MovieSage 🎬

A sophisticated movie recommendation system that suggests films based on user ratings and collaborative filtering techniques. Get personalized movie suggestions based on viewing patterns and user preferences! 🎯

## 🌟 Features

- Collaborative filtering-based recommendation engine
- Movie similarity analysis using correlation matrices
- Support for large-scale movie rating datasets
- Interactive movie search and recommendation retrieval
- Visualization of rating distributions and patterns
- Top 4 movie recommendations for each film

## 🛠️ Technologies Used

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- IPython Widgets

## 📊 Dataset Requirements

The system expects two main data files:
1. `dataset.csv` - Tab-separated file with columns:
   - user_id
   - item_id
   - rating
   - timestamp

2. `movieIdTitles.csv` - Movie metadata file with columns:
   - item_id
   - title

## 🚀 Getting Started

1. Clone the repository:
```bash
git clone https://github.com/yourusername/movie-sage.git
cd movie-sage
```

2. Install required dependencies:
```bash
pip install pandas numpy matplotlib seaborn ipywidgets
```

3. Place your dataset files in the project directory:
   - `dataset.csv`
   - `movieIdTitles.csv`

4. Run the Jupyter notebook or Python script:
```bash
jupyter notebook "Movie Recommender System.ipynb"
```

## 💡 How It Works

1. The system loads and processes movie ratings data
2. Creates a user-movie rating matrix
3. Calculates correlation between movies based on user ratings
4. Generates top 4 recommendations for each movie
5. Saves recommendations for quick retrieval
6. Provides an interactive interface for movie lookup

## 📈 Example Usage

```python
# Get recommendations for a specific movie
inputMovieName.value = "Star Wars (1977)"
getRecommendations(None)
```

## 🎯 Results

The system provides four recommended movies based on user rating patterns and movie similarities. Recommendations are generated only for movies with sufficient rating data (>100 ratings) to ensure quality suggestions.

## 📝 Notes

- The system uses collaborative filtering, focusing on movie-movie similarities
- Only movies with more than 100 ratings are considered for recommendations
- The correlation matrix approach ensures recommendations are based on genuine user preferences
- Results are cached for faster subsequent lookups

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

