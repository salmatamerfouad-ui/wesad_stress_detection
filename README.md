# wesad_stress_detection
83.4% stress detection accuracy from raw ECG, EDA, RESP &amp; TEMP signals; full ML pipeline with subject-independent validation on 15 real participants.


# WESAD Stress Detection Pipeline

This project builds a machine learning pipeline to detect stress from physiological signals recorded by a chest-worn wearable device. Using the WESAD dataset (15 subjects), we process four signals — ECG, EDA, RESP, and TEMP — through Butterworth filters, extract statistical features from 60-second sliding windows, and classify stress states using five classifiers evaluated with Leave-One-Subject-Out cross-validation. The best results were 83.4% accuracy for binary stress detection (LDA) and 70.6% for 3-class classification (AdaBoost).

## How to Run

Clone the repo, install requirements with `pip install -r requirements.txt`, then open and run all cells in `WESAD_Stress_Detection.ipynb`. The dataset downloads automatically via kagglehub.

## Requirements

numpy, pandas, matplotlib, seaborn, scipy, scikit-learn, kagglehub, jupyter

## Reference

Schmidt et al. (2018). Introducing WESAD, a Multimodal Dataset for Wearable Stress and Affect Detection. ACM ICMI 2018.
