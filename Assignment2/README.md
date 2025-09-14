# Assignment 2: Classification (Bike Buyer Prediction)

## Objective
The goal of this assignment is to analyze the Adventure Works Cycles customer dataset and build preprocessing pipelines to predict potential bike buyers. By identifying key customer attributes, the marketing department can better target future customers for a mailing campaign.

Dataset: [Adventure Works Cycles Customer Data (Kaggle)](https://www.kaggle.com/datasets/jahias/microsoft-adventure-works-cycles-customer-data)

---

## Tasks

### Part I: Feature Selection, Cleaning, and Preprocessing
1. Examine all attributes in the dataset.  
2. Select only relevant features for predicting future bike buyers.  
3. Remove unnecessary attributes.  
4. Create a new DataFrame with selected attributes.  
5. Determine each attribute’s data type (Discrete, Continuous, Nominal, Ordinal, Interval, Ratio).

### Part II: Data Preprocessing and Transformation
1. Handle missing values.  
2. Normalize data.  
3. Apply discretization (binning) for continuous attributes or categorical attributes with many unique values.  
4. Apply standardization/normalization where needed.  
5. Apply binarization (One-Hot Encoding) for categorical attributes.

### Part III: Proximity / Correlation Analysis
1. Ensure all attributes are on the same scale for numeric features and binarized for nominal features.  
2. Calculate similarity between two objects using:  
   - Simple Matching  
   - Jaccard Similarity  
   - Cosine Similarity  
3. Calculate correlation between **Commute Distance** and **Yearly Income**.

---

## Files
- `ML_Assignment_1_and_2.ipynb` → Contains the full implementation of Assignment
