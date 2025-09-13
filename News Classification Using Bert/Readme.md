News Classifier using BERT
Overview

This project explores text classification using BERT (Bidirectional Encoder Representations from Transformers) on the AG News dataset. The aim is to automatically categorize news articles into one of four classes: World, Sports, Business, and Sci/Tech.

The implementation leverages the Hugging Face Transformers library, which provides state-of-the-art tools for natural language processing (NLP).

Objectives

Develop a model capable of classifying news articles into predefined categories.

Combine pretrained BERT embeddings with fine-tuning for downstream classification.

Evaluate model performance using accuracy and F1-score.

Dataset

AG News dataset: A benchmark dataset widely used for text classification tasks.

Contains four categories:

World

Sports

Business

Sci/Tech

Each record includes a news article and its corresponding label.

Methodology

Data Loading: The AG News dataset is loaded directly using Hugging Face Datasets.

Preprocessing:

Tokenization with the BERT tokenizer.

Padding and truncation applied to a fixed sequence length.

Labels formatted for supervised training.

Model Setup:

A pretrained BERT base uncased model is adapted for sequence classification.

A classification head with four output classes is added.

Training:

Fine-tuning performed using Hugging Face’s Trainer API.

Training parameters include learning rate scheduling, batch size optimization, and weight decay.

Evaluation:

Metrics used are accuracy and weighted F1-score.

Both training and validation results are monitored.

Results

The model demonstrates strong performance on the AG News dataset, achieving high accuracy even with limited training epochs.

Weighted F1-scores confirm balanced classification across all categories.

Training on a reduced subset of the dataset was used for experimentation, with full training expected to yield even better results.
