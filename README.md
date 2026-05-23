# 📚 NLP Assignments

A collection of Natural Language Processing (NLP) assignments covering a range of topics — from classical text processing to modern deep learning and transformer-based approaches.

---

## 🗂️ Repository Structure

```
Assignment_NLP/
├── Week 1 Text Foundations/
├── Assignment 1/
├── Assignment 2 21-05-2026/
└── README.md
```

> Each folder contains Jupyter Notebooks (`.ipynb`) covering the respective topic.

---

## 🧠 Topics Covered

| # | Folder | Topic | Description |
|---|--------|-------|-------------|
| 1 | `Week 1 Text Foundations` | Information Extraction | Dependency parsing and syntactic analysis with spaCy's `displacy`, Named Entity Recognition (NER) to extract ORG / GPE / PERSON / DATE entities, and document similarity using TF-IDF vectors and cosine similarity |
| 2 | `Assignment 1` | Text Preprocessing Pipeline | End-to-end text cleaning pipeline including hashtag & URL removal, lowercasing, tokenization, stop word removal, and a comparison of stemming approaches (Porter, Snowball, Lancaster) vs. lemmatization using NLTK and spaCy |
| 3 | `Assignment 2 21-05-2026` | Content-Based Recommendation System | Movie recommendation engine built with TF-IDF vectorization and cosine similarity — preprocesses a custom movie dataset, accepts a free-text user query, and returns the top-3 most relevant results |

---

## 🛠️ Tools & Libraries

| Category | Libraries / Tools |
|----------|-------------------|
| **Language** | Python 3.x |
| **NLP** | NLTK, spaCy (`en_core_web_sm`) |
| **ML / DL** | scikit-learn, PyTorch, TensorFlow |
| **Transformers** | Hugging Face Transformers |
| **Notebooks** | Jupyter Notebook |
| **Environment** | VS Code |

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
pip install -r requirements.txt
```

> If there's no `requirements.txt` yet, install the core libraries manually:
> ```bash
> pip install nltk spacy scikit-learn torch transformers
> python -m spacy download en_core_web_sm
> ```

---

## 🚀 Running an Assignment

Open any assignment folder in VS Code and launch the notebook:

```bash
jupyter notebook "Week 1 Text Foundations/"
```

Or open the `.ipynb` file directly in VS Code with the Jupyter extension.

---

## 👤 Author

**Nihal Pujari**
🔗 [GitHub](https://github.com/Nihalpujari)

---

## 📄 License

This repository is intended for academic purposes. Feel free to use it as a reference.
