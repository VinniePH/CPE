# Rhizome Rot Detection (CPE Thesis)

Two-stage pipeline kept as thesis core:
1. `Notebooks/01-data-preparation.ipynb`
2. `Notebooks/02-deit-train.ipynb`
3. `Notebooks/03-frcnn-train-2.ipynb`

## Run order
- Run notebook 01 first to generate `config.json`, `dataset/`, and `results/dataset_qa_summary.csv`.
- Run notebook 02 to train and evaluate DeiT classifier.
- Run notebook 03 to train and evaluate Faster R-CNN detector.

## Environments
- Primary: Kaggle GPU
- Secondary: Colab
- Also supports local paths through environment detection and `WORK_DIR`.

## Main outputs
- `results/deit_best_model/`, `deit_metrics.json/csv`, confusion matrix, training log
- `results/rcnn_best.pth`, `rcnn_metrics.json/csv`, sample predictions
