# 🚀 FastSearch50K

**FastSearch50K** is a blazing-fast semantic search engine that uses the Vector Space Model (TF-IDF + Cosine Similarity) to search over 50,000+ documents in under 500 milliseconds per query. Designed for performance and scalability, this project is ideal for NLP-based search systems and can be easily extended with ANN techniques like FAISS or full inverted index systems.

---

## ✨ Features

- 🔍 Vector Space Search (TF-IDF)
- ⚡ Query time < 500 ms on 50k documents
- 🧠 Cosine similarity scoring
- 🧹 NLP preprocessing (stopwords removal, lowercasing)
- 📂 Google Colab-compatible
- 📦 Easily extensible to large-scale or ANN-based systems

---

## 📁 Project Structure

```plaintext
FastSearch50K/
├── data/
│   └── docs.txt                 # 50k documents (or generated if not found)
│
├── indexing/
│   └── tfidf_vectorizer.py      # TF-IDF vectorizer and document embedding
│
├── search/
│   └── search_engine.py         # Main search logic using cosine similarity
│
├── utils/
│   └── text_preprocessing.py    # Stopword removal, cleaning, tokenization
│
├── colab_notebook.ipynb         # Interactive Google Colab notebook
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation


---

## 📌 How It Works

1. Loads a dataset of 50,000 documents (or auto-generates dummy ones).
2. Preprocesses each document (stopwords removal, lowercase, tokenization).
3. Vectorizes the corpus using **TF-IDF**.
4. Accepts user queries, vectorizes them, and performs **cosine similarity** search.
5. Returns the top `k` most relevant results in milliseconds.

---

## 🚀 Getting Started (Google Colab)

> No local setup needed — just run in Google Colab!

!pip install -q scikit-learn nltk
Or run the full Colab notebook (Add link when uploading)

🧠 Future Improvements
Integrate FAISS or Annoy for Approximate Nearest Neighbors

Boolean inverted index for exact search

Deploy as a Flask API or FastAPI microservice

Add front-end search UI

🛠 Requirements
Python 3.7+

scikit-learn

nltk

Install with:


pip install -r requirements.txt

👨‍💻 Author
Bishal Sarkar (@Bishu-21)
Contributor, Innovator & Hackathon Enthusiast
GitHub

📄 License
MIT License – use freely, modify wisely.

---

## 📂 Final GitHub Repository Structure

FastSearch50K/
├── data/
│ └── docs.txt
├── indexing/
│ └── tfidf_vectorizer.py
├── search/
│ └── search_engine.py
├── utils/
│ └── text_preprocessing.py
├── colab_notebook.ipynb
├── requirements.txt
└── README.md
---
