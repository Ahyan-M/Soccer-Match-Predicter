# Soccer Match Predictor

This project is a machine learning model that predicts the outcome of English Premier League matches based on historical match data. The model predicts whether a team will win a match with an accuracy of **67.5%**.

## Features

- Utilizes match metadata such as:
  - Venue
  - Opponent team
  - Match time
  - Day of the week
- Encodes categorical features for machine learning compatibility
- Trains a logistic regression classifier to predict match results
- Measures model accuracy on validation data

## How It Works

1. **Data Preparation**: The dataset (`matches.csv`) is cleaned and encoded.
2. **Feature Engineering**:
   - `venue_code`, `opp_code`, `hour`, and `day_code` are generated.
   - Target is binary: 1 for win, 0 otherwise.
3. **Model Training**: A logistic regression model is trained using scikit-learn.
4. **Evaluation**: The model achieves a prediction accuracy of ~67.5%.

## Requirements

- Python 3.x
- pandas
- scikit-learn
- Jupyter Notebook (optional)

Install the dependencies with:

```bash
pip install pandas scikit-learn
