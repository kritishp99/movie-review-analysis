# Movie Review Sentiment Analysis Using TensorFlow

## Project Overview

This project uses Deep Learning and TensorFlow to perform **Text Classification** on movie reviews. It analyzes the text of a movie review and classifies its sentiment as either **Positive** or **Negative**.

The project uses the IMDB Movie Reviews dataset and a Neural Network built using TensorFlow/Keras.

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib

## Dataset

The project uses the built-in **IMDB Movie Reviews Dataset** provided by Keras.

- 25,000 training reviews
- 25,000 testing reviews
- Binary sentiment labels:
  - 0 – Negative
  - 1 – Positive

The dataset is loaded using `tensorflow.keras.datasets.imdb` with the 10,000 most frequent words.

## Model Architecture

The project uses a Sequential Neural Network with the following layers:

1. **Embedding Layer** – Converts words into dense vector representations.
2. **Global Average Pooling 1D** – Reduces the sequence into a single feature vector.
3. **Dense Layer** – 16 neurons with ReLU activation.
4. **Output Layer** – 1 neuron with Sigmoid activation for binary classification.

### Model Configuration

- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Evaluation Metric: Accuracy
- Batch Size: 512
- Maximum Sequence Length: 500
- Vocabulary Size: 10,000

## Installation

Install the required libraries:

```bash
pip install tensorflow numpy pandas matplotlib
```

## How to Run

1. Clone this repository:

```bash
git clone https://github.com/YOUR-USERNAME/movie-review-sentiment-analysis.git
```

2. Open the project folder.
3. Launch Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `TensorFlow_Final (1).ipynb`.
5. Run the notebook cells in order.

The IMDB dataset is downloaded automatically when the notebook loads it for the first time.

## Results

The model evaluates its performance using test accuracy and visualizes training and validation accuracy using Matplotlib.

## Model Saving

The trained model is saved in Keras format:

```python
keras.saving.save_model(model, "my_model.keras")
```

## Future Improvements

- Improve prediction on custom movie reviews.
- Experiment with different neural network architectures.
- Improve model accuracy and generalization.
- Deploy the model as a web application.

---

**Project Type:** Deep Learning | Natural Language Processing | Text Classification

**Framework:** TensorFlow / Keras
