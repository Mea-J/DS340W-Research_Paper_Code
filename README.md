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
