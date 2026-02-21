# Intelligent Analytics 

## Project Overview
This project implements and evaluates **Multi-Layer Perceptron (MLP)**, **Radial Basis Function (RBF)**, and **Support Vector Machine (SVM)** networks for three applications:

1. **Reactive-Ion Plasma Etching Process Modeling**  
   Develop empirical models to predict etch characteristics of semiconductor fabrication processes (etch rate, uniformity, oxide, and photoresist selectivities) using experimental data from Himmel and May (1993).

2. **Pattern Recognition in Process Control Charts**  
   Detect process deviations in X-Charts based on the standard runs rules, automating the identification of out-of-control points using neural networks.

3. **Multi-Font Character Recognition**  
   Classify upper-case English letters from multiple fonts (Courier, New York, Chicago, Geneva, Times, Venice) using MLP, RBF, and SVM networks.

---

## Datasets

### 1. Plasma Etching Process
- **Source:** Himmel & May (1993), May, Huang & Spanos (1991)
- **Inputs (6):** Chamber Pressure, RF Power, Electrode Gap, CCl4 Flow, He Flow, O2 Flow  
- **Outputs (4):** Etch Rate, Etch Uniformity, Oxide Selectivity, Photoresist Selectivity  
- **Total Samples:** 53  
- **File:** `PlasmaEtchData.csv`  

### 2. Process Control Charts
- **Training Set:** 2500 patterns (1000 in-control, 250 per rule violation)  
- **Testing Set:** 250 patterns (100 in-control, 25 per rule violation)  
- **File Names:** `SPC-Training.dat`, `SPC-Testing.dat`  

### 3. Multi-Font Character Recognition
- **Fonts:** Courier, New York, Chicago, Geneva, Times, Venice  
- **Input Vector:** 14 features per pattern  
- **Output Vector:** 26 binary values (alphabet match)  
- **File Names:** `CharacterRecognition-Training.dat`, `CharacterRecognition-Testing.dat`  

---

## Project Objectives

- Train **MLP, RBF, and SVM networks** for regression and classification tasks.  
- Compare network performance in terms of prediction accuracy, generalization, and robustness.  
- Analyze empirical models for plasma etching to support semiconductor process optimization.  
- Automate process control chart evaluation to detect out-of-control conditions.  
- Perform multi-font character recognition with neural network models.  

---

## Methodology

1. **Data Preprocessing:** Normalization/scaling, train-test split.  
2. **Network Design:**
   - **MLP:** Feedforward network with hidden layers, trained using backpropagation.  
   - **RBF:** Radial basis neurons for nonlinear mapping.  
   - **SVM:** Kernel-based support vector regression/classification.  
3. **Training & Validation:** Cross-validation and hyperparameter tuning.  
4. **Evaluation:**  
   - Regression metrics: MSE, R²  
   - Classification metrics: Accuracy, Confusion Matrix, F1-score  
   - Comparative analysis of MLP, RBF, and SVM performance  

---

## Usage

1. Clone the repository
