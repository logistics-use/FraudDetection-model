This project implements a hybrid classical-quantum approach for financial fraud detection using synthetic transaction data. It combines classical machine learning techniques with quantum-inspired models (Variational Quantum Classifier and Quantum Support Vector Machine) to identify fraudulent transactions with higher accuracy.

The system also demonstrates quantum angle encoding, quantum feature maps, and ensemble techniques for hybrid quantum-classical models, along with visualizations such as quantum circuits, Bloch spheres, ROC curves, and precision-recall curves.

Key Features

Synthetic Dataset Generation: Creates a complex, multi-featured dataset simulating normal and fraudulent transactions with realistic patterns including:

Transaction amounts, hours, locations, merchants

Behavioral features

Fraud types (large purchase, micro transactions, behavioral anomalies)

Data Preprocessing & Encoding:

Standard scaling and optional PCA for dimensionality reduction

Quantum Angle Encoding of features into qubit rotations

Hybrid Quantum-Classical Models:

Variational Quantum Classifier (VQC) with feature map + ansatz circuits

Quantum Support Vector Machine (QSVM) with quantum kernel fallback

Quantum Ensemble combining multiple quantum models with weighted averaging

Classical Baseline: RBF kernel SVM for performance comparison

Evaluation & Visualization:

Confusion matrices, ROC curves, Precision-Recall curves

Case analysis of normal vs fraud samples

Quantum circuit diagrams and Bloch sphere visualizations

Libraries & Tools

Classical ML: numpy, pandas, scikit-learn, matplotlib, seaborn

Quantum Computing: qiskit, qiskit-aer, qiskit.visualization

Visualization: Matplotlib, Seaborn, Qiskit’s circuit drawing tools

Workflow

Generate Dataset: create_advanced_dataset() simulates transaction records with normal and fraud cases.

Preprocess & Encode: QuantumAngleEncoder transforms features into qubit angles suitable for quantum circuits.

Train Models:

Baseline SVM for classical comparison

Advanced VQC and QSVM quantum models

Combine models in QuantumEnsemble for improved prediction

Predict & Evaluate: Evaluate using accuracy, precision, recall, F1-score, ROC & PR curves.

Visualize Results: Confusion matrices, quantum circuits, Bloch spheres, ROC & PR curves.

Case Analysis: Compare model predictions on selected fraud and normal transactions
