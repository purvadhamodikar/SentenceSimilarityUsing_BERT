# Sentence Similarity using BERT in NLP

## Overview

This repository contains code for a Natural Language Processing (NLP) project that focuses on measuring sentence similarity using BERT (Bidirectional Encoder Representations from Transformers). The goal is to leverage pre-trained BERT models to calculate the similarity between pairs of sentences.

## Table of Contents

- [Introduction](#introduction)
- [Installation](#installation)
- [Examples](#examples)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Sentence similarity is a crucial task in various NLP applications, such as duplicate detection, paraphrase identification, and information retrieval. BERT, being a state-of-the-art transformer-based model, has demonstrated remarkable performance in various NLP tasks.

This project provides a Python implementation for sentence similarity using BERT. It utilizes the Hugging Face Transformers library for easy integration with pre-trained BERT models.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/purvadhamodikar/SentenceSimilarityUsing_BERT
    ```

2. Change to the project directory:

    ```bash
    cd SentenceSimilarityUsing_BERT
    ```

3. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

## Examples

Here's an example of how to use the code:

```python
from sentence_similarity import SentenceSimilarity

# Initialize SentenceSimilarity with a pre-trained BERT model
similarity_calculator = SentenceSimilarity(model_path='path/to/pretrained/bert')

# Compare two sentences
sentence1 = "The quick brown fox jumps over the lazy dog."
sentence2 = "A fast brown fox leaps over a sleepy canine."

similarity_score = similarity_calculator.calculate_similarity(sentence1, sentence2)

print(f"Similarity Score: {similarity_score}")
