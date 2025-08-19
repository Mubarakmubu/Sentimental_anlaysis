# Sentimental_anlaysis
#Sentiment Analysis with BERT and Logistic Regression
#Project Summary
- This project implements a sentiment analysis system that classifies app reviews into three sentiment categories (Negative, Neutral, Positive) using both traditional machine learning (Logistic Regression with TF-IDF) and deep learning approaches (BERT transformer model). The system was trained on a dataset of app reviews with numerical scores that were mapped to sentiment labels.
#📊 Performance Metrics
- BERT Model Performance:
. Accuracy: 84.99%
  
 .F1 Score: 82.46%

 .Validation Loss: 0.4156

- Logistic Regression Performance:
  .Accuracy: 66.23%

  .F1 Score: 57% (weighted average)

The BERT model significantly outperforms the traditional Logistic Regression approach, demonstrating the power of transformer-based models for natural language processing tasks

#⚙️ Workflow
- 1, Data Preparation

     *Load and clean the dataset containing app reviews and scores

     *Map numerical scores (1-5) to sentiment labels:

         Scores 1-2: Negative (0)

          Score 3: Neutral (2)

          Scores 4-5: Positive (1)

- 2 Data Splitting

    .Split data into training (80%) and testing (20%) sets

  - 3 BERT Model Training

. Tokenize text using BERT tokenizer

. Fine-tune BERT-base-uncased model for sequence classification

. Train for 3 epochs with batch size of 8

. Evaluate using accuracy and F1 score

- 4 Logistic Regression Baseline

   .Extract features using TF-IDF vectorization

    .Train logistic regression classifier

     .Compare performance with BERT model

-  5 Model Deployment

   .Save the trained BERT model and tokenizer

    .Create an interactive prediction interface

   
  # Dependencies
  
   .Python 3.10+

  .pandas

 .torch

 .scikit-learn

transformers (Hugging Face)

datasets
