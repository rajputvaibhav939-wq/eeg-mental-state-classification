# EEG-Based Mental State Classification Using Machine Learning

## Overview
This project explores the classification of mental states using EEG band power features. EEG signals were preprocessed in MATLAB to extract frequency band powers corresponding to Delta, Alpha, Beta, and Gamma waves. The processed dataset was then used in Python to train and evaluate several machine learning classifiers.

The objective of this project is to compare different machine learning models and analyze their performance in classifying EEG-based mental states.

---

## Dataset
The dataset consists of EEG band power features extracted from brain signals. Each sample contains four features:

- **Delta** – Low frequency brain activity  
- **Alpha** – Relaxed mental state  
- **Beta** – Active thinking and focus  
- **Gamma** – High-level cognitive processing  

Each sample is labeled with a target class representing the mental state.

Dataset size:

- **Samples:** 10  
- **Features:** 4  
- **Classes:** 2  

---

## Preprocessing
Raw EEG signals were preprocessed using MATLAB before being used in Python. The preprocessing included:

- Noise filtering  
- Artifact removal  
- Extraction of frequency band powers:
  - Delta
  - Alpha
  - Beta
  - Gamma

The extracted band power values were saved in a `.mat` file and imported into Python for machine learning experiments.

---

## Machine Learning Models
The following classifiers were implemented and evaluated:

- Logistic Regression  
- Support Vector Machine (SVM)  
- K-Nearest Neighbors (KNN)  
- Random Forest  

Model performance was evaluated using **5-fold cross-validation**.

---

## Results

| Model | Mean Accuracy |
|------|---------------|
| Logistic Regression | 0.5 |
| Support Vector Machine (SVM) | 0.4 |
| KNN | 0.5 |
| Random Forest | 0.8 |

Random Forest achieved the best performance among the evaluated models.

---

## Key Observations
- Random Forest performed better due to its ability to capture nonlinear relationships in EEG features.
- Linear models such as Logistic Regression showed moderate performance.
- The small dataset size caused fluctuations in cross-validation accuracy.

---

## Technologies Used
- Python  
- NumPy  
- Pandas  
- SciPy  
- Scikit-learn  
- Matplotlib  
- Jupyter Notebook  

---

## Project Structure

```
eeg-mental-state-classification/
│
├── data/
│   └── EEG_bandpower_dataset.mat
│
├── notebooks/
│   └── eeg_classification.ipynb
│
├── report/
│   └── EEG_classification_report.pdf
│
├── results/
│   └── model_comparison.png
│
├── requirements.txt
│
└── README.md
```

---

## Limitations
- The dataset is very small (10 samples).
- Results may not generalize to larger EEG datasets.
- More data would improve model reliability.

---

## Future Work
Possible improvements for this project include:

- Using larger EEG datasets
- Testing deep learning models
- Exploring additional EEG features
- Building real-time EEG classification systems

---

## Author
AI & Robotics Engineering Student  
Machine Learning Enthusiast

---

## License
This project is intended for educational and research purposes.
