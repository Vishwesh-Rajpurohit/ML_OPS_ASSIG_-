# DistilBERT Goodreads Genre Classifier

This repository contains an MLOps assignment on genre classification of Goodreads reviews using DistilBERT. The model was fine-tuned in a Kaggle notebook with GPU support, the experiments were tracked in Weights & Biases, and the final checkpoint was published on Hugging Face Hub.

## Overview

The objective of this work was to build and document a simple end-to-end text classification pipeline. For this, a pre-trained DistilBERT model was adapted to the UCSD Goodreads review dataset and evaluated on a separate test split. The full workflow was executed in Kaggle so that training, logging, and model sharing could be handled in one place.

## Setup

To reproduce the run:

1. Open the Kaggle notebook linked below.
2. In the notebook settings, enable both GPU and Internet.
3. Add the following Kaggle Secrets:
   - `WANDB_API_KEY`
   - `HF_TOKEN`
4. Run all cells in sequence.
5. During execution, the training logs will be recorded in Weights & Biases (Wandb), and the trained model can then be pushed to Hugging Face Hub.

## Results

| Metric | Score |
|---|---:|
| Eval Accuracy | 0.60125 |
| Eval F1 | 0.59813 |
| Eval Loss | 2.38206 |
| Eval Runtime | 15.4646 |
| Eval Samples/Second | 103.462 |
| Eval Steps/Second | 3.233 |
| Test Accuracy | 0.60125 |
| Test F1 | 0.59813 |
| Test Loss | 2.38206 |
| Test Runtime | 15.1941 |

## Project Links

- Kaggle Notebook: [ML_OPS_Assignment](https://www.kaggle.com/code/vishveshrg25ait2130/ml-ops-1/notebook)
- Weights & Biases Dashboard: [W&B Project](https://wandb.ai/g25ait2130-indian-institute-of-technology-jodhpur/huggingface/overview)
- Hugging Face Model: [VishweshR/distilbert-goodreads-genres](https://huggingface.co/VishweshR/distilbert-goodreads-genres/tree/main)

## Remarks

This repository mainly documents the assignment pipeline and its outputs. The emphasis is on showing the complete workflow clearly: Kaggle-based training, experiment tracking through W&B, and public model hosting on Hugging Face.
