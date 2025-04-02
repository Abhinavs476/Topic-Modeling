# README: Text Analysis and Topic Modeling Pipeline

## Overview
This script performs text preprocessing, visualization, and topic modeling on academic papers extracted from a ZIP archive. The workflow includes:
- Extracting and reading CSV data
- Cleaning and processing text
- Generating a word cloud for visualization
- Removing stopwords and tokenizing text
- Creating a dictionary and corpus for topic modeling
- Applying Latent Dirichlet Allocation (LDA) for topic extraction
- Visualizing the topics using pyLDAvis

## Prerequisites
Ensure the following Python libraries are installed:
```bash
pip install pandas zipfile wordcloud nltk gensim pyLDAvis
```

## Workflow
1. **Extract Data**: Extracts `papers.csv` from `papers.zip`.
2. **Preprocess Text**: Removes punctuation, converts text to lowercase, and removes stopwords.
3. **Generate Word Cloud**: Creates a visualization of frequent words in the dataset.
4. **Tokenization & Stopword Removal**: Tokenizes sentences and removes common stopwords.
5. **Prepare Corpus & Dictionary**: Creates a dictionary and corpus for topic modeling.
6. **Topic Modeling with LDA**: Uses Gensim's LDA model to identify topics in the dataset.
7. **Visualization**: Generates an interactive topic visualization with pyLDAvis.

## Outputs
- **Word Cloud**: A visual representation of word frequency.
- **LDA Topics**: Extracted topics displayed as keywords.
- **Interactive Topic Visualization**: Saved as `results/outputLDAvis_<num_topics>.html`.

## Running the Script
Simply execute the script in a Python environment:
```bash
python script.py
```

## Notes
- The number of topics (`num_topics`) is set to 10 but can be adjusted.
- Ensure `nltk` stopwords are downloaded before running.
- Output files are saved in the `results/` directory.

This script provides an end-to-end text analysis pipeline, from data extraction to topic modeling and visualization.

