# MFIL-Net + VRN: Human Disease Prediction using Vital Signs

## 📖 Overview
This project proposes a novel **MFIL-Net + VRN (Medical Features Interaction Learning + Vital Resonance Network)** framework for **multi-label disease prediction** using vital physiological signals.  
The model integrates **IoMT-based time-series data** (Heart Rate, Blood Pressure, Body Temperature, and Oxygen Saturation) to detect early-stage diseases with high accuracy, interpretability, and robustness.  

Unlike traditional ML methods, MFIL-Net + VRN captures **harmonic interactions between vital signs**, improving diagnostic precision and minimizing false positives.

---

## ⚙️ Features
- Multi-label disease prediction using **4 primary vitals**: HR, BP, Temp, SpO₂.
- **Rule-based labeling** using clinical thresholds.
- **MFIL-Net**: Dense neural architecture to learn multi-feature interactions.
- **Vital Resonance Network (VRN)**: Captures inter-vital coherence & harmonic dynamics.
- **Noise injection & regularization** for robustness against overfitting.
- **Comparative benchmarking** against classical ML models:
  - Random Forest
  - Logistic Regression
  - Support Vector Machine
  - XGBoost
  - KNN
  - Decision Tree

---

## 📊 Dataset
- Vital sign records in CSV format.
- 4 main inputs: HR, BP, Temp, SpO₂.
- 7 engineered features derived from domain knowledge.
- Labels: **10 disease conditions** generated via medical rule-based logic.

---

## 🏗️ Model Architecture
- **Input Layer**: 11 features (4 vitals + 7 engineered).
- **Hidden Layers**:
  - Dense (128 → 64 → 32 neurons) with ReLU.
  - Batch Normalization + Dropout (p=0.3).
  - L2 Regularization (λ=0.01).
- **VRN Module**:
  - Gaussian Noise injection to simulate biological variability.
- **Output Layer**:
  - 10 Sigmoid neurons (multi-label classification).

---

## 🚀 Implementation
- Framework: **TensorFlow / Keras**
- Loss Function: **Binary Cross-Entropy**
- Optimizer: **Adam**
- Metrics: Accuracy, Precision, Recall, F1-Score, Specificity, ROC-AUC, PR-AUC.

---

## 📈 Results
- **MFIL-Net + VRN** achieved:
  - ~97% Accuracy & Precision
  - ~78% Recall
  - ~86% F1-Score
  - 100% Specificity
  - ~100% ROC-AUC and ~97% PR-AUC
- Outperformed all baseline models in both accuracy and clinical reliability.

---

## 🔮 Future Work
- Integration with **Electronic Health Records (EHRs)**.
- Edge-AI deployment on low-power IoT devices.
- Multi-modal diagnostic fusion (ECG, PPG, Lab data).
- Adaptive learning for unseen conditions.
- Clinical validation through large-scale trials.

---

## 👨‍💻 Authors
- **Anmol Rai**, Apex Institute of Technology, Chandigarh University  
- **Tati Vinay**, U.V. Patel College of Engineering, Ganpat University  
- **Jyoti Srivastava**, Faculty of Engineering and Technology, Ganpat University  

---

## 📜 License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
