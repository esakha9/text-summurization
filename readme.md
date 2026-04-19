# News Summarization Project

## Overview

This project builds a text summarization system using the **BART (Bidirectional and Auto-Regressive Transformer)** model.
It is trained on the CNN/DailyMail dataset to generate concise summaries from long news articles.

---

## Project Structure

```
news-summarizer/
│
├── data_preprocessing.py   # Data cleaning and preparation
├── train.py                # Model training pipeline
├── requirements.txt        # Dependencies
├── README.md               # Project documentation
├── .gitignore              # Ignore unnecessary files
├──model.safetensors        # model file 
```
Trained Model

The trained model is too large to upload on GitHub.

👉 Download it from Google Drive:
https://drive.google.com/file/d/1LwT8_3SdVrnyjYyOgqGaMmEpB6xMFL4r/view?usp=drive_link
---

## Model Details

* Model: `facebook/bart-base`
* Task: Abstractive Text Summarization
* Dataset: CNN/DailyMail
* Framework: Hugging Face Transformers

---

## Installation

```bash
pip install -r requirements.txt
```

---

## Data Preparation

* Remove unnecessary columns (like `id`)
* Clean text (remove newlines, spaces)
* Truncate long articles
* Convert to HuggingFace Dataset format

---

## Training

```bash
python train.py
```

Training includes:

* Tokenization (text → numbers)
* Model learning (BART)
* Loss optimization
* Checkpoint saving

---

## 📊 Evaluation

Model performance is evaluated using **ROUGE metrics**:

* ROUGE-1
* ROUGE-2
* ROUGE-L


---

## 💡 Future Improvements

* Use `bart-large` for better performance
* Hyperparameter tuning
* Deploy as API (Flask / FastAPI)
* Add web interface

---

## Author

Esa khan
AI Engineer

---

## ⭐ Acknowledgements

* Hugging Face Transformers
* CNN/DailyMail Dataset
