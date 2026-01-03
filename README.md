# Hi-C Forecasting with Temporal Attention

This repository implements a CNN-based Hi-C forecasting framework enhanced with temporal attention mechanisms. The project includes a baseline CNN, a single-head temporal attention model, and a multi-head temporal attention model, evaluated through a controlled ablation study.

## Models
- **Baseline CNN**: Encoder–decoder architecture without attention
- **Single-Head Temporal Attention**: Lightweight temporal self-attention over historical Hi-C matrices
- **Multi-Head Temporal Attention**: Four-head attention mechanism for diverse temporal dependency modeling

## Evaluation Metrics
- Mean Squared Error (MSE)
- Structural Similarity Index Measure (SSIM)
- Pearson Correlation Coefficient (PCC)

## Experiments
A systematic ablation study compares the baseline model with attention-based enhancements under identical training conditions.

## Usage
Train a model:
```bash
python train.py --model single --epochs 10
