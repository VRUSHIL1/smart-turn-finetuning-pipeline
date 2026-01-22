# Smart-Turn Dictionary Fine-Tuning Pipeline (Hindi & Hinglish)

This repository contains an end-to-end fine-tuning pipeline for training a
language/speech model using Smart-Turn Dictionaries.  
The pipeline is designed to improve turn understanding and intent clarity in
Hindi and Hinglish conversational data, including both complete and incomplete
user utterances commonly seen in real-world voice and chat systems.

---

## Problem Statement

In real conversational AI systems (voice assistants, call-center bots, chatbots):

- Users frequently speak in Hindi or Hinglish
- Utterances are often incomplete, interrupted, or context-dependent
- Traditional models struggle with:
  - Mid-sentence cutoffs
  - Partial intents
  - Code-mixed language (Hindi + English)

Example problematic utterances:
- "haan woh order…"
- "cancel karna hai"
- "delivery ka status"
- "nahi nahi rehne do"

These patterns lead to intent misclassification and turn-boundary errors.

This project addresses these challenges using a Smart-Turn Dictionary–driven
fine-tuning approach.

---

## Solution Overview

This pipeline introduces Smart-Turn Dictionaries to guide the model during
fine-tuning by:

- Encoding conversational turn cues
- Explicitly handling complete vs incomplete utterances
- Supporting Hindi-only and Hinglish (code-mixed) data
- Structuring conversational training data realistically

The trained model learns to:
- Detect when a user has finished speaking
- Interpret partial or interrupted utterances
- Preserve intent even in short or noisy phrases

---

## What This Project Does

- Builds Smart-Turn Dictionaries for conversational signals
- Prepares structured datasets with:
  - Complete utterances
  - Incomplete / cut-off utterances
  - Hindi and Hinglish samples
- Fine-tunes a pretrained model on this data
- Tests and evaluates model predictions using realistic examples

---

## Dataset Characteristics

The training data used in this pipeline includes:

### Languages
- Hindi
- Hinglish (Hindi + English code-mixed)

### Utterance Types
- Complete sentences
- Incomplete or interrupted phrases
- Short intent-driven expressions

### Conversation Style
- Spoken, informal language
- Real-world noisy conversational patterns

This makes the pipeline suitable for production-grade conversational AI systems.

---

## Notebook

- smart_turn_dictionary_finetuning_pipeline.ipynb

The notebook covers:
1. Data loading and preprocessing
2. Smart-turn dictionary construction
3. Model loading and fine-tuning
4. Training configuration
5. Evaluation and sample inference

---

## How to Run

1. Open the notebook in Google Colab
2. Install required dependencies
3. Run all cells sequentially from top to bottom
4. Review training logs and evaluation outputs

---

## Run on Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]
(https://colab.research.google.com/github/VRUSHIL1/smart-turn-finetuning-pipeline/blob/main/smart_turn_dictionary_finetuning_pipeline.ipynb)

---

## Tech Stack

- Python
- PyTorch
- Transformers
- Jupyter Notebook / Google Colab
- Dictionary-based NLP techniques

---

## Skills Demonstrated

- End-to-end model fine-tuning
- Conversational NLP for Hindi and Hinglish
- Handling incomplete and noisy user input
- Dataset design for real-world dialogue systems
- Training, testing, and evaluation pipelines
- Reproducible ML experimentation

---

## Use Cases

- Voice assistants (ASR + NLU)
- Call-center automation
- Conversational chatbots
- Streaming and real-time dialogue systems
- Multilingual and code-mixed NLP applications

---

## Resume-Ready Summary

Built an end-to-end fine-tuning pipeline using smart-turn dictionaries to improve
intent understanding in Hindi and Hinglish conversational data, including
incomplete and interrupted user utterances. Implemented data preprocessing,
model training, and evaluation in a reproducible notebook-based workflow.

