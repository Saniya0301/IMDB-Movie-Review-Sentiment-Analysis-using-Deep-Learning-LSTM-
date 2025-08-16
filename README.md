# 🎬 IMDB Movie Review Sentiment Analysis using Deep Learning (LSTM)

This project performs **sentiment analysis** on the **IMDB movie reviews dataset** using **LSTM (Long Short-Term Memory)** neural networks. The model classifies reviews as either **Positive** or **Negative** based on textual data.

---

## 📂 Dataset
- **Dataset Used**: [IMDB Movie Review Dataset](https://ai.stanford.edu/~amaas/data/sentiment/)
- Contains **50,000 reviews**:
  - 25,000 Positive reviews
  - 25,000 Negative reviews
- Balanced dataset with equal distribution of sentiments.

---

## ⚙️ Tech Stack & Libraries
- **Python**
- **Pandas, NumPy** → Data processing
- **Scikit-learn** → Train-test split
- **TensorFlow / Keras** → Deep Learning (LSTM model)
- **Joblib** → Saving Tokenizer

---

## 🧠 Model Architecture
1. **Embedding Layer** → Converts words into dense vector representations  
2. **LSTM Layer** → Captures sequential dependencies in text  
3. **Dense Layer (Sigmoid Activation)** → Outputs sentiment (0 = Negative, 1 = Positive)  

**Model Summary:**
- Input Dimension: 5000 (top words considered)
- Sequence Length: 200
- Embedding Size: 128
- LSTM Units: 128
- Dropout: 0.2
- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Metrics: Accuracy

---

## 🚀 Steps in Code
1. **Data Loading**  
   ```python
   data = pd.read_csv("IMDB_Dataset.csv")

   
2.Preprocessing

Convert labels: positive → 1, negative → 0

3.Tokenization (limit 5000 words)

Padding sequences (max length = 200)

Train-Test Split (80% training, 20% testing)

4.LSTM Model Building


---
📜 License

This project is open-source and available under the MIT License.


---
Author

SANIYA CHHABRA
