# Czech to English Translation Model

This repository contains code for training and evaluating a sequence-to-sequence model for translating Czech text to English. The model leverages the Helsinki-NLP pre-trained model and tokenizers. The project demonstrates data preparation, model fine-tuning, and evaluation using BLEU score.

## Overview

This project performs the following tasks:
1. **Dataset Loading:** Utilizes the Helsinki-NLP dataset for Czech-English translation.
2. **Model and Tokenizer Setup:** Loads pre-trained models and tokenizers.
3. **Data Preparation:** Tokenizes and preprocesses the data for training.
4. **Training Configuration:** Sets up training parameters and trains the model.
5. **Evaluation:** Evaluates the model's performance using BLEU score.

## Installation

To run the code, you need to install the required libraries. You can install them using pip:

```bash
pip install datasets transformers sentencepiece transformers[torch] sacrebleu evaluate accelerate -U gradio
