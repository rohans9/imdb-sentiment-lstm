# imdb-sentiment-lstm

## 📌 Overview
This project uses a deep learning model—**LSTM (Long Short-Term Memory)**—to predict the sentiment of IMDb movie reviews. Given a review in plain text, the model classifies it as either **positive** or **negative**. This kind of text classification is a classic example of how NLP (Natural Language Processing) can help automate human opinion analysis.

---

## 🧠 Problem Statement
When people watch a movie, they often head to platforms like IMDb to share what they thought about it. These reviews are helpful not only to other viewers but also to filmmakers, producers, and marketers who want to understand public opinion.

But with thousands of reviews posted every day, manual analysis is not practical.

This project aims to:
- Build a model that can **automatically detect the sentiment** of a review.
- Use **LSTM**, a type of Recurrent Neural Network, to capture the sequence and context of words in a sentence.
- Evaluate the model using **accuracy**, **precision**, **recall**, and **F1-score**.

---

## 📊 Dataset
- **Source:** IMDb Movie Review Dataset
- **Size:** 50,000 total reviews
- **Split:** 25,000 for training, 25,000 for testing
- **Classes:** Binary (Positive or Negative sentiment)
- **Balance:** Evenly balanced

---

## ⚙️ Methodology

1. **Text Preprocessing**
   - Tokenization
   - Padding sequences to ensure equal length
   - Encoding words into integers

2. **Model Architecture**
   - Embedding layer
   - LSTM layer
   - Dense output layer with Sigmoid activation

3. **Training Setup**
   - Loss Function: Binary Crossentropy
   - Optimizer: Adam
   - Metric: Accuracy

4. **Evaluation**
   - Test on unseen data
   - Generate Confusion Matrix and Classification Report

---

## 📈 Evaluation Metrics

- ✅ **Accuracy**
- 📊 **Confusion Matrix**
- 📌 **Precision**
- 📌 **Recall**
- 📌 **F1-score**

---

## ✅ Results
The model successfully classifies reviews with high accuracy. The goal was to achieve **above 85% test accuracy**, and results confirmed that the LSTM model is capable of learning sentiment effectively from the textual data.

---

## 🚀 How to Run

1. Clone this repository or download the Jupyter notebook.

2. Install the required libraries (if not already installed):
   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn tensorflow
