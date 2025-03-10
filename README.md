# Multilingual Text Classification with IndicCorp Dataset

## Overview
This project presents a **Multilingual Text Classification System** using **IndicCorp**, a monolingual dataset with **11 Indic languages**. The methodology integrates **CountVectorizer** for feature extraction and **Multinomial Naïve Bayes** for classification, achieving **73.37% accuracy**.

## Dataset
**IndicCorp** is a vast linguistic resource with **9 billion tokens (~100GB of text data)** covering:
- Hindi, Bengali, Telugu, Marathi, Tamil, Gujarati, Malayalam, Odia, Punjabi, English, and Assamese.
- Data sources: **news articles, literature, web content, and social media**.
- Format: **One sentence per line in a single large text file**.

## Data Preprocessing
To enhance data quality, the preprocessing pipeline includes:
- **Normalization**: Standardizing text format.
- **Tokenization**: Splitting text into words/tokens.
- **Cleaning**: Removing noise, unnecessary symbols, and duplicates.
- **Vectorization**: Converting text into numerical feature vectors.

## Model Architecture
The **Multilingual Text Classification System** follows a robust **machine learning pipeline**:
1. **Data Preprocessing** → Tokenization & Normalization.
2. **Feature Extraction** → Using **CountVectorizer** to create sparse matrices of token counts.
3. **Classification** → **Multinomial Naïve Bayes (MultinomialNB)** for text classification.
4. **Prediction** → The trained model is used for new text classification.

### Performance Metrics
| Metric  | Value |
|---------|--------|
| Accuracy | 73.37% |
| MSE (Mean Squared Error) | 0.13 |
| RMSE (Root Mean Squared Error) | 0.36 |
| Perplexity | 1.002 |

## Results & Discussion
- The model processes data in **batches of 32**, achieving an accuracy **comparable to benchmark results (70%-78%)**.
