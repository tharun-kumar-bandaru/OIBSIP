# Task 5 – Autocomplete and Autocorrect Data Analytics

## Oasis Infobyte – Data Analytics Internship

### Project Overview

This project focuses on developing and analyzing NLP-based **Autocomplete and Autocorrect systems** using a real-world English text corpus.

The autocomplete system predicts the next word using frequency-based **Bigram and Trigram models**, while the autocorrect system identifies and corrects misspelled words using **Levenshtein Edit Distance** and word-frequency information.

---

## Objective

The main objectives of this project are:

- Perform NLP text preprocessing and analysis.
- Analyze word frequencies from a large text corpus.
- Build a Bigram-based autocomplete model.
- Build a Trigram-based autocomplete model.
- Generate the top 3 word predictions for different prefixes.
- Implement an edit-distance-based autocorrect system.
- Test autocorrect on 20+ deliberately misspelled words.
- Compare multiple autocomplete and autocorrect approaches.
- Evaluate model performance using accuracy, precision, and recall.
- Visualize frequent words and autocorrect performance using a confusion matrix.
- Discuss the limitations of the implemented approaches compared with modern production systems.

---

## Dataset

### Wikipedia Text Corpus

The project uses a real-world English **Wikipedia Text Corpus** obtained from Kaggle.

The corpus provides English sentences and paragraphs that are suitable for:

- NLP preprocessing
- Word frequency analysis
- N-gram language modeling
- Autocomplete
- Text prediction

---

## Technologies Used

- Python
- Pandas
- NumPy
- NLTK
- TextDistance
- PySpellChecker
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Workflow

```text
Dataset Collection
       ↓
Data Loading
       ↓
Text Preprocessing
       ↓
Tokenization
       ↓
Word Frequency Analysis
       ↓
Bigram Model
       ↓
Trigram Model
       ↓
Autocomplete Testing
       ↓
Autocorrect Implementation
       ↓
Levenshtein Distance
       ↓
20+ Misspelling Tests
       ↓
Performance Evaluation
       ↓
Visualization
       ↓
Comparison & Conclusion
