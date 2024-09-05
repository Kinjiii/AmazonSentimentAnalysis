# Amazon Review Sentiment Analysis

## Overview
This project analyzes an Amazon review dataset, focusing on sentiment analysis using Natural Language Processing (NLP) techniques, particularly Recurrent Neural Networks (RNNs). The primary objective is to understand customer satisfaction and product sentiment by classifying reviews as positive, negative, or neutral. This information can help Amazon enhance product recommendations, understand customer preferences, and improve overall business strategies.

## Dataset
The dataset includes:
- **Product Title:** The name of the product being reviewed.
- **Customer Review:** The text of the review left by the customer.

### Why This Dataset?
Amazon collects a vast number of customer reviews and ratings for various products, making it an ideal dataset for sentiment analysis. By applying NLP techniques such as RNNs, we can analyze the text of reviews to classify them based on sentiment, providing valuable insights into customer satisfaction.

### Potential Use Cases:
1. **Sentiment Analysis:** Determining whether a review is positive, negative, or neutral can help Amazon understand customer satisfaction and improve product recommendations.
2. **Product Recommendation:** Using RNNs to analyze user reviews, product descriptions, and customer interactions allows for more accurate product suggestions.
3. **Content Generation:** RNNs can generate new, contextually relevant text based on the review content, offering possibilities for creating product descriptions or customer interaction scripts.

## Analysis Workflow
### 1. Exploratory Data Analysis (EDA)
- Initial data exploration is conducted to check assumptions, inspect for anomalies (missing, duplicated, or mis-coded data), and get a sense of the dataset.
- This stage helps determine the types of analyses suitable for the data.

### 2. Data Preprocessing and Cleaning
- Clean the text data by removing null values and irrelevant characters.
- Tokenize the text data, converting it into sequences of integers that can be processed by the model.
- Pad the sequences to ensure consistent input dimensions, which is crucial for efficient batch processing and model stability.

### 3. Model Creation and Training
- A sequential model is built using:
  - **Bidirectional Long Short-Term Memory (LSTM) Layers:** To capture the context of text sequences from both directions.
  - **Batch Normalization Layer:** To stabilize the learning process and speed up convergence.
  - **Dropout Layer:** To prevent overfitting by randomly dropping units during training.
  - **Dense Layers:** For classification of the input data.
- The model is compiled, trained, and evaluated to assess its performance.

### 4. Model Evaluation and Testing
- Plot accuracy curves for training and validation data to visualize model performance.
- Save the trained model for future use.
- Test the model's predictions to assess its ability to classify review sentiments accurately.

## Purpose
The primary goal of this analysis is to gain insights into the sentiment expressed in Amazon reviews. By understanding these sentiments, Amazon can refine its product strategies and help sellers improve customer satisfaction. A thorough analysis of the data will provide a deeper understanding of customer feedback, driving informed decisions and enhancing overall business outcomes.

## Conclusion
This analysis offers valuable insights into customer sentiment based on Amazon reviews. Understanding these sentiments enables better product recommendations, targeted improvements, and strategic decision-making that can enhance the customer experience on Amazon.

## Author
**Matthew Adamson**

---

Thank you for exploring this sentiment analysis project! Feel free to contribute or reach out with any questions.
