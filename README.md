🧠 Text Preprocessing and Vectorization using NLTK and Scikit-learn
This project demonstrates a complete pipeline for text preprocessing and feature extraction in Natural Language Processing (NLP), using a well-known speech paragraph. It covers the cleaning of raw text and transforming it into numerical vectors using Bag of Words (BoW) and TF-IDF (Term Frequency–Inverse Document Frequency).

📌 Objective
The goal of this project is to showcase how raw textual data can be prepared for machine learning models by:

Breaking it into sentences and words

Cleaning and normalizing the text

Removing noise (stopwords, punctuation)

Extracting meaningful features using BoW and TF-IDF

This forms the first and essential step in any NLP pipeline.


⚙️ Workflow Explained
Here is a breakdown of what the script does:

1. Input Text
A paragraph (e.g., a speech or article) is taken as input.

2. Text Cleaning and Preprocessing
Sentence Tokenization: The text is split into sentences using nltk.sent_tokenize.

Regex Cleaning: Non-alphabetic characters are removed.

Lowercasing: All words are converted to lowercase.

Tokenization: Each sentence is broken into individual words.

Stopword Removal: Common English words like "the", "is", "and" are removed.

Lemmatization: Words are reduced to their root form (e.g., "running" → "run") using WordNetLemmatizer.

3. Corpus Creation
Each cleaned sentence is joined back into a string and stored in a list called corpus, which contains all processed text.

4. Feature Extraction
Two vectorization techniques are applied:

Bag of Words (BoW):

Converts text into a matrix of token counts.

Each row represents a sentence; each column represents a word.

Values represent the frequency of the word in that sentence.

TF-IDF (Term Frequency-Inverse Document Frequency):

Similar to BoW, but weighs words based on how unique they are across all sentences.

Words that appear in many sentences get lower scores, making the model more focused on unique or important terms.

🛠 Libraries Used
NLTK for natural language processing tasks (tokenization, stopwords, lemmatization)

Scikit-learn for feature extraction (BoW and TF-IDF)

re (Regular expressions) for text cleaning

📈 Why This Matters
Text preprocessing is crucial in NLP because raw text is messy. Models perform much better when the text is cleaned, normalized, and vectorized correctly. This small project demonstrates a foundational skill set in NLP pipelines for task like:

Sentiment analysis

Text classification

Information retrieval

Chatbots
