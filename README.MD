## Movie Recommender System

### Overview
This project implements a Movie Recommender System using Neural Collaborative Filtering (NCF). The system predicts movie ratings for users and provides movie recommendations based on these predictions.

### Files
- movie_2.ipynb: Jupyter notebook containing the implementation of the Movie Recommender System.

### Requirements
- Python 3.11.5
- Jupyter Notebook
- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn
- tensorflow
- keras
- keras-tuner

### Installation
1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd movie-recommender-system
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

### Usage
1. Open the Jupyter notebook:
    ```sh
    jupyter notebook movie_2.ipynb
    ```

2. Run the cells in the notebook to:
    - Load and preprocess the dataset.
    - Visualize the data.
    - Train the Neural Collaborative Filtering model.
    - Evaluate the model.
    - Make predictions and provide movie recommendations.

### Key Sections
- **Data Loading and Preprocessing**: Load the movie ratings and movie details datasets, preprocess the data, and split it into training and testing sets.
- **Data Visualization**: Visualize the distribution of ratings, number of ratings per user, and number of ratings per movie.
- **Model Training**: Define and train the Neural Collaborative Filtering model using Keras and TensorFlow.
- **Hyperparameter Tuning**: Use Keras Tuner to find the best hyperparameters for the model.
- **Model Evaluation**: Evaluate the model's performance on the test dataset.
- **Recommendations**: Make movie recommendations for a given user based on the trained model.

### Example
To get movie recommendations for a specific user, run the following code in the notebook:
```python
user_id = 105623  # Replace with an actual userId from your dataset
top_recommendations = recommend_movies(user_id)
print(top_recommendations.to_markdown())
```

---

## Climate Change Classification Model

### Overview
This project analyzes global temperature data and builds a classification model to understand climate change trends. The analysis includes data visualization, data preprocessing, and model training.

### Files
- climate-modelling.ipynb: Jupyter notebook containing the implementation of the Climate Change Classification Model.

### Requirements
- Python 3.11.5
- Jupyter Notebook
- numpy
- pandas
- matplotlib
- seaborn
- plotly
- scikit-learn

### Installation
1. Clone the repository:
    ```sh
    git clone <repository-url>
    cd climate-change-modelling
    ```

2. Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```

### Usage
1. Open the Jupyter notebook:
    ```sh
    jupyter notebook climate-modelling.ipynb
    ```

2. Run the cells in the notebook to:
    - Load and preprocess the global temperature dataset.
    - Visualize temperature trends and geographical distribution.
    - Train and evaluate Linear Regression and Polynomial Regression models.
    - Make predictions for future global temperatures.

### Key Sections
- **Data Loading and Preprocessing**: Load the global temperature dataset, clean the data, and handle missing values.
- **Data Visualization**: Visualize temperature trends using various plots, including dynamic maps and bar charts.
- **Model Training**: Train Linear Regression and Polynomial Regression models to predict global temperatures.
- **Model Evaluation**: Evaluate the models' performance and visualize the residuals.
- **Predictions**: Use the trained models to predict future global temperatures.

### Example
To predict the global land temperature for a specific year, run the following code in the notebook:
```python
X_predict = [2084]
X_predict_poly = poly_features.transform(np.array(X_predict).reshape(1, -1))
y_predict = poly_regressor.predict(X_predict_poly)
print(f"Predicted Land Global Temperature in {X_predict[0]}: {y_predict[0][0]:.2f} °C")
```

---