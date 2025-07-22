# COPD Detection using Respiratory Audio Signals

This project presents a machine learning pipeline to detect **Chronic Obstructive Pulmonary Disease (COPD)** from respiratory sound recordings. Using handcrafted acoustic features and ensemble learning models, the system is optimized for potential low-cost screening in clinical or remote environments.

---

## 📁 Project Structure

- `COPD_Detection_Detailed_Exploration.ipynb`  
  Contains full exploratory work, data cleaning, feature extraction using MFCC, training and evaluation of multiple models (SVM, ANN, CNN, Random Forest), confusion matrices, ROC curves, and accuracy metrics.

- `COPD_Detection_Final_Results.ipynb`  
  A clean, result-focused notebook containing the streamlined version of the model pipeline, showcasing only the key results for both balanced and imbalanced datasets.

---

## 📌 Dataset Used

- **Source:** [Kaggle - Respiratory Sound Database](https://www.kaggle.com/datasets)  
- **Note:** Dataset is not included in this repository due to licensing. Please download it directly from Kaggle and place it in your Google Drive before running the notebooks.

---

## 🧪 Workflow Summary

### 1️⃣ Balanced Dataset
- Subset of the dataset selected with **26 COPD** and **26 non-COPD** samples.
- Applied MFCC (Mel-Frequency Cepstral Coefficients) feature extraction.
- Trained on multiple models including:
  - Random Forest (RF)
  - Support Vector Machine (SVM)
  - Artificial Neural Network (ANN)
  - Convolutional Neural Network (CNN)
- **Best Accuracy:**  
  ✅ Random Forest achieved **96.2% accuracy** on the balanced dataset.

---

### 2️⃣ Full Dataset (Imbalanced)
- Expanded dataset to include **64 COPD** and **62 non-COPD** samples (some versions may vary slightly).
- Noticed **class imbalance**, which affected performance.
- Applied **SMOTE (Synthetic Minority Oversampling Technique)** to balance the data.
- Used **5-Fold Cross-Validation** for reliable evaluation.
- **Accuracy Across Models:**  
  ✅ Achieved **~88–89% accuracy** consistently across RF, SVM, ANN after SMOTE and CV.

---

## 🧠 Techniques Used

- **MFCC**: Extracted key acoustic features from respiratory audio signals.
- **SMOTE**: Balanced the dataset during training by generating synthetic minority class examples.
- **Ensemble & Deep Learning Models**: Compared performance of Random Forest, SVM, ANN, CNN.
- **Evaluation Metrics**: Accuracy, Confusion Matrix, ROC Curve.

---

## 🚀 How to Run

1. Open either notebook in **Google Colab**.
2. Mount your **Google Drive**.
3. Make sure the dataset is present in the expected path inside Drive.
4. Run all cells to train and evaluate the models.

---

## 📈 Results Snapshot

| Dataset        | Method         | Accuracy |
|----------------|----------------|----------|
| Balanced (26/26) | Random Forest   | 96.2%    |
| Imbalanced (64/62) + SMOTE | RF/SVM/ANN | ~88–89% |

---

## 📎 Acknowledgments

- Kaggle Respiratory Sound Dataset
- SRM University Faculty (Advisor: Dr. Sudestna Nahak)
- Submitted to: IIT Delhi Conference (Awaiting results)

---

## 📫 Contact

**Lakshya Agrawal**  
Email: [agrawal2004lakshya@gmail.com]  
GitHub: [github.com/la2951](https://github.com/la2951)

