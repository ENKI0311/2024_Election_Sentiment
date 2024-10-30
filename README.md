# 2024_Election_Sentiment
An analysis of polling data to predict election sentiment, uncover key influences, and interpret Independent support impact on electoral dynamics.

---

# Election Sentiment Analysis with Predictive Modeling

This project analyzes polling data to predict public sentiment for political parties leading up to election day. Using feature engineering and machine learning techniques, it explores which factors most influence sentiment scores and predicts potential outcomes, including how Independent support impacts electoral dynamics.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Methodology](#methodology)
- [Results](#results)
- [Conclusion](#conclusion)
- [Usage](#usage)
- [License](#license)

## Project Overview
This project predicts election-day sentiment for political parties using historical polling data, with a particular focus on understanding the implications of high support for Independent candidates. By building a predictive model, we can gauge which party might have the strongest favorability, revealing trends and public sentiment shifts in response to major events.

## Dataset
The dataset includes historical poll data covering pollster ratings, sentiment scores, sample sizes, and support percentages for candidates from various parties. Each entry reflects a poll with associated metadata (e.g., pollster credibility, methodology, start and end dates).

## Methodology
1. **Data Preprocessing**: Handled missing values, encoded categorical features, and scaled numerical values to standardize inputs for modeling.
2. **Exploratory Data Analysis (EDA)**: Examined distributions, correlations, and relationships to identify key features influencing sentiment.
3. **Predictive Modeling**:
   - **Models Tested**: Linear Regression, Gradient Boosting, and Random Forest.
   - **Hyperparameter Tuning**: Conducted Grid Search on the Random Forest model, achieving the highest accuracy with an R² of 0.989.
   - **Feature Importance**: Analyzed feature impacts, finding `numeric_grade` (pollster rating) to be the most influential factor in predicting sentiment.
4. **Sentiment Prediction**: Applied the tuned model to election-day conditions, predicting sentiment scores across parties.

## Results
The tuned Random Forest model provided reliable predictions, indicating that the Independent party had the highest sentiment score on election day, suggesting strong public favorability. This result demonstrates the influence of non-major parties in shifting electoral dynamics and shaping strategies of major parties in close races.

## Conclusion
This analysis underscores the value of polling data in assessing public sentiment and forecasting election outcomes. By identifying key drivers of sentiment, this model offers a flexible approach for real-time sentiment tracking. While Independent sentiment rarely predicts a win, high support can still influence outcomes by impacting major-party strategies and voter turnout.

## Usage
To replicate this analysis:
1. Clone the repository.
2. Ensure all required dependencies are installed (`pip install -r requirements.txt`).
3. Run the Jupyter notebook to preprocess data, build models, and analyze results.

## License
This project is licensed under the MIT License.

--- 
