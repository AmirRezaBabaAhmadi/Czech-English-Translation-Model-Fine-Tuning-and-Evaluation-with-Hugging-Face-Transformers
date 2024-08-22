# Czech to English Translation Model

This repository contains code for training and evaluating a sequence-to-sequence model for translating Czech text to English. The model leverages the Helsinki-NLP pre-trained model and tokenizers. The project demonstrates data preparation, model fine-tuning, and evaluation using BLEU score.

## Overview

This project performs the following tasks:
1. **Dataset Loading:** Utilizes the Helsinki-NLP dataset for Czech-English translation.
2. **Model and Tokenizer Setup:** Loads pre-trained models and tokenizers.
3. **Data Preparation:** Tokenizes and preprocesses the data for training.
4. **Training Configuration:** Sets up training parameters and trains the model.
5. **Evaluation:** Evaluates the model's performance using BLEU score.

## Model Details

The model used in this project is **Helsinki-NLP/opus-mt-cs-en**. This is a pre-trained sequence-to-sequence (Seq2Seq) model designed for translation from Czech (`cs`) to English (`en`).

### Key Details:
- **Model Name:** Helsinki-NLP/opus-mt-cs-en
- **Model Type:** Sequence-to-Sequence (Seq2Seq) model
- **Pre-trained For:** Czech to English translation
- **Source:** Helsinki-NLP's OPUS-MT models, which are available on the Hugging Face Model Hub.

### Explanation:
- **AutoModelForSeq2SeqLM:** This class from the `transformers` library loads the pre-trained Seq2Seq model. In this case, it specifically loads the `Helsinki-NLP/opus-mt-cs-en` model.
- **AutoTokenizer:** This class loads the tokenizer corresponding to the model. The tokenizer handles the conversion between text and tokens that the model can process.

The `Helsinki-NLP/opus-mt-cs-en` model is part of the OPUS-MT project by Helsinki-NLP, which provides a variety of translation models for different language pairs based on the Marian NMT framework.

## Installation

To run the code, you need to install the required libraries. You can install them using pip:

```bash
pip install datasets transformers sentencepiece transformers[torch] sacrebleu evaluate accelerate -U gradio
