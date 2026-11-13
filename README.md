# Road Damage Detection and Severity-Aware Maintenance Prioritization

A deep learning-based road damage detection system using **YOLOv8n** and the **RDD2022 dataset**. The project detects road cracks and potholes, estimates their severity, and assigns maintenance priorities.

## Features

- Detects four types of road damage.
- Estimates damage severity using bounding-box area.
- Assigns maintenance priorities based on damage type and severity.
- Compares SGD and AdamW optimizers.
- Generates detection results and maintenance reports.

## Damage Categories

| Class | Damage Type        |
| ----- | ------------------ |
| D00   | Longitudinal Crack |
| D10   | Transverse Crack   |
| D20   | Alligator Crack    |
| D40   | Pothole            |

## Tech Stack

- Python
- YOLOv8n
- PyTorch
- Ultralytics
- OpenCV
- NumPy, Pandas, Matplotlib

## Model Performance

The final model was trained for 40 epochs using SGD and selected based on validation performance.

| Metric    | Test Result |
| --------- | ----------: |
| Precision |      60.94% |
| Recall    |      50.72% |
| mAP50     |      53.98% |
| mAP50-95  |      26.99% |

**Selected Model:** YOLOv8n-SGD

## Project Workflow

```text
RDD2022 Dataset
       ↓
Data Preprocessing
       ↓
YOLOv8n Training
       ↓
Optimizer Comparison
       ↓
Model Evaluation
       ↓
Damage Detection
       ↓
Severity Assessment
       ↓
Maintenance Prioritization
```

## Notebooks

| Notebook | Description                           |
| -------- | ------------------------------------- |
| 01       | Dataset Verification                  |
| 02       | Baseline YOLOv8n Training             |
| 03       | Optimizer Comparison                  |
| 04       | Validation Evaluation                 |
| 05       | Final Test Evaluation                 |
| 06       | Severity & Maintenance Prioritization |
| 07       | Final 40-Epoch Experiment             |

## Dataset

The project uses the RDD2022 Road Damage Dataset.

## Future Scope

- Campus-specific road damage detection.
- Improved severity estimation.
- GPS-based damage mapping.
- Real-time deployment on edge devices.

## Contributors

- Amrit Kumar
- Dikshant Bhanarkar
- Chaitanya Pahade
- Aryan Shambharkar
