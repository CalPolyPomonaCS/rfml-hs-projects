# DroneRF Classic Machine Learning: Drone Detection

A 10-week summer research project for high school students.

**Title:** Evaluating Classic Machine Learning and Neural Network Models for Drone Radio-Frequency (RF) Detection.

**Research question:** To what extent can classic machine learning models and deep neural networks correctly classify drone types and activities using radio-frequency signals?

## How to start

1. Open [`DroneRF_Highschool_Project.ipynb`](DroneRF_Highschool_Project.ipynb) — or launch it directly in Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/username/repo/blob/main/DroneRF_Highschool_Project.ipynb)
2. Mount your Google Drive to load and save datasets and results.
3. Configure the `RAW_DIR` and `RESULTS_DIR` paths in Section 2.
4. Run a **small subset** of the dataset first before processing the full database.
5. Fill in the code structure and run cells from top to bottom.

Ask your instructor if stuck.

## 10-Week Plan

| Week | Focus | What students do |
|------|-------|------------------|
| 1 | Introduction | Learn what RF signals and drone detection are |
| 2 | Dataset setup | Download/extract data and inspect raw files |
| 3 | Signal preprocessing | Convert raw signals into frequency-domain features using FFT |
| 4 | Exploratory analysis | Plot raw signal snippets and spectrum charts |
| 5 | Labels and supervised learning | Build the aggregated `RF_Data.csv` with features and labels |
| 6 | Baseline ML models | Train and evaluate Gaussian Naive Bayes and Logistic Regression |
| 7 | Stronger ML models | Train Random Forest, SVM, K-Nearest Neighbors, and a DNN |
| 8 | Evaluation | Compare model accuracy, F1-score, and confusion matrices |
| 9 | Improvement | Test different subset sizes or multi-level classification targets |
| 10 | Final deliverable | Prepare poster, report, or presentation. Ethical discussion |

## Datasets

The project provides evaluations across three target classification configurations:
- **Level 1:** Drone vs. Background (Binary)
- **Level 2:** Bebop vs. AR vs. Phantom vs. Background (4 Classes)
- **Level 3:** Detailed multi-activity behaviors (10 Classes)

**Data Format:** Raw radio frequency signal slices stored in high (`H`) and low (`L`) frequencies extracted from `.rar` packages containing indexed timestamps.

## Key references

- Al-Sa'd et al., "RF-based drone detection and identification using deep learning frameworks": <https://ieeexplore.ieee.org/document/8350363>
- Scikit-Learn Supervised Learning Documentation: <https://scikit-learn.org/stable/supervised_learning.html>
- SciPy Signal Processing (`scipy.signal`): <https://docs.scipy.org/doc/scipy/reference/signal.html>
