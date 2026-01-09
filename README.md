# Topic Modelling for Articles and Comments

This project applies **unsupervised topic modelling** techniques to analyze large-scale textual data from articles and user comments. The goal is to uncover latent themes, compare topic structures across content types, and measure semantic similarity between articles and public discourse.

The project demonstrates an end-to-end NLP pipeline, including text preprocessing, topic extraction using **Latent Dirichlet Allocation (LDA)**, visualization with word clouds, and similarity analysis using cosine similarity.

---

## 📌 Objectives

- Identify dominant topics in **user comments**
- Identify dominant topics in **news/articles**
- Compare and relate themes across articles and comments
- Quantify similarity between article topics and comment topics
- Visualize topic structures for interpretability

---

## 🗂️ Data Description

The analysis uses two primary datasets:

**Comments Dataset**
- Text-based user comments
- Includes metadata such as author, timestamps, and article references

**Articles Dataset**
- Headline
- Abstract
- Lead paragraph
- Publication date

For articles, relevant text fields are merged into a single combined text column prior to modelling.

---

## 🔄 Methodology

### 1. Text Preprocessing
- Lowercasing
- Removal of punctuation, numbers, and special characters
- Stopword removal (NLTK)
- Tokenization
- Lemmatization using WordNet

### 2. Feature Engineering
- Text vectorization using **CountVectorizer**
- Stopword filtering during vectorization
- Bag-of-Words representation

### 3. Topic Modelling
- Applied **Latent Dirichlet Allocation (LDA)** separately to:
  - Comments
  - Articles
- Extracted top keywords per topic
- Experimented with number of topics for interpretability

### 4. Topic Visualization
- Generated **WordClouds** for each topic
- Visual inspection to validate semantic coherence of topics

### 5. Topic Comparison
- Topics extracted independently for articles and comments
- Keyword overlap analysis
- Comparative interpretation of public discourse vs published content

### 6. Similarity Analysis
- Combined articles and comments into a shared vector space
- Computed **cosine similarity matrix**
- Identified which comments most closely align with which articles

---

## 📊 Key Outputs

- Topic keywords for each LDA topic
- WordCloud visualizations per topic
- Topic similarity matrix (Articles × Comments)
- Interpretable mapping between article themes and public sentiment

---

## 🧠 Example Topics Identified

**Comments Topics (Sample):**
- Electric vehicle charging infrastructure
- Energy sources and emissions
- Climate change and public policy
- Cost and adoption barriers of EVs
- Political discourse around energy

**Articles Topics (Sample):**
- Tesla and EV market trends
- Climate policy and global warming
- Innovation in smart mobility
- Charging technology and infrastructure
- Automotive industry developments

---

## 🛠️ Tech Stack

- **Python**
- **Pandas** – Data manipulation
- **NLTK** – Text preprocessing
- **Scikit-learn** – LDA, vectorization, similarity metrics
- **Matplotlib** – Visualization
- **WordCloud** – Topic visualization


---

## 🚀 How to Run

1. **Clone the repository**
```bash
   git clone <repository-url>
   cd <repository-name>
```

2. **Install dependencies**
```bash
   pip install pandas nltk scikit-learn matplotlib wordcloud
```

3. **Download NLTK resources** (first run only)
```python
   import nltk
   nltk.download('punkt')
   nltk.download('stopwords')
   nltk.download('wordnet')
```

4. **Run the notebook**
```bash
   jupyter notebook "Topic Modelling_Talha.ipynb"
```

---

## 📈 Extensions & Future Work

- Use BERTopic or transformer-based topic models
- Dynamic topic modelling over time
- Sentiment-aware topic modelling
- Interactive dashboards (Tableau / Plotly)
- Topic evolution across publication dates

---

## 👤 Author

**Talha Gulzar**  
MS in Business Analytics  
Babson College
