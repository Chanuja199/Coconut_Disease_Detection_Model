# AI-Based Coconut Disease Detection System

This repository contains the training pipeline and model report for an AI-based system designed to detect coconut diseases. The project utilizes a MobileNetV2 architecture trained to classify images into five distinct categories.

---

## Project Overview

The model identifies five specific classes: `bud_rot`, `healthy`, `leaf_spot`, `lethal_yellowing`, and `root_wilt`. The pipeline processes a dataset of 2185 images, applying extensive data augmentation to handle class imbalances, particularly for the underrepresented `bud_rot` class. The training process involved a frozen base phase followed by fine-tuning the top 40 layers of the MobileNetV2 base model.

## Performance Metrics

The final model achieved excellent performance, exceeding the initial target of 85% accuracy. 

| Metric | Score |
| :--- | :--- |
| **Test Accuracy** | 98.17% |
| **Weighted F1-Score** | 98.17% |


---

## Instructions for Running the Pipeline

1.  Go to **Runtime → Change runtime type → T4 GPU** before running.
2.  Run the notebook cells from **top to bottom** in order.
3.  When prompted in Cell 2, follow the link to authenticate Google Drive and paste the provided code.
4.  Update the `DATASET_PATH` variable in Cell 3 to match your specific Google Drive folder path.
5.  The final output files, including the TFLite models and `labels.txt`, will be saved automatically to your Drive.
