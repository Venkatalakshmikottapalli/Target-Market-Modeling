# Targeted Marketing Model for SMARTMARKET

## Project Overview
This project develops a targeted marketing model for SMARTMARKET to optimize campaign response rates. The objective is to identify the top 25% of subscribers most likely to respond to marketing campaigns from week 27 onwards, using historical data and behavioral patterns.

## Dataset
The dataset is stored in the `data/` folder and contains the following columns:

- `week_number`: The week the campaign was launched.
- `subscriber_id`: A unique identifier for each subscriber.
- `user_category`: Category of the subscriber (A, B, C, or D).
- `state_id`: The location of the subscriber.
- `gender`: Gender of the subscriber.
- `campaign_id`: ID of the marketing campaign.
- `response`: Whether the subscriber responded to the campaign (1 for response, 0 for no response).

Additional features generated through feature engineering include:
- `FRQ_W_2`, `FRQ_W_3`, `FRQ_W_4`, `FRQ_W_5`: Response frequency in the past 2-5 weeks.
- `LIFE_TIME_RESPONSE_RATE`: Overall response rate of the subscriber across all campaigns.
- `LAST_CAMPAIGN`, `LAST_2ND_CAMPAIGN`: IDs of the last two campaigns received.
- `IS_LAST_A_RESPONSE`: Indicates if the subscriber responded to the last campaign.
- `WEEK_SINCE_LAST_RESPONSE`: Number of weeks since the last response.

## Project Structure
- `data/`: Contains the dataset in CSV format (`dataset.csv`).
- `notebook/`: Contains the Jupyter notebook (`targeted_marketing_model.ipynb`) used for data preprocessing, model training, and evaluation.

## Key Steps

1. **Data Preprocessing**: 
   - Load the dataset and clean any missing values.
   - Feature engineering to create new columns based on historical behavior patterns.
   
2. **Exploratory Data Analysis (EDA)**:
   - Analyze patterns and trends related to gender, state, user category, and past responses to derive insights.

3. **Modeling**:
   - Build a machine learning model to predict the likelihood of a subscriber responding to a marketing campaign.
   - Features are selected based on the relevance to response prediction, such as historical responses and recent campaign interaction.

4. **Model Evaluation**:
   - Evaluate the model using metrics such as precision, recall, and AUC-ROC to gauge the effectiveness of predictions.
   
5. **Prediction**:
   - Predict the top 25% of subscribers most likely to respond for future campaign targeting.


