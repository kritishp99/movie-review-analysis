# Movie Review Sentiment Analysis Using TensorFlow

## Project Overview

This project uses **Deep Learning and TensorFlow** to perform text classification on movie reviews. It analyzes the text of a movie review and predicts whether its sentiment is **Positive or Negative**.

The project uses the IMDB Movie Reviews dataset and a Neural Network built using TensorFlow/Keras.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- Jupyter Notebook

## Dataset

The project uses the **IMDB Movie Reviews Dataset** available through TensorFlow/Keras.

- 25,000 training reviews
- 25,000 testing reviews
- Binary sentiment labels:
  - 0 – Negative
  - 1 – Positive

## Model Architecture

The neural network consists of the following layers:

1. **Embedding Layer** – Converts words into dense vector representations.
2. **Global Average Pooling 1D** – Reduces the sequence into a fixed-size representation.
3. **Dense Layer (16 neurons, ReLU)** – Learns patterns from the text.
4. **Output Layer (1 neuron, Sigmoid)** – Predicts positive or negative sentiment.

### Model Configuration

| Parameter | Value |
|---|---|
| Optimizer | Adam |
| Loss Function | Binary Crossentropy |
| Batch Size | 512 |
| Epochs | 10 |
| Maximum Sequence Length | 500 |
| Vocabulary Size | 10,000 |

## Model Performance

The trained model achieved the following result on the test dataset:

| Metric | Result |
|---|---:|
| Test Accuracy | **79%** |
| Epochs | 10 |

The model predicts whether a given movie review expresses positive or negative sentiment.

## Project Structure

```text
movie-review-analysis/
│
├── Movie_Review_Sentiment_Analysis.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

## Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/movie-review-analysis.git
```

### 2. Navigate to the project folder

```bash
cd movie-review-analysis
```

### 3. Install the required libraries

```bash
pip install -r requirements.txt
```

### 4. Run the notebook

Open the notebook using Jupyter Notebook or Google Colab and execute the cells in order.

The IMDB dataset will be downloaded through TensorFlow/Keras when needed.

## Custom Review Prediction

The project includes a prediction function that accepts a movie review and classifies its sentiment.

Example:

```python
predict_review("This movie was wonderful and entertaining!")
```

Possible output:

```text
Predicted sentiment: Positive
```

The prediction depends on the trained model.

## Future Improvements

- Improve model accuracy through hyperparameter tuning.
- Experiment with different neural network architectures.
- Use LSTM or GRU layers for sequence-based learning.
- Build a simple web application for sentiment prediction.
- Improve text preprocessing and prediction performance.

## Conclusion

This project demonstrates how Deep Learning and Natural Language Processing can be used for sentiment analysis. Using TensorFlow and the IMDB dataset, the neural network learns to classify movie reviews into positive and negative categories.

---

**Project:** Movie Review Sentiment Analysis  
**Framework:** TensorFlow / Keras  
**Language:** Python
