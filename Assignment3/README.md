# Assignment 3: Regression, Validation & PCA

## Objective
The goal of this assignment is to practice regression techniques (Multiple Linear Regression), validation strategies (K-Fold and train/validation/test splits), optimization with Gradient Descent, and dimensionality reduction using PCA.

---

## Tasks

### Q1: K-Fold Cross Validation (Multiple Linear Regression with Least Squares)
Dataset: [USA House Price Prediction](https://drive.google.com/file/d/1O_NwpJT-8xGfU_-3llUl2sgPu0xllOrX/view?usp=sharing)  

Steps:
1. Separate dataset into input features (all columns except *price*) and output variable (*price*).  
2. Scale the input features.  
3. Divide the dataset into 5 folds.  
4. Perform 5 iterations:
   - Use one fold as test set, remaining folds as training set.  
   - Compute β (coefficients), predicted values, and R² score.  
5. Select the β with maximum R² score and retrain using 70% of data, test on 30%.  

---

### Q2: Validation Set (Gradient Descent Optimization)
Dataset: same as Q1.  

Steps:
1. Split dataset into: Training (56%), Validation (14%), Test (30%).  
2. Try different learning rates {0.001, 0.01, 0.1, 1}.  
3. Train using Gradient Descent for 1000 iterations.  
4. Record regression coefficients for each learning rate.  
5. Compute R² score for Validation and Test sets.  
6. Select the best coefficients based on performance.  

---

### Q3: Preprocessing & Multiple Linear Regression with PCA
Dataset: [Car Price Prediction (UCI Auto Imports Dataset)](https://archive.ics.uci.edu/ml/machine-learning-databases/autos/imports-85.data)  

Steps:
1. Load dataset with provided column names and replace `?` with NaN.  
2. Handle missing values using central tendency imputation (drop rows with NaN in *price*).  
3. Convert categorical values:
   - `num_doors`, `num_cylinders`: words → numbers.  
   - `body_style`, `drive_wheels`: dummy encoding.  
   - `make`, `aspiration`, `engine_location`, `fuel_type`: label encoding.  
   - `fuel_system`: `pfi → 1`, else `0`.  
   - `engine_type`: `ohc → 1`, else `0`.  
4. Split dataset into input features (X) and output (*price*).  
5. Scale all features.  
6. Train Linear Regression (70% train, 30% test) using sklearn.  
7. Apply PCA for dimensionality reduction and retrain regression.  
8. Compare performance with and without PCA.  

---

## Files
- `ML_Assignment_3.ipynb` → Implementation of all three parts (Q1, Q2, Q3).  

---

## How to Run
1. Open the notebook in Jupyter Notebook or JupyterLab.  
2. Install required libraries:  
   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn
