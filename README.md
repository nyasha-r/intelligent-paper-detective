# intelligent-paper-detective
An NLP-based research paper discovery system that uses text embeddings and similarity search to help users find academic papers related to their interests.

## Overview

Intelligent Paper Detective explores different text representation techniques for searching academic research papers. It combines natural language processing, semantic embeddings, and approximate nearest-neighbor search to retrieve papers based on textual similarity.

## Features

- **Text preprocessing:** Cleans and prepares research paper titles and abstracts.
- **Multiple text representations:** Explores Sentence Transformers (MiniLM), SciBERT, and Word2Vec.
- **Similarity search:** Uses HNSW for approximate nearest-neighbor retrieval.
- **Interactive interface:** Provides a Gradio-based interface for searching papers.
- **Evaluation experiments:** Includes experiments comparing retrieval metrics and search latency.

## Technologies Used

- Python
- NLP and text preprocessing
- Sentence Transformers — MiniLM
- SciBERT
- Word2Vec
- HNSW (`hnswlib`)
- Gradio
- Pandas and NumPy

## How It Works

1. Load and preprocess academic paper titles and abstracts.
2. Generate vector representations using the selected text embedding method.
3. Build an HNSW index for efficient similarity search.
4. Convert a search query into a vector representation.
5. Retrieve and display papers with similar representations.

## Getting Started

The project was developed using Google Colab.

1. Clone or download this repository.
2. Open the notebook in Google Colab.
3. Install the required dependencies.
4. Configure the dataset path and any required preprocessing steps.
5. Run the notebook cells in order.

**Note:** The notebook may require access to the original dataset and regenerated embeddings or search indexes. Refer to the notebook for the exact dependencies and data-loading instructions.

## Project Status

This project is a work in progress. Current experiments explore multiple embedding approaches and approximate nearest-neighbor retrieval. Evaluation methodology and reproducibility can be further improved.

## Future Improvements

- Evaluate retrieval quality using relevant-paper judgments and realistic search queries.
- Compare embedding methods on the same dataset and evaluation set.
- Improve reproducibility and document experimental results.
- Evaluate search robustness and end-to-end query latency.

## Author

Nyasha Singh

Master's Student, University of Aizu, Japan
