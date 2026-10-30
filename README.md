# Temporal Morphing Network (TMN) for Human Activity Recognition

Code for the paper *Temporal Morphing Network for HAR Using Learned Deformation Fields*.

TMN learns a per-sample temporal deformation field over wearable-sensor windows, followed by SE channel attention and a transformer encoder.

| Dataset | Classes | Accuracy |
|---|---|---|
| WISDM v2 | 18 | 94.23% |
| UCI-HAR | 6 | 91.92% |

## Contents

- `TMN_Kaggle_Full.ipynb` - full pipeline (Kaggle, with auto-checkpointing): TMN training on WISDM, ablations B-F (no morph field, no consistency loss, no SE attention, mean pooling, accelerometer only), ablation chart, UCI-HAR cross-dataset evaluation, final summary.
- `TMN_Kaggle_Full_executed.ipynb` - the same pipeline with the saved outputs from a Kaggle run.

## Running

Open `TMN_Kaggle_Full.ipynb` on Kaggle (GPU), attach the WISDM v2 dataset, and run all cells. Each step saves a checkpoint zip so an interrupted run can resume.
