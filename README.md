# Lab2: Text Representation and Visualization

This repository contains two Jupyter notebooks exploring different techniques for text representation and visualization.

## `part1.ipynb`

This notebook demonstrates a simple information extraction task using regular expressions. It extracts product information from a text description and generates a bill summarizing the purchase.

**Key functionalities:**

- Utilizes regular expressions to identify and extract product names, quantities, unit prices, and total prices from a text description of a purchase.
- Employs data cleaning techniques to remove stop words and format numerical values.
- Generates a structured bill in a tabular format using the pandas and tabulate libraries, providing a clear overview of the extracted information.

## `part2.ipynb`

This notebook delves into various text vectorization techniques, including:

- One-hot encoding: Creates binary vectors representing the presence or absence of unique words in a corpus.
- Bag-of-Words: Counts the occurrences of frequently used words in a corpus, disregarding word order and context.
- TF-IDF (Term Frequency-Inverse Document Frequency): Assigns weights to words based on their frequency within a document and their rarity across the entire corpus, emphasizing the importance of distinctive words.
- Word Embedding:
  - Word2Vec: Utilizes neural networks to learn word embeddings, capturing semantic and syntactic relationships between words. The notebook explores both CBOW (Continuous Bag-of-Words) and Skip-gram architectures, comparing their results.
  - FastText: Similar to Word2Vec, learns word embeddings but considers subword information, making it effective for handling rare or out-of-vocabulary words. You need to download the pre-trained FastText model from [here](https://fasttext.cc/docs/en/crawl-vectors.html) and place it in the appropriate directory.
  - GloVe (Global Vectors for Word Representation): Leverages word co-occurrence statistics to learn word embeddings, capturing global corpus information. Download the GloVe embeddings from [this Kaggle dataset](https://www.kaggle.com/datasets/watts2/glove6b50dtxt?resource=download) and place the file in the appropriate directory.

**Visualization:**

- Employs t-SNE (t-distributed Stochastic Neighbor Embedding) for dimensionality reduction, enabling the visualization of high-dimensional word embeddings in a 2D space. The notebook presents t-SNE plots for each text vectorization method, providing insights into the relationships and clusters formed by different approaches.

**Usage:**

- The data used in `part2.ipynb` is assumed to have been scraped and preprocessed in Lab1. Ensure that you have the necessary data available or run Lab1 to collect and preprocess the data before executing `part2.ipynb`.

**Conclusions:**

The notebook concludes by emphasizing that the choice of the optimal text vectorization technique depends on the specific task and dataset characteristics. For tasks requiring semantic understanding, Word2Vec, FastText, and GloVe are recommended over simpler methods. Dimensionality reduction techniques like t-SNE are valuable for visualizing and interpreting the results of text vectorization.

## Files in the Repository:

- `part1.ipynb`
- `part2.ipynb`
- `t-SNE Plot for FastText Data.png`
- `t-SNE Plot for GloVe Data.png`
- `t-SNE Plot for One-Hot Encoding Data.png`
- `t-SNE Plot for Word2Vec(CBOW) Data.png`
- `t-SNE Plot for Word2Vec (Skip-gram) Data.png`

