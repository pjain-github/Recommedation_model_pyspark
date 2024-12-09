# Recommeedation Model using Pyspark

## Overview

This notebook explores the recipie data and builds a collaborative filtering model to predict recipe ratings. It involves data cleaning, exploratory data analysis (EDA), feature selection, model training, and evaluation.

## Steps Involved

1. **Setup:** Mount Google Drive, install necessary libraries (Pyspark, Lenskit), and create a Spark session.
2. **Data Loading:** Read raw ratings and recipes data from CSV files into Spark DataFrames.
3. **Data Cleaning:** Handle missing values and convert data types for relevant columns (e.g., nutrition, tags, submitted date).
4. **EDA:** Analyze data distributions, relationships, and patterns, including nutrition values and tag frequencies.
5. **Feature Selection:** Remove irrelevant features (e.g., text-based columns) for modeling.
6. **Train-Test Split:** Divide the dataset into training and testing sets based on a cutoff date.
7. **Collaborative Filtering Model:** Build an Alternating Least Squares (ALS) model using Pyspark's ML library.
8. **Model Training:** Train the ALS model on the training data.
9. **Model Prediction:** Generate predictions on the test data using the trained model.
10. **Model Evaluation:** Evaluate the model's performance using RMSE and rank-based metrics (reciprocal rank, NDCG, DCG).

## Technology Used

- **Google Colab:** Cloud-based notebook environment for running the code.
- **Pyspark:** Python library for distributed data processing using Apache Spark.
- **Lenskit:** Python library for recommender systems research and development.
- **Pandas:** Python library for data manipulation and analysis.
- **NumPy:** Python library for numerical computing.

## Final Performance

- **RMSE:** [Insert RMSE value obtained from the model evaluation].
- **Rank-based Metrics:** 
    - Reciprocal Rank: [Insert average reciprocal rank].
    - NDCG: [Insert average NDCG].
    - DCG: [Insert average DCG].

## Observations

- The collaborative filtering model provides reasonable predictions for recipe ratings.
- Only one record had NDCG and DCG values greater than 0, suggesting potential areas for improvement.

## Future Work

- Explore different model parameters and algorithms to improve prediction accuracy.
- Incorporate content-based features (e.g., ingredients, tags) for a hybrid recommender system.
- Implement a user interface for recipe recommendations.
