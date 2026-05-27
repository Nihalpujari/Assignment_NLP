# 📚 NLP Assignments — SRH University

A collection of Natural Language Processing (NLP) assignments and lab exercises covering classical text processing, vector representations, neural networks, and applied NLP systems.

---

## 🗂️ Repository Structure

```
Assignment_NLP/
├── Week 1 Text Foundations/
│   ├── NLP_Lab_Week1.ipynb
│   └── README.md
├── Assignment 1/
│   └── code.ipynb
├── Assignment 2 21-05-2026/
│   ├── ANSWERED_InformationExtraction.ipynb
│   └── recommendation_system.ipynb
├── Business Scenario_TextRepresentation/
│   └── applicationproject.ipynb
├── FFNN - Sentiment Analysis/
│   └── p1.ipynb
└── README.md
```

---

## 🧠 Topics Covered

### 📁 Week 1 Text Foundations

#### `NLP_Lab_Week1.ipynb` — Core NLP Pipeline

A hands-on lab covering the fundamental building blocks of any NLP pipeline.

| Section | Topic | What's Covered |
|---------|-------|----------------|
| 0 | Setup | Package installation, NLTK downloads, library imports |
| 1 | Tokenization | Whitespace, Regex, NLTK, spaCy, GPT-2 BPE — compared side by side |
| 2 | Stemming & Lemmatization | Porter, Snowball, Lancaster stemmers vs WordNet & spaCy lemmatizers |
| 3 | Stop Words & Cleaning | 5-step pipeline: lowercase → remove URLs → remove punctuation → tokenize → remove stop words |
| 4 | Bag of Words & N-grams | CountVectorizer, unigrams vs bigrams, term frequency analysis |
| 5 | TF-IDF | TfidfVectorizer, mini search engine using cosine similarity |
| 6 | String Similarity | Levenshtein edit distance, Jaccard similarity, cosine similarity |

---

### 📁 Assignment 1

#### `code.ipynb` — Text Preprocessing Pipeline

End-to-end text cleaning and normalization on a real NLP paragraph:

- Hashtag removal using Regex
- Smart lowercasing (preserves acronyms like `AI`, `NLP`)
- NLTK word tokenization
- Stemming vs Lemmatization comparison (Porter, Snowball, Lancaster, spaCy)
- Punctuation removal using Python `string` module

---

### 📁 Assignment 2 (21-05-2026)

#### `ANSWERED_InformationExtraction.ipynb` — Information Extraction

| Task | Tools | What's Done |
|------|-------|-------------|
| Dependency Parsing | spaCy, displacy | Syntactic tree visualization, ROOT identification, ambiguity analysis |
| Named Entity Recognition | spaCy | Extracts ORG, GPE, PERSON, DATE entities from real text |
| Document Similarity | TF-IDF, cosine similarity | Measures similarity between documents; discusses semantic limitations |

#### `recommendation_system.ipynb` — Movie Recommendation Engine

Content-based recommendation system built on a custom 10-movie dataset:

- Full preprocessing pipeline (lowercase, punctuation removal, stopwords, lemmatization)
- TF-IDF vectorization of movie descriptions (141 features)
- Cosine similarity ranking returning top-3 results for any free-text query
- Tested with queries like `"Artificial Intelligence"`, `"Happy new year"`, `"is the earth flat"`

---

### 📁 Business Scenario — Text Representation

#### `applicationproject.ipynb` — Job Applicant Matching System

Matches job applicants' CVs to job descriptions using NLP similarity:

- Dataset of job roles (AI Engineer, Data Engineer, BI Analyst, etc.) and applicant profiles
- Bag of Words matrix built with `CountVectorizer`
- TF-IDF matrix built with `TfidfVectorizer`
- Cosine similarity comparison between BoW and TF-IDF approaches
- Conclusion: TF-IDF produces better differentiation between applicants

---

### 📁 FFNN — Sentiment Analysis

#### `p1.ipynb` — 3-Class Sentiment Classifier

Feed Forward Neural Network built from scratch to classify text into 3 sentiment categories:

| Component | Details |
|-----------|---------|
| Vectorization | TF-IDF (`TfidfVectorizer`) |
| Model | Sequential FFNN — Dense(8, ReLU) → Dense(3, Softmax) |
| Loss | `sparse_categorical_crossentropy` |
| Labels | 0 = Negative, 1 = Positive, 2 = Neutral |
| Training | 100 epochs |
| Visualization | Loss curve and prediction scatter plot with Matplotlib |

---

## 🛠️ Tools & Libraries

| Category | Libraries |
|----------|-----------|
| **Language** | Python 3.x |
| **NLP** | NLTK, spaCy (`en_core_web_sm`) |
| **ML / DL** | scikit-learn, TensorFlow / Keras |
| **Visualization** | Matplotlib, spaCy displacy |
| **Data** | NumPy, Pandas |
| **Notebooks** | Jupyter Notebook / VS Code |

---

## ⚙️ Setup & Installation

### 1. Clone the repository

```bash
git clone https://github.com/Nihalpujari/Assignment_NLP.git
cd Assignment_NLP
```

### 2. Create a virtual environment (recommended)

```bash
python -m venv venv
source venv/bin/activate        # macOS / Linux
venv\Scripts\activate           # Windows
```

### 3. Install dependencies

```bash
pip install nltk spacy scikit-learn tensorflow numpy pandas matplotlib Levenshtein
python -m spacy download en_core_web_sm
```

---

## 👤 Author

**Nihal Pujari**
🔗 [GitHub](https://github.com/Nihalpujari)

---

## 📄 License

This repository is intended for academic purposes. Feel free to use it as a reference.
