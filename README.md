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
## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the project directory:
   ```bash
   cd Yelp_Boost
   ```
3. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```
## Usage

1. Place the required JSON files (`user.json`, `business.json`, etc.) and the training CSV file (`yelp_train.csv`) in the specified folder.
2. Run the main script:
   ```bash
   python main.py <folder_path> <val_file> <output_file>
   ```
   Replace `<folder_path>`, `<val_file>`, and `<output_file>` with the appropriate paths.
3. The script generates predictions in the specified `<output_file>` and prints the RMSE and error distribution.
## Hyperparameter Tuning

- Hyperparameter tuning for XGBoost and CatBoost is implemented using Optuna.
- The tuning code is commented out due to time constraints and unavailability of Optuna in certain environments. 
