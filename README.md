# ECG Classification for Remote Health Monitoring

## Overview

This repository contains the implementation of my capstone project focused on ECG signal classification to improve **remote health monitoring**, addressing challenges like **class imbalance** and **computational efficiency**. The project leverages machine learning techniques like **Temporal Convolutional Networks (TCN)** and **XGBoost** to classify heart conditions from the **ECG5000** dataset.

> Achieved a **macro F1 score of 0.6546 (TCN)** and **0.5785 (XGBoost)** using innovative data augmentation, feature engineering, and interpretable model design.

> Achieved the highest score (95/100) among 20 participants for this project

This work showcases skills in data analysis, preprocessing, machine learning, and model optimization—ideal for roles in **Data Science**, **Data Engineering**, **ETL Development**, and **ML Engineering**.

---

## 🚩 Project Highlights

### 🔧 Problem Solved
Addressed **extreme class imbalance** in ECG5000 (e.g., class 4: 11 samples vs. class 0: 781) to enable accurate detection of **rare heart conditions**, crucial for remote diagnostics.

### Methodologies

- **Method A (TCN):**  
  Implemented a lightweight TCN with data augmentation (odd-even sampling, amplitude shifting).  
  - **Macro F1:** 0.6546  
  - **Accuracy:** 0.9206  

- **Method B (XGBoost):**  
  Developed interpretable features (e.g., `permutation_entropy`, `simple_angle`)  
  - **Macro F1:** 0.5785 (vs. baseline 0.4109, a **+41.2% improvement**)  
  - **Accuracy:** 0.8767  

- **Method C (KNN):**  
  Baseline method with limited ability to handle imbalance.  
  - **Macro F1:** 0.5681  
  - **Accuracy:** 0.9220  

### 💡 Key Innovations

- Novel **odd-even sampling** and **amplitude shifting** to address minority class underrepresentation.
- Custom feature engineering (`simple_angle`, `maxMinMore`) for interpretable ECG analysis.
- Post-processing override (`overridePredict`) to boost minority class predictions.

> 💡 Impact: Models designed for **low-power devices**, enabling deployment in **rural healthcare** scenarios.

---

## 📈 Relevance & Skills Demonstrated

- In-depth evaluation using **macro F1**, precision, recall, AUROC, and class-specific metrics.
- Robust preprocessing: standardization, noise injection, and imbalance mitigation.
- Efficient workflows to **extract, transform, and augment ECG signals**.
- Engineered and optimized **TCN** and **XGBoost** with **hyperparameter tuning** and custom overrides.

---

## 📊 Key Results

| Method       | Macro F1 | Accuracy | Strengths                                |
|--------------|----------|----------|------------------------------------------|
| **TCN**      | 0.6546   | 0.9206   | Superior minority class performance      |
| **XGBoost**  | 0.5785   | 0.8767   | Interpretable, feature-driven approach   |
| **KNN**      | 0.5681   | 0.9220   | Simplicity, strong on majority classes   |



---

## ⚙️ Technical Skills

- **Languages:** Python  
- **Libraries:** TensorFlow, XGBoost, Scikit-learn, NumPy, Pandas, Matplotlib  
- **Techniques:** Data augmentation, feature engineering, hyperparameter tuning  
- **Concepts:** Imbalanced classification, deep learning (TCN), ensemble methods (XGBoost), interpretability

---

## Future Improvements

- **Hybrid Models:** Combine TCN and XGBoost for improved performance and interpretability.
- **Generative Augmentation:** Use GANs to create synthetic minority class ECG signals.
- **Edge Deployment:** Optimize models for wearables using quantization and pruning.
- **Explainability:** Integrate SHAP for clinical model transparency.

---

## About Me

I’m a data enthusiast passionate about building **scalable and interpretable** ML solutions for real-world problems. This project reflects my ability to handle complex datasets, engineer pipelines, and optimize models for **both performance and practicality**.

📌 I'm actively seeking opportunities in:
- Data Analysis  
- Data Engineering  
- ETL Development  
- Machine Learning Engineering

---

## Acknowledgments

This project was inspired by:

- **Ismail et al. (2023)** – TCN-based ECG classification  
- **Rajpal et al. (2020)** – Interpretable ECG via XGBoost  
- **Biloborodova et al. (2022)** – Hybrid feature engineering for ECG  

📚 *For detailed citations, see project documentation.*

---

⭐ **Star this repository** if you found it helpful! Contributions and feedback are welcome.
