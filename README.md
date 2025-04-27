# sentiment_analysis
# Simple Movie Review Sentiment Analysis using a Lexicon Approach

## Overview

This project implements a basic sentiment analysis system for movie reviews. It determines whether a review expresses a positive, negative, or neutral sentiment by using a predefined lexicon (dictionary) of words associated with different emotional tones.

## Steps Performed

1.  **Data Loading and Preprocessing:** The movie review dataset was loaded using Pandas. Simple text preprocessing steps were applied, including converting text to lowercase and removing basic punctuation.
2.  **Sentiment Lexicon Creation:** A Python dictionary was created, containing common positive (e.g., "happy", "good", "love") and negative (e.g., "bad", "terrible", "hate") words, each assigned a sentiment score (+1 for positive, -1 for negative).
3.  **Sentiment Score Calculation:** For each movie review, the system checked for the presence of words from the sentiment lexicon and calculated a total sentiment score by summing the scores of the matched words.
4.  **Sentiment Classification:** Based on the overall sentiment score, each review was categorized as positive, negative, or neutral using predefined thresholds.
5.  **Evaluation:** The performance of the sentiment analysis system was evaluated by calculating the accuracy, comparing the predicted sentiment labels with the actual sentiment labels (if available in the dataset).

## Results

* **Overall Accuracy:** [Insert the accuracy percentage you obtained here, e.g., 12.21%]
* **Predicted Sentiment Distribution:**
    * Positive Reviews: [Insert the number or percentage of positive reviews]
    * Negative Reviews: [Insert the number or percentage of negative reviews]
    * Neutral Reviews: [Insert the number or percentage of neutral reviews]
* **Example Reviews:**
    * **Positive:** "This movie was absolutely fantastic! I really enjoyed the great acting and wonderful story."
    * **Negative:** "The film was terrible and a complete waste of time. I hated every single scene."
    * **Neutral:** "The movie had some interesting parts, but overall it was just okay."

## How to Use

1.  Make sure you have Python and the Pandas library installed (`pip install pandas`).
2.  Clone this repository to your local machine.
3.  Ensure the movie review dataset (`training.1600000.processed.noemoticon.csv` or your specific dataset) is in the `./dataset` folder (or adjust the file path in the code).
4.  Run the Python script (e.g., `your_script_name.py` or the Jupyter Notebook).

## Discussion and Conclusion (Optional)

The lexicon-based approach provides a simple way to perform sentiment analysis but has limitations in capturing the nuances of language. The low accuracy observed highlights the need for more sophisticated techniques, such as incorporating a more comprehensive lexicon, considering word weights, handling negation, and potentially using machine learning models for improved performance.