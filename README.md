# DistilBERT Goodreads Genre Classifier

This project fine-tunes **DistilBERT** to classify Goodreads reviews into book genres using a Kaggle notebook with GPU support. The workflow includes model training and evaluation in Kaggle, experiment tracking with Weights & Biases, and model publishing on Hugging Face Hub.

## Project summary

The goal of this project is to build a simple end-to-end MLOps workflow for text classification. A pre-trained DistilBERT model was fine-tuned on the UCSD Goodreads review dataset and evaluated on a held-out test split. The full training workflow was run in Kaggle, tracked in W&B for reproducibility, and the final trained model was pushed to a public Hugging Face repository.

## Setup instructions

1. Open the Kaggle notebook linked below.
2. Enable GPU and Internet in the Kaggle notebook settings.
3. Add the required Kaggle Secrets:
   - `WANDB_API_KEY`
   - `HF_TOKEN`
4. Run the notebook from top to bottom.
5. The training run will be logged to Weights & Biases, and the trained model can be pushed to Hugging Face Hub.

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

## Project links

- Kaggle Notebook: [ML_OPS_Assignment](https://www.kaggle.com/code/vishveshrg25ait2130/ml-ops-1/notebook)
- Weights & Biases Dashboard: [W&B Project](https://wandb.ai/g25ait2130-indian-institute-of-technology-jodhpur/huggingface/overview)
- Hugging Face Model: [VishweshR/distilbert-goodreads-genres](https://huggingface.co/VishweshR/distilbert-goodreads-genres/tree/main)

## Notes

This repository is intended to support the assignment workflow and make the experiment easy to inspect. The main focus is on the pipeline setup: Kaggle training, W&B tracking, and public model hosting through Hugging Face.
