# Movie Review Sentiment Analysis

## Project Overview

This project uses Deep Learning and Natural Language Processing (NLP) to classify movie reviews as **Positive** or **Negative**.

A neural network model is trained using the IMDB movie review dataset to understand the sentiment expressed in text reviews.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Jupyter Notebook

## Dataset

The project uses the **IMDB Movie Reviews Dataset**, which contains:

- 25,000 training reviews
- 25,000 testing reviews
- Binary sentiment labels: Positive and Negative

The dataset is limited to the 10,000 most frequent words.

## Model Architecture

The project uses a Sequential Neural Network with the following layers:

1. **Embedding Layer** – Converts words into dense vector representations.
2. **Global Average Pooling Layer** – Reduces the sequence into a fixed-size representation.
3. **Dense Layer** – Learns patterns from the review representations using ReLU activation.
4. **Output Layer** – Uses Sigmoid activation to predict positive or negative sentiment.

### Model Configuration

- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Epochs: 10
- Batch Size: 512
- Maximum Review Length: 500
- Vocabulary Size: 10,000

## Results

The trained model achieved approximately **79% test accuracy**.

The project also includes:
- Training and validation accuracy visualization
- Training and validation loss visualization
- Predictions on custom movie reviews

## Project Structure

```text
movie-review-analysis/
│
├── Movie_Review_Sentiment_Analysis.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Installation and Usage

### 1. Clone the Repository

```bash
git clone https://github.com/kritishp99/movie-review-analysis.git
```

### 2. Navigate to the Project Directory

```bash
cd movie-review-analysis
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Notebook

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Run the cells in `Movie_Review_Sentiment_Analysis.ipynb` to train the model and test predictions.

## Custom Review Prediction

The project includes a prediction function that allows users to enter their own movie reviews and classify them as positive or negative.

Example:

```python
predict_sentiment("The movie was amazing and I really enjoyed it!")
```

## Future Improvements

- Improve model accuracy through hyperparameter tuning.
- Experiment with LSTM and GRU architectures.
- Use pre-trained word embeddings.
- Deploy the model using a web application.

## Conclusion

This project demonstrates how Deep Learning and NLP can be used for sentiment analysis. It provides practical experience in text preprocessing, neural network development, model evaluation, and sentiment prediction.

---

**GitHub Repository:**  
https://github.com/kritishp99/movie-review-analysis
