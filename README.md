# MNIST Image Classification: MLP vs CNN

Comparison of a **fully connected neural network (MLP)** and a **convolutional neural network (CNN)** on the **MNIST** handwritten digit dataset (10 classes, 28×28 grayscale images).

**Course:** SWE012 — Deep Learning with Python  
**Author:** [Your Name]

---

## What this project does

- Trains an **MLP** baseline (flattened pixels → dense layers → softmax).
- Trains a **CNN** (convolution + pooling → dense → softmax).
- Keeps training conditions **as fair as possible**: same preprocessing, train/validation/test split, optimizer/loss, epochs, and batch size.
- Reports **validation curves**, **test accuracy/loss**, **confusion matrices**, and **sample misclassifications**.

---

## Results (update numbers if your run differs)

| Model | Test accuracy | Test loss |
|------|----------------|-----------|
| MLP  | ~0.9815        | ~0.0908   |
| CNN  | ~0.9904        | ~0.0399   |

**Takeaway:** The CNN typically achieves **higher accuracy** and **lower test loss** on MNIST, consistent with stronger **inductive bias** for spatial structure (local patterns + weight sharing).

---

## Repository contents

- `[notebook-name].ipynb` — full experiment (Kaggle/Jupyter notebook)

---

## How to run

### Option A — Kaggle (recommended)

1. Create a Kaggle Notebook with **GPU** (optional) and **Internet** enabled (if needed for `mnist.load_data()`).
2. Upload this notebook or copy its cells.
3. **Run all cells** (or **Save Version → Save & Run All** on Kaggle).

