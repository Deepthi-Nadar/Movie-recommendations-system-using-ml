# Movie Recommendation System

This project implements a simple movie recommendation system based on content-based filtering. The system recommends movies similar to a given movie based on their genres, keywords, tagline, cast, and director.

## Introduction

Movie recommendation systems are essential tools for helping users discover new content in the vast landscape of available movies. This particular system leverages textual metadata associated with movies to find similarities and suggest films that align with user preferences. By analyzing features like genres, keywords, cast, and director, it provides personalized recommendations.

## Features

-   **Content-Based Filtering**: Recommends movies based on the similarity of their attributes (genres, keywords, tagline, cast, director).
-   **TF-IDF Vectorization**: Uses TF-IDF to convert text data into numerical feature vectors.
-   **Cosine Similarity**: Employs cosine similarity to measure the similarity between movie feature vectors.
-   **Interactive Input**: Allows users to enter a movie name to get recommendations.
-   **Top 10 Recommendations**: Provides a list of the top 10 most similar movies.

## How to Use

To use this movie recommendation system, follow these steps:

1.  **Clone the Repository (or download the notebook)**:

    ```bash
    git clone <repository-url>
    cd movie-recommendation-system
    ```

2.  **Ensure you have the dataset**: Make sure the `movies.csv` file is present in the same directory as the notebook or update the path in the code if it's located elsewhere.

3.  **Run the Jupyter Notebook / Colab Notebook**: Open the notebook in Google Colab or a Jupyter environment.

    The notebook will guide you through the following steps:
    -   Loading necessary libraries (`pandas`, `numpy`, `difflib`, `sklearn`).
    -   Loading and preprocessing the dataset.
    -   Selecting relevant features and handling missing values.
    -   Combining selected features into a single string for each movie.
    -   Converting text data to numerical feature vectors using `TfidfVectorizer`.
    -   Calculating cosine similarity between all movie pairs.
    -   Prompting the user to enter a favorite movie name.
    -   Finding the closest match for the entered movie name in the dataset.
    -   Retrieving and sorting similar movies based on similarity scores.
    -   Printing the top 10 recommended movies.

4.  **Enter your favorite movie name** when prompted by the system in the last code cell.

## Requirements

To run this notebook, you need the following Python libraries:

-   `pandas`
-   `numpy`
-   `scikit-learn`
-   `difflib`

You can install them using pip:

```bash
pip install pandas numpy scikit-learn difflib
```

