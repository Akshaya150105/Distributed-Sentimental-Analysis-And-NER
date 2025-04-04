# Distributed-Sentimental-Analysis-And-NER
# OVERVIEW

This project integrates two distinct NLP pipelines—**Sentiment Analysis** and **Named Entity Recognition (NER)**—into a unified Gradio-based interface, implemented in a distributed manner.

## Sentiment Analysis
This component analyzes customer sentiment from Amazon product reviews, classifying feedback into **positive**, **neutral**, or **negative** categories. It processes large-scale review data, uncovers sentiment trends, evaluates product aspects, and visualizes rating distributions and key terms, empowering stakeholders to understand customer opinions effectively.

## Named Entity Recognition (NER)
This component focuses on extracting named entities (e.g., persons, organizations, locations) from a separate text dataset stored in a specified directory. It preprocesses unstructured text, trains a custom NER model, and enables real-time entity detection, offering a scalable solution for domain-specific entity recognition tasks.

---

# TECHNOLOGIES USED

## Sentiment Analysis
- **Dataset Used**: Amazon Review Dataset
- **SQLite**: Stores and queries structured Amazon review data efficiently.
- **PySpark**: Handles scalable ingestion and preprocessing of large review datasets.
- **spaCy**: Performs tokenization and stopword removal for text preprocessing.
- **Gensim (GloVe)**: Generates word embeddings to capture semantic meaning in reviews.
- **Hugging Face Transformers (BERT)**: Classifies sentiment using a pre-trained BERT model (`nlptown/bert-base-multilingual-uncased-sentiment`).
- **Pandas**: Manages data manipulation and analysis of review datasets.
- **Matplotlib**: Visualizes sentiment trends and rating distributions.
- **WordCloud**: Highlights key terms and phrases in customer feedback.
- **Gradio**: Powers the interactive dashboard for real-time sentiment analysis.

## Named Entity Recognition (NER)
- **Dataset Used**: Gum Dataset (Georgetown University Multilayer Corpus)
- **PySpark**: Preprocesses and manages large text files from a directory, storing them in Parquet format.
- **spaCy**: Trains a custom NER model and extracts entities using pre-trained models (`en_core_web_lg`).
- **srsly**: Creates and handles annotated JSONL data for NER model training.
- **os, glob, random**: Facilitates file handling, directory scanning, and data shuffling for preprocessing.
- **Gradio**: Provides an interactive interface for real-time NER extraction from text or uploaded files.

  OUTPUT:
  Here are some snapshots of our project outcomes
  
  ![image](https://github.com/user-attachments/assets/58dce45a-5b04-4ab7-a689-ff66ceb67ae7)

  ![image](https://github.com/user-attachments/assets/f6509481-594f-4ca6-9538-2f346163f723)

  ![image](https://github.com/user-attachments/assets/28e9452f-c79f-4d7e-851c-a0998fe851d8)

  ![image](https://github.com/user-attachments/assets/d13387cd-533c-4772-bc0e-b205b15e3887)

  ![image](https://github.com/user-attachments/assets/8057f2c6-0ae0-429c-825e-fa6c898dcf3c)

  ![image](https://github.com/user-attachments/assets/4ecb285d-de0c-4ed1-a295-81b4ae20965f)

  ![image](https://github.com/user-attachments/assets/fe7343c8-57cd-401d-9b67-775a6ba10913)
     
