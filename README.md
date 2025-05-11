🔤 English to Hindi Translator 🇬🇧➡️🇮🇳

This project translates English sentences to Hindi using a Sequence-to-Sequence model with LSTM and attention. It was built as a learning project for neural machine translation using a small parallel corpus.

📘 Overview

- Built using LSTM-based Encoder-Decoder with Attention
- Trained on English-Hindi sentence pairs
- Includes CLI and optional Streamlit app

📚 Dataset

- Around 30000 English-Hindi sentence pairs
- Basic to moderate complexity
- No pre-trained embeddings used

🧠 Model

- Encoder: Bidirectional LSTM
- Decoder: LSTM with Bahdanau Attention
- Trained using sparse categorical cross-entropy

⚠️ Limitations

- Hindi grammar is complex (gender, tense, context)
- Short training time and small model
- Many out-of-vocabulary words
- Not enough computational power, I had top limit the sentences down to 3000

Despite this, it works well for basic, common sentences and demonstrates how neural translation works.

🧪 Example

Input:  
Where are you going  
Output:  
तुम कहाँ जा रहे हो  

Input:  
She is drinking tea  
Output:  
वह चाय पी रही है  

🛠️ Run Locally

1. Clone and install

   git clone https://github.com/yourusername/EngHindiTranslator.git  
   cd EngHindiTranslator  
   pip install -r requirements.txt

2. Train or load model

   python train.py

3. Translate

   python translate.py  
   or  
   streamlit run app.py

📁 Files

- train.py – Training code  
- translate.py – Translation script  
- app.py – Web UI  
- model.h5 – Trained model  
- tokenizer.pkl – Saved tokenizer

🚀 Future Plans

- Use Transformers (like mT5 or MarianMT)
- Improve accuracy with larger corpus and embeddings
- Add BLEU score evaluation


