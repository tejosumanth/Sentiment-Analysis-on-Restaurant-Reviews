# Sentiment-Analysis-on-Restaurant-Reviews using DistlBERT, LSTM and GRU

This project focuses on sentiment analysis of textual reviews using state-of-the-art natural language processing (NLP) techniques. The project utilizes DistilBERT for sequence classification, combined with text preprocessing steps such as tokenization, stemming, and lemmatization. Additionally, it includes experiments with LSTM and GRU models to explore different deep learning architectures for sentiment prediction.

Project Overview
Dataset: The project uses a dataset of reviews with labeled sentiments (positive or negative). The dataset is preprocessed to remove noise, lowercased, and cleaned of punctuation and stopwords. It is then tokenized and further processed with stemming and lemmatization.

Models Used:

DistilBERT: A distilled version of BERT, used for sequence classification with custom dropout layers to prevent overfitting.
LSTM: A Long Short-Term Memory network is employed to capture the sequential nature of text data, with hyperparameter tuning for optimization.
GRU: A Gated Recurrent Unit network is also explored as an alternative to LSTM for sequential data processing.
Evaluation Metrics:

Accuracy: Measures the percentage of correct predictions.
ROC-AUC: Area Under the Receiver Operating Characteristic curve, indicating model performance.
Confusion Matrix: Provides insight into the model's classification performance across different classes.
Precision, Recall, F1-Score: Additional metrics to assess the model’s performance in binary classification tasks.
Project Structure
Data Preprocessing:

Lowercasing, punctuation removal, stopword removal.
Stemming using PorterStemmer.
Lemmatization using WordNetLemmatizer.
Tokenization using DistilBERT's tokenizer.
Word2Vec embeddings are also created for use with LSTM/GRU models.
Model Training:

DistilBERT: Custom TensorFlow model with dropout layers. The model is fine-tuned on the preprocessed data.
LSTM: Sequential model with hyperparameter tuning through grid search.
GRU: Sequential model trained on Word2Vec embeddings with dropout layers to prevent overfitting.
Evaluation:

Performance metrics are computed using sklearn.
ROC-AUC curve plotted to visualize model performance.
Prediction:

Custom sentiment predictions for new reviews, using trained models.
Results
The project demonstrates the effectiveness of different NLP techniques and deep learning models in sentiment analysis.
It highlights the trade-offs between using transformers like DistilBERT and traditional RNN-based models like LSTM and GRU.
