# Flight Delay Prediction using Decision Tree Model

## Overview

This project aims to analyze and predict flight delays using machine learning, specifically a Decision Tree model. The notebook was developed during the **AI Bootcamp - June 2024 Cohort**. It includes the necessary steps for preprocessing the dataset, applying machine learning algorithms, and evaluating model performance.

## Contents

### 1. **Libraries Used**

The following Python libraries are utilized in this notebook:

- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Matplotlib** & **Seaborn**: Data visualization
- **Scikit-learn (sklearn)**:
    - `StandardScaler`: For feature scaling
    - `PCA`: Principal Component Analysis for dimensionality reduction
    - `LabelEncoder`: For encoding categorical variables
    - `KMeans`: For clustering (optional exploration)
    - `DecisionTreeClassifier`: For the Decision Tree model

### 2. **Installation of Additional Packages**
If needed, the following packages are required and can be installed via pip:
- `graphviz`: For visualizing decision trees
- `pydotplus`: For additional tree visualization functionality

Install commands:
```bash
!pip install graphviz
!pip install pydotplus
```

### 3. **Notebook Workflow**

The notebook follows this workflow:
1. **Data Loading and Exploration**: Import the dataset, explore its structure, and perform initial data cleaning.
2. **Preprocessing**:
    - Feature scaling using `StandardScaler`.
    - Label encoding for categorical features.
    - Optional: PCA for dimensionality reduction.
3. **Model Building**: A Decision Tree Classifier is used to predict flight delays.
4. **Model Evaluation**: Evaluate the model using accuracy, confusion matrix, and other relevant metrics.
5. **Visualization**: Visualize the decision tree using `graphviz` and `pydotplus`.

### 4. **Usage**

1. Clone the repository or download the Jupyter notebook.
2. Install the necessary dependencies listed in the notebook.
3. Run each cell to preprocess the data, build the model, and visualize the results.
4. Modify the notebook to explore different algorithms or improve the model.

### 5. **Data**

The dataset used for this project contains flight details and delays. The columns are documented in the accompanying project documentation, which includes:
- Flight number, airline, origin, destination
- Scheduled and actual times
