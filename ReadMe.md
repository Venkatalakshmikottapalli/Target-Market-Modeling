# Targeted Marketing Model for SMARTMARKET

## Table of Contents
- [Introduction](#introduction)
- [Data Acquisition](#data-acquisition)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This project aims to build a targeted marketing model for SMARTMARKET to optimize campaign response rates. The model identifies and targets only 25% of the subscriber base starting from week 27, leveraging data-driven insights to enhance marketing effectiveness.

## Data Acquisition
The dataset used for this project includes subscriber information and campaign responses, consisting of various features such as:
- `week_number`
- `subscriber_id`
- `user_category`
- `state_id`
- `gender`
- `campaign_id`
- `response`
- Additional derived features

## Exploratory Data Analysis
Exploratory data analysis (EDA) is performed to understand the dataset's structure, identify trends, and uncover patterns. Key analyses include:
- Distribution of user categories and responses
- Gender and state analysis
- Campaign effectiveness and response rates

## Feature Engineering
Feature engineering is conducted to extract meaningful variables from the existing dataset. New features include:
- Frequency metrics (`FRQ_W_2`, `FRQ_W_3`, `FRQ_W_4`, `FRQ_W_5`)
- Lifetime response rate
- Recency metrics (`LAST_CAMPAIGN`, `LAST_2ND_CAMPAIGN`, `IS_LAST_A_RESPONSE`, `WEEK_SINCE_LAST_RESPONSE`)

## Modeling
Various machine learning algorithms are implemented to build the targeting model. Key steps include:
1. Data preprocessing (handling missing values, encoding categorical variables)
2. Model selection (e.g., logistic regression, decision trees, random forests)
3. Hyperparameter tuning to optimize model performance

## Evaluation
Model performance is evaluated using appropriate metrics, such as:
- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC Curve

The results help determine the most effective targeting strategy.

## Usage
To use this project:
1. Clone the repository.
2. Install the necessary libraries as specified in the `requirements.txt` file.
3. Update any file paths in the code as needed.
4. Run the main script to train the model and evaluate its performance.

## Contributing
Contributions are welcome! If you have suggestions for improvements or find issues, please open an issue or submit a pull request.

## License
This project is licensed under the MIT License.



