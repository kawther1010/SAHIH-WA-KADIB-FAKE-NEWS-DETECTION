# 📰 Fake News Detection using BERT

## 📌 Project Description
This project aims to detect fake news using a BERT-based model. It utilizes a dataset scraped from various sources and a merged dataset for improved accuracy. The model is trained to classify news articles as real or fake, enhancing the reliability of online information.

## 🚀 Features
- 🤖 **BERT-based Classification Model**: Leverages transformer architecture for NLP tasks.
- 🗄️ **Scraped & Merged Datasets**: Combines multiple datasets for better generalization.
- 🔍 **Text Preprocessing**: Tokenization, stopword removal, and vectorization.
- 📊 **Performance Metrics**: Evaluates using accuracy, precision, recall, and F1-score.
- 🌐 **Web Scraping Integration**: Optionally allows scraping additional news sources.

## 🛠 Installation
To set up the project, install the required dependencies:

```bash
pip install transformers torch scikit-learn pandas beautifulsoup4 requests nltk
```

## 📂 Dataset
This project uses a combination of scraped data and publicly available fake news datasets. To scrape new data, use:

```python
from scraper import scrape_news
scrape_news("https://example-news-website.com")
```

## 🎯 Model Training
Train the BERT model with:

```bash
python train.py --epochs 5 --batch-size 16 --dataset ./news-dataset.csv
```

## 🔍 Usage
To classify a news article:

```python
from detector import classify_news
text = "Breaking: Scientists discover water on Mars!"
result = classify_news(text)
print("Prediction:", result)
```

## 📈 Evaluation
The model's performance is evaluated using:
- ✅ **Accuracy**
- 📉 **Precision, Recall, and F1-score**

## 🙌 Acknowledgments
- 🌟 **Hugging Face Transformers** for BERT implementation
- 📰 **Various open-source fake news datasets**
- 🧠 **NLP Research Community** for advancements in text classification

## 📜 License
This project is licensed under the **MIT License**.

