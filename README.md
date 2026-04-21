# DM_HW_3

This repository contains my submission code and generated outputs for **Homework 3** in **Data Mining**.

## Overview

This homework has two main parts:

### Task 1: Algorithmic Analysis of K-Means Clustering
In Task 1, K-means clustering was implemented **from scratch** using the provided dataset.  
Three distance/similarity measures were compared:

- Euclidean distance
- \(1 -\) Cosine similarity
- \(1 -\) Generalized Jaccard similarity

The analysis includes:
- SSE comparison
- cluster-label accuracy using majority voting
- convergence behavior
- effect of different stopping conditions
- result plots

### Task 2: Recommender Systems with Matrix Data
In Task 2, a recommender system was built using the `ratings_small.csv` dataset.  
Three model types were compared:

- PMF-style matrix factorization using SVD
- User-based Collaborative Filtering
- Item-based Collaborative Filtering

The analysis includes:
- 5-fold cross-validation
- RMSE and MAE comparison
- similarity metric comparison (cosine, MSD, Pearson)
- effect of number of neighbors \(K\)
- result plots

---

## Repository Contents

### Notebooks
- `HW3_Task1.ipynb`  
  Contains the full code, outputs, and plots for Task 1.

- `HW3_Task2.ipynb`  
  Contains the full code, outputs, and plots for Task 2.

### Task 1 Plot Files
- `task1_sse.png`
- `task1_accuracy.png`
- `task1_iterations.png`

### Task 2 Plot Files
- `task2_similarity_rmse.png`
- `task2_similarity_mae.png`
- `task2_k_rmse.png`
- `task2_k_mae.png`

### Report
- `HW3_Report.pdf`  
  Final PDF report for the assignment.

---

## Datasets Used

### Task 1
- `kmeans_data.zip`
  - `data.csv`
  - `label.csv`

### Task 2
- `ratings_small.csv.zip`
  - `ratings_small.csv`

> Note: These datasets were used to run the notebooks, but depending on submission preference, they may or may not be uploaded to this repository.

---

## Tools and Libraries

The work in this repository uses Python along with the following main libraries:

- `numpy`
- `pandas`
- `matplotlib`
- `zipfile`
- `surprise` (for recommender systems in Task 2)

Task 1 was executed in a Jupyter-style notebook environment.  
Task 2 was executed in Google Colab because the `surprise` package required a compatible runtime setup.

---

## Task 1 Summary

Task 1 focuses on comparing three K-means variants using different distance measures.

### Main steps
1. Load the dataset from `kmeans_data.zip`
2. Set \(K\) equal to the number of unique labels
3. Implement K-means from scratch
4. Compute SSE
5. Assign cluster labels using majority voting
6. Compute predictive accuracy
7. Compare iterations, runtime, and stopping conditions
8. Generate plots

### Outputs included
- SSE comparison table
- accuracy comparison table
- stopping condition analysis
- generated figures for report use

---

## Task 2 Summary

Task 2 focuses on recommender system evaluation using movie rating data.

### Main steps
1. Load `ratings_small.csv`
2. Convert the ratings into Surprise-compatible format
3. Evaluate:
   - PMF-style SVD
   - User-based CF
   - Item-based CF
4. Use 5-fold cross-validation
5. Compare RMSE and MAE
6. Test cosine, MSD, and Pearson similarities
7. Test different neighbor values \(K\)
8. Generate plots for the report

### Outputs included
- model comparison table
- similarity metric comparison
- neighbor-size comparison
- generated figures for report use

---

## How to Run

### Task 1
Open:

`HW3_Task1.ipynb`

Run all cells in order.

### Task 2
Open:

`HW3_Task2.ipynb`

Run all cells in order.

> Important: If running Task 2 in Google Colab, make sure the required package setup is completed before executing the notebook cells.

---

## Notes

- The notebooks include both code and output for transparency.
- The report itself does **not** include pasted code, following assignment instructions.
- The plots saved in this repository were used in the final PDF report.
- Task 2 used a PMF-style latent factor approach through SVD for practical implementation.

---

## Author

**Jay Sonawane**

---

## Submission Note

This repository is provided as the code-access link for Homework 3 so the TA can review:
- source code
- notebook outputs
- generated plots
- experiment structure
