# Explainable Anomaly Detection for Industrial Predictive Maintenance using LSTM Autoencoders

This master project focuses on detecting anomalies in industrial systems using LSTM Autoencoders and explainable AI techniques.

## Technologies Used
- Python
- TensorFlow / Keras
- SHAP
- NumPy
- Pandas
- Matplotlib

## Objective
The goal of this project is to improve predictive maintenance by identifying abnormal patterns in industrial sensor data.
## 🧪 Methodology

The project follows a structured approach to ensure reliable anomaly detection and explainability:

### 1. Data Pre-processing
* **Dataset:** NASA C-MAPSS (Commercial Modular Aero-Propulsion System Simulation) Turbofan Engine Degradation Dataset.
* **Feature Engineering:** Normalization, Handling sensor noise, and Windowing for time-series compatibility.

### 2. Proposed Architecture (LSTM Autoencoder)
* **Encoder:** Captures temporal dependencies and compresses multi-sensor input data into a low-dimensional latent space.
* **Decoder:** Attempts to reconstruct the original input from the latent representation.
* **Anomaly Scoring:** Anomalies are detected based on the **Reconstruction Error** (the difference between the original and reconstructed input).



### 3. Explainability with SHAP
* Integrating **SHAP (SHapley Additive exPlanations)** to interpret the model's output.
* This allows identifying exactly which sensor (e.g., Temperature, Pressure, Fan speed) contributed most to a detected anomaly, making the system "Explainable."
