# EMG-Based Hand Gesture Classification
## Overview
Hand rehabilitation is a critical process for patients recovering from neurological conditions such as stroke. One of the main challenges is detecting the patient's intended movement accurately and in real time.

This project aims to analyze EMG signals collected from forearm muscles and build machine learning models capable of predicting whether the user intends to open or close their hand.

Artificial Intelligence (AI) enables the analysis of complex biosignals like EMG to uncover patterns that are difficult to detect using traditional methods. By leveraging machine learning algorithms, AI can:

Identify muscle activation patterns
Predict hand movement intention with high accuracy
Enable real-time decision making
Support rehabilitation systems with intelligent assistance

AI-driven models act as supportive systems that enhance rehabilitation efficiency rather than replacing clinical decisions.

## Dataset
EMG data collected from forearm muscles, focusing on two main channels:
- Flexor Digitorum
- Extensor Digitorum

Signals are processed and transformed into features representing muscle activity for classification tasks.

## Methodology
Data Preprocessing

- Handling signal noise using filtering techniques
- Bandpass filtering (20–450 Hz)
- Notch filtering (50 Hz)
- Signal rectification
- Envelope extraction (smoothing)

## Segmentation
Applying sliding window technique to convert continuous signals into samples

## Feature Extraction
- Extracted features from each EMG channel:
- Mean Absolute Value (MAV)
- Root Mean Square (RMS)
- Variance
- Waveform Length (WL)
- Zero Crossing (ZC)
- Slope Sign Change (SSC)
- Willison Amplitude (WAMP)

Total features per sample: 14

## Models Implemented
- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (RBF)
- K-Nearest Neighbors (KNN)
- XGBoost
- Soft Voting Ensemble

## Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Results
The models achieved high performance with accuracy exceeding 90 percent.

Best performing models:
- Support Vector Machine (RBF)
- Soft Voting Ensemble

Other models such as Logistic Regression and Random Forest also showed strong performance with faster inference time.

## Key Highlights
- Implemented multiple classification algorithms
- Compared model performance
- Achieved over 90 percent accuracy
- Built a complete signal processing and ML pipeline
- Designed for real-time rehabilitation applications
