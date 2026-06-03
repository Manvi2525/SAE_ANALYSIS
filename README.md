# SAE Analysis of Fine-Tuned Language Models

## Overview

This project studies how fine-tuning affects the internal feature space of Pythia-160M using Sparse Autoencoders (SAEs).

The workflow consists of:

1. Fine-tuning Pythia-160M on PubMed abstracts
2. Extracting layer-6 activations
3. Training SAEs on both base and fine-tuned activations
4. Comparing learned features

## Key Findings

- 96.3% of SAE features remained stable after fine-tuning
- Only 3.7% of features exhibited substantial changes
- Medical concepts such as "lymphoma" appeared in newly activated features
- Overall activation density remained unchanged
- Decoder cosine similarity failed due to feature rotation

## Notebooks

- finetune.ipynb
- collect_activations.ipynb
- train_sae.ipynb
- compare_features.ipynb

## Model Weights and Activation Caches

Google Drive links:

https://drive.google.com/drive/folders/1x4FmXtCL6wl7uJXtOD2vJGfL-JpP1pKQ?usp=drive_link
