# 🛍️ Mall Customer Segmentation using K-Means Clustering

This project uses **unsupervised learning** to segment mall customers into meaningful groups using the **K-Means clustering** algorithm. It helps identify distinct customer profiles based on their gender, age, annual income, and spending behavior.


## 📌 Project Overview

The goal is to group similar customers together so that businesses can:
- Understand customer behavior
- Personalize marketing strategies
- Improve customer satisfaction and sales

We use the **Mall Customers** dataset which contains:
- Customer ID
- Gender
- Age
- Annual Income (in $1000s)
- Spending Score (1–100)

---

## 🧠 What the Code Does

1. **Load and clean the dataset**  
   - Drops `CustomerID` as it is not useful for clustering.
   - Converts `Gender` to numeric using Label Encoding.

2. **Visualize data**  
   - Displays pairwise relationships using `seaborn.pairplot`.

3. **Elbow Method to find optimal k**  
   - Trains KMeans for `k=1 to 10` clusters.
   - Plots the inertia (sum of squared distances) to find the "elbow" point.

4. **Train K-Means model**  
   - Fits the model using the chosen `k` (e.g. 5).
   - Adds the cluster labels to the dataset.

5. **Visualize final clusters**  
   - Plots clusters using `Annual Income` and `Spending Score`.

6. **Evaluate clustering**  
   - Calculates and prints the **Silhouette Score**.

## 🧾 Dataset

**Filename:** `Mall_Customers.csv`  
Columns:
- `CustomerID` (dropped during processing)
- `Gender`
- `Age`
- `Annual Income `
- `Spending Score `

## 🛠️ Requirements

Make sure you have these Python libraries installed


