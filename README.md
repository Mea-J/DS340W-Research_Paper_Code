# DS340W-Research_Paper_Code
A repo that holds the code for my research papers in DS340W

# Parent Paper 1: A hybrid framework for heart disease prediction using classical and quantum-inspired machine learning techniques
## Paper Pipeline (CGA-CPSO-CSVM):
- Data description: combined UCI heart-disease dataset (918 unique rows, 11 features), 80:20 train/test split
- - 734 train / 184 test.
- CGA: genetic-algorithm wrapper feature selection (roulette-wheel selection, one-point crossover, bit-flip mutation)
- - paper reports 9 of 11 features selected (~19% reduction).
- CPSO: particle swarm optimization of the SVM hyperparameters (C, gamma).
- CSVM: final RBF-kernel SVM trained on the selected features and tuned hyperparameters, evaluated with Accuracy, Precision, Sensitivity (Recall), Specificity, F1, MCC, ROC-AUC, LR+, LR-, and DOR
- Tenfold cross-validation of the final model, as described in the paper's "K-fold cross-validation" section.


# Parent Paper 2: Advancing Neurological Disease Prediction through Machine Learning Techniques
- Data description: Open-sourced medical datasets (not actually listed)
- - Uses separated EEG, MRI, and clinical data and a combined dataset of both.
  - was split 80/20
- Evaluates predictive performance of machine learning techniques three conditions: Parkinson's disease, Epilepsy, and Multiple Sclerosis.
- Models Used:
- - SVM
  - KNN
  - Gradient Boosting (best performance metrics)
  - Random Forest
  - SVM-KNN hybrid model
- Feature Engineering:
- - Wavelet Transforms
  - PCA transformsP
 

# Parent Paper 3: High Performance Heart Disease Prediction Through Soft Voting Ensemble: An Interpretable Machine Learning Approach
- Data: Heart Disease for Health Research (Kaggle)
- - 10,000 entries and 21 columns
  - Preprocessing: imbalance issue, applied random oversampling
- Evaluates the predictive performance and interpretability of a soft voting ensemble classifier for heart disease prediction
- Hyperparameters: Grid search
- Proposed Model: Combination
- - SVM
  - MLP
  - Extra Trees
-Evaluation: The soft voting ensemble method was compared to the best performing individual classifiers by accuracy, precision, recall, F1-score, and ROC.


# My Implementation
- Goal: Evaluate the generalizability and Interpretability of Hybrid Machine Learning Models for Disease Prediction
- Research Questions:
- - Do GA-PSO optimized models maintain their performance when evaluated on an independent dataset?
  - Do the most important predictive features remain consistent across different datasets?
  - Does combining GA and PSO actually improve generalizability compared with using either technique independently?
- Data: Combined datasets, along with external validation dataset
- Methods: I will apply a genetic algorithm for feature selection and particle swarm optimization for hyperparamter tuning to an ensemble machine learning model. Then for interpretability validation I will use SHAP. To evaluate the models performance, I will use a logistic regression model both with and without the optimization steps.
  - Ensemble Method: Support Vector Machine-Random Forest-Multilayer Perceptron
- Evaluation Metrics:
- - F1
  - Accuracy
  - Precision 
  - Recall
  - ROC-AUC
  - Consistency of feature importance
  


