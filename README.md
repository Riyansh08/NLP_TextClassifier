# NLP_TextClassifier



A hybrid model using token embeddings, character embeddings, and positional embeddings for abstract sequence classification.

## Project Overview
This project implements a hybrid model to classify sequences (sentences) within medical abstracts. It combines **pretrained token embeddings** (such as GloVe), **character-level embeddings**, and **positional embeddings** (based on sentence position in the abstract) to capture both semantic meaning and structural information.

The model helps classify abstract sentences into categories such as **Objective**, **Methods**, **Results**, and **Conclusion**.

## Key Features
- **Pretrained Token Embeddings**: Uses pretrained GloVe embeddings to capture word-level semantic relationships.
- **Character-Level Embeddings**: Captures the internal structure of words by embedding individual characters.
- **Positional Embeddings**: Adds information about the sentence's position within the abstract (e.g., "Sentence 1 of 10") to enhance the understanding of abstract structure.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/HybridTextClassifier.git
    cd HybridTextClassifier
    ```

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Training the Model

To train the model on your dataset, use the following command:

```bash
python train.py --data_path /path/to/data --epochs 10
