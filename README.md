# Yelp Boost Recommendation System

Yelp Boost is a weighted hybrid recommendation system designed to predict user ratings for businesses. By leveraging advanced feature engineering and machine learning models, this project aims to achieve a low RMSE (Root Mean Square Error) for accurate predictions.

## Features

- **Hybrid Recommendation System**: Combines predictions from XGBoost and CatBoost models using a weighted formula.
- **Feature Engineering**: Extracts and aggregates meaningful features from multiple datasets.
- **Robust Handling of Missing Data**: Assigns default values to ensure robustness.
- **Error Analysis**: Provides RMSE and error distribution insights.
## Data Sources

- `user.json`: Contains user attributes such as average stars and review count.
- `business.json`: Includes business attributes like latitude, longitude, stars, and binary attributes (e.g., `GoodForKids`, `HasTV`).
- `review_train.json`: Aggregates `useful`, `funny`, and `cool` counts for each business.
- `checkin.json`: Aggregates check-in counts for each business.
