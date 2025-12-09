# sst2-transformers
STATS 507 Final Project
# Comparing Pretrained Transformer Models on GLUE SST-2

This project compares several pretrained Transformer models from the Hugging Face Hub on the GLUE SST-2 sentiment classification task, focusing on both validation accuracy and training efficiency.
## How to Run
### Google Colab
1. Open `notebooks/sst2_transformer_comparison.ipynb` in Google Colab.
2. Set runtime to GPU (Runtime → Change runtime type → GPU).
3. Run all cells from top to bottom.

## Models and Training Setup
Models:
- `albert-base-v2`
- `bert-base-uncased`
- `distilbert-base-uncased`
- `roberta-base`

All models are fine-tuned on GLUE SST-2 with the same hyperparameters:
- 5 epochs
- batch size 16
- learning rate 2e-5
- evaluation metric: accuracy
## Results (Summary)

- `roberta-base` achieves the highest validation accuracy on SST-2 but has the longest training time.
- `distilbert-base-uncased` is the fastest to train but with slightly lower accuracy.
- `albert-base-v2` and `bert-base-uncased` lie in between in terms of both accuracy and runtime.

For detailed figures and analysis, see `STATS 507 Final Project.pdf`.
