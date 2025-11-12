# Driver Health Monitoring: Facial Emotion Recognition & Heart Rate Analysis

## Overview

This project implements a system for real-time driver health and safety monitoring by combining two key physiological data streams: **Facial Emotion Recognition (FER)** and **Electrocardiogram (ECG)** signal analysis for Heart Rate (BPM) extraction.

The primary objective is to enhance the efficiency of in-vehicle health monitoring by moving beyond traditional systems. By fusing emotional state and cardiac data, the system aims to accurately and proactively identify high-stress levels or immediate health threats in a driver, enabling actionable safety recommendations.

---

## Key Features

* **Facial Emotion Recognition (FER):** Identifies and classifies the driver's current emotional state (e.g., 'tensed', 'calm', 'happy') from image inputs.
* **Heart Rate (BPM) Extraction:** Processes raw ECG signals to accurately calculate the driver's Beats Per Minute (BPM), likely using QRS complex detection via cross-correlation with a filter.
* **Combined Threat Assessment:** Fuses the classified emotional state and the calculated BPM value to generate a comprehensive threat score or warning level.
* **Actionable Safety Recommendations:** Provides clear output, such as "Threat = Yes, Recommend immediate dismissal from driving," based on the combined physiological indicators.

---

## Dependencies and Setup

This project is implemented in a Jupyter Notebook and requires several standard Python scientific computing libraries.

### Prerequisites

To run this notebook, ensure you have Python installed, and then install the required libraries:

```bash
pip install numpy pandas matplotlib scikit-learn
# Note: Additional libraries for deep learning (TensorFlow/Keras or PyTorch) 
# and image processing (OpenCV or PIL) are likely required for the FER component.
