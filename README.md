# Movie Recommendation System

## Project Overview

This project is a movie recommendation system that utilizes both a Hybrid Recommender Model and a Matrix Factorization Model. The Hybrid Recommender combines user, movie, genre, and sentiment features to make predictions, while the Matrix Factorization Model relies on user-item interactions. The goal of this project is to compare the performance of these two models and determine which one provides better recommendations based on accuracy and classification metrics.

## Dataset

The project uses a dataset that includes the following information:
- **user_id**: Unique identifier for each user.
- **movie_id**: Unique identifier for each movie.
- **movie_title**: The title of the movie.
- **genre**: The genre of the movie.
- **average_sentiment_score**: Sentiment score derived from user reviews.
- **rating**: User rating for the movie.

### Data Sources
- The primary data file is `merged_data_1.csv`, which contains detailed movie information, including genres and user ratings.
- After training the Hybrid Recommender Model, a new dataset `hybrid_model_predictions.csv` was generated, which includes predicted ratings alongside actual user ratings.

## Models

### 1. Hybrid Recommender Model
This model incorporates multiple features:
- **User Embedding**: Captures latent factors representing user preferences.
- **Movie Embedding**: Captures latent factors representing movie characteristics.
- **Genre Embedding**: Encodes genre information.
- **Sentiment Embedding**: Uses sentiment analysis scores derived from user reviews.

### 2. Matrix Factorization Model
This model focuses on user-item interactions, learning latent features for both users and items to predict ratings.

## Evaluation Metrics

The models are evaluated using the following metrics:
- **Root Mean Squared Error (RMSE)**
- **Mean Absolute Error (MAE)**
- **R2**
- **Accuracy**
- 

## How to Run the Project

### Prerequisites
- Python 3.7 or higher
- Required libraries: `pandas`, `numpy`, `torch`, `sklearn`, `plotly`

### Steps to Run
   1 .  **Prepare the Dataset**:
   - Place the `merged_data_1.csv` file in the designated directory.
   
   2 . **Train the Models**:
   - Run the training script to train both the Hybrid Recommender Model and the Matrix Factorization Model.
   - The script will generate `hybrid_model_predictions.csv`.

   3 . **Evaluate the Models**:
   - Run the evaluation script to compare the models based on RMSE, MAE, Precision, Recall, and F1-Score.
   - The script will generate visualizations of the results.

   4 . **Generate Recommendations**:
   - Use the recommendation script to generate movie recommendations for a specific user.


## Files and Directories

- `merged_data_1.csv`: Original dataset with movie information.
- `hybrid_model_predictions.csv`: Contains predicted and actual ratings generated by the Hybrid Recommender Model.
- `README.md`: Project documentation.
- `training_script.py`: Script for training the models.
- `evaluation_script.py`: Script for evaluating model performance.

## Visualizations

**Matrix Factorization:-**

RMSE over Epochs

![App Screenshot](https://github.com/Salman-Khan-Mohammed/Recommendation-System/blob/main/Matrix-f_RMSE_AHP.png)


**Hybrid Model:-**

RMSE over Epochs

![App Screenshot](https://github.com/Salman-Khan-Mohammed/Recommendation-System/blob/main/Hybrid-M_AHP.png)


**Comparing the performance of both models using bar charts :-** These visualizations provide a clear comparison across different evaluation metrics.
![App Screenshot](https://github.com/Salman-Khan-Mohammed/Recommendation-System/blob/main/Models_Comparison.png)

## Observations

The Matrix Factorization Model outperforms the Hybrid Recommender Model in terms of both accuracy and classification metrics:
- The Hybrid model has a higher RMSE (0.937605) and MAE (0.741122) compared to the Matrix Factorization model, indicating that its predictions are less accurate.

- In contrast, the Matrix Factorization model significantly outperforms the Hybrid model in every evaluation metric. It has a much lower RMSE (0.299825) and MAE (0.222490), indicating better prediction accuracy.
  

## Conclusion

This project demonstrates the power of different recommendation models. The Matrix Factorization Model outperformed the Hybrid Model in this context, but further improvements and tuning might help the Hybrid Model achieve better results in future iterations.

## License

This project is licensed under the MIT License.

## Acknowledgments

- Thanks to the open-source community for providing the libraries used in this project.
- Special thanks to [Your Name/Your Team] for contributions and support in developing this project.


## License

[MIT](https://choosealicense.com/licenses/mit/)


## Support


For any questions or feedback, please contact:

Name: Mohammed Salman Khan

Email: mohammedsalman65257@gmail.com 

LinkedIn: https://www.linkedin.com/in/mohammed-salman-khan-529177193/
