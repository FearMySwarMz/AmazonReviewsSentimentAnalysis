# Sentiment Analysis of Amazon Product Reviews

## Project Overview
This project implements sentiment analysis on Amazon product reviews using multiple text representation techniques, including Word2Vec, GloVe, and BERT embeddings (both frozen and fine-tuned). These representations are combined with machine learning and deep learning models to evaluate their effectiveness on real-world sentiment classification tasks.

The project covers the full NLP pipeline: text preprocessing, embedding generation, feature extraction, model training, and performance evaluation.

## Objectives
- Perform sentiment analysis on real Amazon review data
- Compare different word and sentence embedding techniques
- Evaluate the impact of frozen vs fine-tuned BERT embeddings
- Gain hands-on experience with NLP and distributed word representations

## Technologies & Libraries
- Python
- Jupyter Notebook
- NumPy
- pandas
- scikit-learn
- gensim (Word2Vec)
- Pre-trained GloVe embeddings
- Hugging Face Transformers (BERT)

## Workflow

### 1. Text Preprocessing
- Cleaning raw review text
- Removing noise such as symbols, numbers, timestamps, and special characters
- Tokenization and normalization

### 2. Text Embeddings
- Training a Word2Vec model on the dataset
- Using pre-trained GloVe embeddings
- Extracting BERT embeddings in frozen mode
- Fine-tuning BERT for sentiment classification

### 3. Review Representation
- Converting each review into a fixed-length feature vector
- Using average word embeddings for Word2Vec and GloVe
- Using the [CLS] token representation for BERT-based models

### 4. Sentiment Classification
- Training machine learning classifiers to predict positive or negative sentiment
- Comparing traditional ML approaches with deep learning-based methods

### 5. Evaluation & Model Comparison
- Evaluating model performance using:
  - Accuracy
  - Precision
  - Recall
  - F1-score
- Comparing the effectiveness of each embedding technique

## Results & Insights
The project highlights the strengths and limitations of different text representation techniques. Fine-tuned BERT models generally outperform traditional embeddings, while Word2Vec and GloVe provide efficient and interpretable baselines.

## Future Improvements
- Experimenting with additional classifiers
- Hyperparameter optimization
- Multi-class sentiment classification
- Incorporating more advanced preprocessing techniques

## Repository Structure
```
├── data/
│   └── amazon_reviews.csv
├── notebooks/
│   ├── preprocessing.ipynb
│   ├── word2vec_training.ipynb
│   ├── glove_embeddings.ipynb
│   ├── bert_frozen.ipynb
│   └── bert_finetuned.ipynb
├── models/
├── results/
└── README.md
```

## License
This project is for educational and research purposes.

## Author
Developed as part of an NLP and Machine Learning experimentation project.
