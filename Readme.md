# Task 8 – K-Means Clustering (AI & ML Internship)

**Author:** Mrutyunjay Joshi  
**Internship:** Elevate Labs – AI & ML Internship  
**Date:** October 2025  

---

## Objective
Perform **unsupervised learning** using **K-Means Clustering** to identify natural groupings within a dataset and visualize how data points are segmented based on similarity.  
This task focuses on learning the concepts of clustering, evaluating clusters, and understanding unsupervised learning behavior.

---

## Tools & Technologies Used
- **Programming Language:** Python  
- **Libraries:**  
  - `NumPy`  
  - `Pandas`  
  - `Matplotlib`  
  - `Seaborn`  
  - `Scikit-learn`

---

## Dataset
**Dataset Used:** [Mall Customer Segmentation Dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

**Features Selected:**
- `Annual Income (k$)`  
- `Spending Score (1–100)`

These attributes were used to group customers with similar income and spending behavior.

---

## Steps Implemented

### Step-1 : Import and Prepare Data
Imported all necessary libraries, loaded the dataset using Pandas, and explored its structure.

### Step-2 : Data Preprocessing
Selected relevant numerical columns and standardized the features using **StandardScaler** to ensure balanced feature contribution.

### Step-3 : Finding Optimal K (Elbow Method)
Plotted inertia values for cluster counts from 1 to 10 to locate the “elbow point,” which indicated the optimal K (≈ 5).

### Step-4 : Applying K-Means Algorithm
Applied K-Means with K = 5, assigning each data point to the nearest centroid and computing cluster centers.

### Step-5 : Visualizing Clusters
Displayed a 2-D scatter plot using Matplotlib and Seaborn to visualize the formed clusters and their centroids.

### Step-6 : Evaluating the Model
Calculated the **Silhouette Score** to evaluate cluster separation and quality.

### Step-7 : Saving the Results
Exported the final dataset with cluster labels to `task8_clustered_customers.csv`.

---

## Results & Observations

| Metric | Result |
|---------|---------|
| **Optimal K (Clusters)** | 5 |
| **Silhouette Score** | ≈ 0.52 |
| **Output File** | `task8_clustered_customers.csv` |

### Insights
- High-income & high-spending customers form premium clusters.  
- Low-income & low-spending customers form budget clusters.  
- Remaining clusters represent moderate spending patterns across different income ranges.