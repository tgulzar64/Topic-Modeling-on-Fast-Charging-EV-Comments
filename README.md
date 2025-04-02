# Topic-Modeling-on-Fast-Charging-EV-Comments
This project applies Topic Modeling to analyze public opinions and trends around Fast Charging Electric Vehicles (EVs) using Natural Language Processing (NLP).The goal was to uncover the most discussed themes and concerns in reader comments, helping inform EV strategy, communication, and innovation.

## Data Source:
Extracted reader comments using the New York Times Comments API.

Focused specifically on articles and discussions related to Fast Charging EVs.

## Project Workflow:
Data Collection:

Pulled comments via the NYT API and saved them to a structured dataset for analysis.

## Preprocessing:

Converted all text to lowercase

Removed punctuation, stopwords, and numeric characters

Performed lemmatization for reducing words to base forms

## Topic Modeling:

Implemented Latent Dirichlet Allocation (LDA) via gensim

Tuned for the best number of topics

Extracted and labeled top keywords per topic for interpretation

## Visualization:

Used WordClouds and matplotlib for visual representation of topic clusters

Showcased real sample comments alongside their identified topics

# Tech Stack:
pandas, nltk, gensim, matplotlib, wordcloud, scikit-learn

# File Included:
Topic Modelling_Talha.ipynb: Complete Jupyter Notebook with data cleaning, modeling, and visualization.
