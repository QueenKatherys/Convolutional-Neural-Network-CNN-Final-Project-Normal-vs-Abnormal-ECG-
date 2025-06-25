# 🫀 BIOST 546A – Final Project  
### Machine Learning for Biomedical and Public Health Big Data  
**University of Washington – Spring 2024**  
**Author:** Kathleen Ashbaker | 📧 kashba@uw.edu  

---

## 🧠 Project Title  
**K-Fold Cross-Validation Enhanced Convolutional Neural Networks for Robust Detection of Abnormal ECG Signals**

---

## 📘 Overview  
This repository contains materials from the final project for BIOST 546A, which focused on applying deep learning techniques to real-world biomedical data. Specifically, this project developed and evaluated a **Convolutional Neural Network (CNN)** for classifying **ECG signals** as either *normal* or *abnormal*. To ensure generalizability and robustness, the model incorporates **k-fold cross-validation** and handles **class imbalance** through class weighting.

---

## 📁 Repository Contents

| File Name                                         | Description                                                               |
|--------------------------------------------------|---------------------------------------------------------------------------|
| `Final Term Paper by Kathleen Ashbaker.pdf`      | Full report detailing methodology, results, and discussion                |
| `Final-Project-Final-Submission-CNN-MODEL.pdf`   | PDF version of R Markdown output with code, plots, and model metrics      |
| `Final Project Final Submission CNN MODEL.Rmd`   | R Markdown source code for the CNN implementation and visualization       |

---

## 🔍 Key Highlights

- **Data Source**: PTB Diagnostic ECG Database (PhysioNet)
- **Input Shape**: ECG heartbeats with 187 timepoints
- **Labels**: Binary classification (0 = Normal, 1 = Abnormal)
- **Frameworks Used**:
  - R with `keras`, `reticulate`, `tensorflow`
  - Python backend (via `reticulate`)
- **Model Architecture**:
  - 1D Convolutional Layer → Max Pooling → Dense Layers
  - Binary output with sigmoid activation
- **Techniques**:
  - Class weighting to address imbalance
  - K-fold cross-validation (k=5)
  - Evaluation via accuracy, loss, and visual learning curves

---

## 📊 Results

| Metric                    | Value               |
|---------------------------|---------------------|
| Final Training Accuracy   | 100.0%              |
| Final Validation Accuracy | 98.86%              |
| Average K-Fold Accuracy   | 98.49%              |
| Training Loss             | 0.0012              |
| Validation Loss           | 0.0429              |

> These metrics indicate strong generalization and effective handling of real-world diagnostic data.

---

## 🛠 Software & Libraries

- R 4.3.0  
- Python 3.9.13 (via `reticulate`)  
- TensorFlow 2.13  
- Keras 2.13.1  
- Packages: `ggplot2`, `keras`, `tensorflow`, `reticulate`

---

## 🧪 Reproducibility

The code is fully reproducible in R using an RStudio environment configured with Python support. All data matrices (`X_train`, `X_test`, `y_train`) were preprocessed, scaled, and reshaped for compatibility with CNN input requirements.

Note: Data files such as `ptb.Rdata` are not included in this repository due to size constraints but are available upon request.

---

## 📬 Contact

For access to the dataset or further discussion:

**Kathleen Ashbaker**  
📧 Email: [kashba@uw.edu](mailto:kashba@uw.edu)  
🔗 GitHub: [@QueenKatherys](https://github.com/QueenKatherys)

---

## 📄 Citation

Ashbaker K. *K-Fold Cross-Validation Enhanced Convolutional Neural Networks for Robust Detection of Abnormal ECG Signals*. BIOST 546A Final Project. University of Washington, Spring 2024.

---

## 📘 License

This project is intended for academic, instructional, and scholarly demonstration purposes only. Attribution is required when referencing or adapting materials.

