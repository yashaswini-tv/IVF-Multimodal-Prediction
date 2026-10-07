# IVF Multimodal Pregnancy Prediction

This repository contains the analysis code for the study:

**Incremental Predictive Value of Blastocyst Imaging Beyond Clinical and Semen Data for Pregnancy Following IVF-ET: A Multimodal Machine Learning Study**

## Study Aim

To evaluate whether blastocyst image information provides incremental predictive value beyond clinical and semen-related data for predicting pregnancy following IVF-ET.

## Dataset

Publicly available **Embryo dataset**, Mendeley Data, Version 1.

DOI: 10.17632/x5s3ky9cpv.1

The dataset contains 2,542 embryo records representing 1,415 unique patients, with paired blastocyst images and clinical/semen-related variables.

## Models

- Clinical model: Histogram-based Gradient Boosting
- Image model: EfficientNetB0
- Multimodal model: Late fusion of clinical and image predictions
- Evaluation performed using patient-level train, validation, and held-out test partitions

## Main Results

- Clinical model AUROC: **0.864**
- Image-only model AUROC: **0.546**
- Multimodal model AUROC: **0.865**
- Multimodal vs clinical AUROC difference: **0.0009**
- 95% bootstrap CI for the difference: **−0.0024 to 0.0044**

Blastocyst imaging provided no material incremental discrimination beyond the clinical and semen-related data in this dataset.

## Code

The Jupyter/Google Colab notebook contains the data preprocessing, patient-level partitioning, model development, evaluation, bootstrap analysis, permutation importance, and Grad-CAM analysis.

## License

The original dataset is distributed under the CC BY 4.0 license. Users should refer to the original Mendeley Data record for dataset licensing and attribution.
