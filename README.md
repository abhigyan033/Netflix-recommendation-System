# Netflix Recommendation System using SVD

This project implements a **Recommendation System** using **Singular Value Decomposition (SVD)** to predict user ratings for movies, based on a dataset of Netflix user ratings. The SVD-based approach helps to provide personalized recommendations to users based on their historical preferences.

## Table of Contents
- [Project Overview](#project-overview)
- [Data](#data)
- [Methodology](#methodology)
- [Libraries Used](#libraries-used)
- [Usage](#usage)
- [Results](#results)
- [Future Improvements](#future-improvements)
- [References](#references)

## Project Overview
The primary goal of this project is to build a movie recommendation system that leverages user-movie ratings data. Using **SVD**, we can identify latent factors in the data that explain user preferences, allowing the system to recommend movies that users are likely to enjoy.

## Data
We use the Netflix Prize dataset, which contains over 100 million ratings from users for various movies. The dataset includes:
- `Cust_Id`: Customer ID (Anonymous)
- `Rating`: Movie ratings given by the customer (1-5)

The data is preprocessed to handle missing values, and the matrix is factorized using SVD to reduce dimensionality.

## Methodology
The following steps were taken in building the recommendation system:
1. **Data Loading and Exploration**: The dataset is loaded into a Pandas DataFrame, and basic exploratory analysis is performed.
2. **Data Preprocessing**: The dataset is cleaned by handling missing values and converting the data into a matrix form.
3. **Singular Value Decomposition (SVD)**: SVD is applied to decompose the user-movie matrix into three components:
   - **U**: User matrix
   - **Σ**: Diagonal matrix of singular values
   - **V**: Movie matrix
4. **Prediction and Evaluation**: Predicted ratings are calculated using the decomposed matrices, and the system's performance is evaluated using metrics such as RMSE.

## Libraries Used
The following Python libraries are required to run the project:
- `numpy`
- `pandas`
- `matplotlib`
- `scikit-learn`
- `scipy`
