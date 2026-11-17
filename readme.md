# Customer Review Sentiment Analysis using NLP and LSTM

## Project Overview

This project focuses on developing a Natural Language Processing (NLP) and Deep Learning-based sentiment analysis system to classify customer reviews as **Positive or Negative**.

The project uses an LSTM (Long Short-Term Memory) neural network to understand sequential patterns in textual data and predict the sentiment expressed in customer reviews.

The model is trained using the IMDB movie review dataset available in Keras.

## Objectives

- Perform text cleaning and preprocessing.
- Convert textual data into numerical representations.
- Implement Bag of Words and TF-IDF techniques.
- Understand word embeddings.
- Develop an LSTM-based sentiment classification model.
- Evaluate model performance using appropriate metrics.
- Generate predictions for new customer reviews.

## Dataset Details

**Dataset:** IMDB Movie Reviews Dataset

**Source:** TensorFlow Keras Built-in Dataset

Dataset information:

| Description | Details |
|---|---|
| Total Reviews | 50,000 |
| Training Samples | 25,000 |
| Testing Samples | 25,000 |
| Vocabulary Size | 10,000 |
| Number of Classes | 2 |
| Maximum Sequence Length | 200 |

### Target Variable

- `0` – Negative Sentiment
- `1` – Positive Sentiment

## Technologies and Libraries Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- NLTK

## Project Workflow

### 1. Text Data Preparation

The text preprocessing stage includes:

- Loading the IMDB dataset.
- Converting numerical sequences into readable text.
- Text cleaning and normalization.
- Tokenization.
- Stopword removal.
- Stemming using Porter Stemmer.
- Word indexing.
- Sequence generation.
- Padding sequences.
- Training and validation splitting.

### 2. Text Representation

Three NLP text representation techniques were explored.

**Bag of Words (BoW)**

Converts text into numerical vectors based on word frequency.

**TF-IDF**

Represents words based on their importance within documents.

**Word Embeddings**

Converts words into dense numerical vectors that can learn semantic relationships.

### 3. LSTM Model Development

An LSTM-based neural network was developed for binary sentiment classification.

**Model Architecture:**

1. Input Layer
2. Embedding Layer
3. LSTM Layer (64 Units)
4. Dropout Layer (0.5)
5. Dense Layer (1 Neuron with Sigmoid Activation)

**Model Configuration:**

| Parameter | Value |
|---|---|
| Vocabulary Size | 10,000 |
| Embedding Dimension | 128 |
| Sequence Length | 200 |
| LSTM Units | 64 |
| Dropout | 0.5 |
| Optimizer | Adam |
| Loss Function | Binary Crossentropy |
| Batch Size | 64 |
| Epochs | 5 |

### 4. Model Evaluation

The model is evaluated using the following performance metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix

The following visualizations are generated:

- Training vs Validation Accuracy
- Training vs Validation Loss
- Confusion Matrix
- Actual vs Predicted Sentiment Comparison

### 5. Sentiment Prediction

The trained model can predict the sentiment of new textual reviews.

Example:

**Input:**
"This movie was amazing and I really enjoyed it."

**Expected Sentiment:** Positive

**Input:**
"This movie was boring and very disappointing."

**Expected Sentiment:** Negative

## Performance Analysis

The project examines the following aspects:

- Impact of sequence length on model performance.
- Importance of the embedding layer.
- Effect of LSTM memory cells.
- Overfitting and regularization techniques.
- Limitations of the sentiment classification model.

### Overfitting Prevention

Dropout regularization and Early Stopping are explored to reduce overfitting and improve generalization.

### Model Limitations

- Difficulty understanding sarcasm.
- Limited understanding of complex language.
- Unknown words may affect predictions.
- Performance may vary across different domains.
- Training requires computational resources.

## Project Structure

```text
NLP-Sentiment-Analysis-LSTM/
│
├── notebooks/
│   └── sentiment_analysis.ipynb
│
├── models/
│   └── imdb_sentiment_lstm.keras
│
├── screenshots/
│
├── README.md
│
└── requirements.txt
```

## Installation and Execution

### Step 1: Clone the Repository

```bash
git clone https://github.com/Karthikd1818/NLP-Sentiment-Analysis-LSTM.git
```

### Step 2: Navigate to the Project

```bash
cd NLP-Sentiment-Analysis-LSTM
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Run the Notebook

```bash
jupyter notebook
```

Open `sentiment_analysis.ipynb` and execute the cells sequentially.

## Conclusion

This project demonstrates how Natural Language Processing and Deep Learning techniques can be used to analyze textual data and classify customer reviews based on sentiment.

By implementing Bag of Words, TF-IDF, Word Embeddings, and LSTM, the project explores different approaches to text representation and sentiment classification.

The LSTM model learns sequential patterns from movie reviews and generates positive or negative sentiment predictions.

This project provides practical experience in NLP preprocessing, text representation, sequential modeling, deep learning, and model evaluation.

## Author

**Karthik**

- GitHub: [Karthikd1818](https://github.com/Karthikd1818)
- LinkedIn: [LinkedIn Profile](https://linkedin.com/in/karthik02052005/)

---

**Project Category:** Natural Language Processing | Deep Learning | Sentiment Analysis