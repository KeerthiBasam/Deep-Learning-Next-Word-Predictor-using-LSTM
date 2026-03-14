
# LSTM Next Word Prediction (NLP Language Model)

A deep learning project that predicts the **next word in a sentence** using a trained **LSTM (Long Short‑Term Memory) neural network**.  
The model learns sequential language patterns from text and predicts the most probable next word given a user input sequence.

The project also includes an **interactive Streamlit web application** that allows users to test the model in real time.

---

# Overview

Next word prediction is a fundamental task in **Natural Language Processing (NLP)** and is commonly used in:

- Search engines
- Text auto‑completion
- Chatbots
- Language modeling
- Smart keyboards
- AI writing assistants

This project demonstrates how to build an **end‑to‑end NLP pipeline** including data preparation, tokenization, sequence modeling with LSTM, and deployment with Streamlit.

---

# Key Features

- LSTM based sequence prediction model
- Text preprocessing and tokenization
- Sequence padding for neural network input
- Early stopping during training to avoid overfitting
- Interactive **Streamlit web interface**
- Trained model and tokenizer saved for inference

---

# Project Structure

```
.
├── app.py                                      # Streamlit application for inference
├── experiments.ipynb                           # Model training notebook
├── tokenizer.pickle                            # Saved tokenizer used during training
├── next_word_lstm_model_with_early_stopping.h5 # Final trained LSTM model
├── next_word_lstm.h5                           # Alternative trained model
├── hamlet.txt                                  # Training dataset
├── requirements.txt                            # Python dependencies
└── README.md                                   # Project documentation
```

---

# Technology Stack

- Python
- TensorFlow / Keras
- NumPy
- Streamlit
- NLP preprocessing techniques
- LSTM Recurrent Neural Networks

---

# Model Architecture

The deep learning model follows a typical **language modeling architecture**:

1. Tokenization of text corpus
2. Creation of input sequences
3. Padding sequences to fixed length
4. Training an LSTM network to predict the next word

Typical architecture:

- Embedding Layer
- LSTM Layer
- Dense Softmax Output Layer

Training strategy:
- Early Stopping used to prevent overfitting
- Sequence based training for contextual learning

---

# Installation

Clone the repository:

```
git clone https://github.com/yourusername/lstm-next-word-prediction.git
cd lstm-next-word-prediction
```

Install dependencies:

```
pip install -r requirements.txt
```

---

# Running the Application

Start the Streamlit application:

```
streamlit run app.py
```

After launching, open the local URL provided by Streamlit in your browser.

---

# Example Usage

Input:

```
To be or not to
```

Prediction:

```
Next word: be
```

---

# How It Works

1. User enters a sequence of words.
2. Text is converted into tokens using the trained tokenizer.
3. The sequence is padded to match model input size.
4. The LSTM model predicts the probability distribution of the next word.
5. The word with the highest probability is returned.

---

# Learning Outcomes

This project demonstrates practical understanding of:

- Natural Language Processing pipelines
- Sequence modeling using LSTM
- Neural network training techniques
- Model serialization and reuse
- Building ML powered web apps with Streamlit

---

# Author

Machine Learning / AI Developer  
Focused on NLP, Deep Learning, and AI application development.
