# 🧠 Next Word Prediction using LSTM (Deep Learning + Streamlit)

This project demonstrates a **Next Word Prediction** model built using:
- TensorFlow / Keras (LSTM)
- Tokenizer-based text preprocessing
- Early Stopping
- Streamlit Web App  
- Joblib for saving the tokenizer

The model predicts the *next word* based on the input sequence provided by the user.

---

## 🚀 Live Streamlit App  
🔗 **Streamlit Deployment Link:**  
👉 https://predicitingnextword-8gkzzhfihgrtjbn3hd3hww.streamlit.app/

---

## 📌 Features

- LSTM-based language model
- Trained on n-gram sequences
- Early stopping for efficient training
- One-hot encoded labels
- Streamlit UI for real-time prediction
- Saved model (`LSTM.h5`)
- Saved tokenizer (`tokenizer.pkl`)

---


---

## 🧠 How the Model Works

1. Input text is converted into word indices using the saved tokenizer  
2. The sequence is padded to match model input length  
3. The LSTM model predicts the probability distribution of next words  
4. The most likely word index is selected (`argmax`)  
5. The index is mapped back to its corresponding English word  

---

## 📦 Installation

```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt
streamlit run app.py

