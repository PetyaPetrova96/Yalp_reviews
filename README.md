# Scalable Data Processing and ML Model for Yelp Reviews Analysis

## Overview
This project involves analyzing Yelp review data to identify influential businesses, assess language authenticity, test hypotheses on cuisine sentiment, and build predictive models for review ratings.

## Key Components

### 1. Influencer Identification
- **Objective**: Identify businesses reviewed by more than 5 influencers.
- **Method**: Defined influencers as users with over 1,000 reviews.
- **Result**: Identified 4,365 businesses fitting the criteria.

### 2. Language Authenticity Analysis
- **Objective**: Analyze the use of authenticity-related language ("authentic," "legitimate") in restaurant reviews.
- **Dataset**: 17 million reviews across 30+ countries.
- **Finding**: Higher usage of authenticity language in Southern U.S. states compared to Northern states.

### 3. Hypothesis Testing on Cuisine Sentiment
- **Objective**: Test whether "authentic" language is used differently for Asian versus European cuisines.
- **Method**: Conducted sentiment analysis on reviews.
- **Result**: Failed to reject the null hypothesis, indicating no significant difference in language use between Asian and European cuisines.

### 4. ML Model for Review Rating Prediction
- **Objective**: Build a predictive model for review ratings.
- **Method**: 
  - Used HashingTF and IDF for text vectorization.
  - Trained Decision Tree, Linear Regression, and Random Forest models.
- **Result**: Linear Regression model yielded the best performance with a low Mean Squared Error (MSE) on dev and test datasets.

## Technologies Used
- **Data Processing**: PySpark
- **Machine Learning**: Decision Tree, Linear Regression, Random Forest
- **Text Vectorization**: HashingTF, IDF

