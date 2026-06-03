# Workflow

## Notebook sequence (must follow)
1. `Notebooks/01-data-preparation.ipynb`
2. `Notebooks/02-deit-train.ipynb`
3. `Notebooks/03-frcnn-train-2.ipynb`

## Stage 1: DeiT classifier
- Healthy vs Infected classification.

## Stage 2: Faster R-CNN detector
- Runs on infected images to localize diseased regions.

## Data-prep outputs
- `config.json`
- `dataset/train`, `dataset/valid`, `dataset/test` (+ COCO annotations)
- `results/dataset_qa_summary.csv`

## CPE deployment direction
- Save all trained outputs under `results/` for later ONNX export and TensorRT/Jetson Nano deployment.
