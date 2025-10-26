# Retail Feedback Classification Demo

## Overview
Python (HuggingFace/PyTorch) pipeline: Classifies Olist sentiment (translated columns), detects Kaputt defects, fuses for order flagging

## Metrics
| Component | Score | Notes |
|-----------|-------|-------|
| Text (BERT) | 0.74 Acc / 0.64 F1 | On translated reviews |
| Image (ResNet) | 1.00 Acc | On Kaputt crops |
| Joint Flagging | 0.76 Prec / 1.00 Rec | Fuses for auto-flags |

## Run in Colab
1. Open .ipynb in Colab.
2. Upload Olist CSV to Drive (/MyDrive/Assignment AI/).
3. Runtime > GPU.
4. Run all (~20 min).
5. Demo: predict_and_flag for alerts

Notebook: Download from repo

## Datasets
- Olist Translated: Kaggle.
- Kaputt Sample: kaputt-dataset.com.
