# 💡 K-Means Clustering Mini Project

This is a mini project demonstrating how to apply **K-Means Clustering** on a dataset (e.g., heart disease dataset) for unsupervised learning. The goal is to cluster patients based on similar features without using labeled outcomes.

---

## 📂 Project Overview

- Load and preprocess a medical dataset (e.g., heart disease data).
- Clean the data by handling missing values and converting categorical data.
- Apply **K-Means clustering**.
- Determine the optimal number of clusters using the **Elbow Method**.
- Visualize clusters and interpret the results.

---

## 📊 Dataset

The dataset used is based on health/heart-related patient information. It contains features such as:

- Age
- Sex
- Chest pain type
- Blood pressure
- Cholesterol levels
- Fasting blood sugar
- Maximum heart rate achieved
- Exercise-induced angina
- and more..

> Note: Actual column names were inferred and cleaned due to missing headers in the raw CSV.

---

## ⚙️ Technologies Used

- Python 🐍
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## 📌 Key Steps

1. **Data Cleaning**  
   - Replaced `"?"` with NaNs and dropped rows with missing data.
   - Converted all string-based numeric values to floats or integers.

2. **Feature Scaling**  
   - Standardized the features using `StandardScaler` to normalize the input for K-Means.

3. **Choosing K**  
   - Used the **Elbow Method** to find the optimal number of clusters by plotting inertia vs. number of clusters.

4. **Model Training**  
   - Applied `KMeans` clustering from scikit-learn.
   - Cluster labels were added to the dataset for further analysis.

5. **Visualization**  
   - Scatter plots and countplots were created to analyze how data is grouped into clusters.

---

## 📈 Results & Interpretation

- **Optimal Clusters Chosen**: `k = 3` (example; based on Elbow curve).
- Patients were grouped into 3 distinct clusters based on health attributes.
- Clusters can potentially represent different **risk groups** or **types of heart conditions** — valuable for exploratory analysis or further classification.

---

## 🧠 Possible Improvements

- Use **PCA** or **t-SNE** for dimensionality reduction and better visualization.
- Test with **hierarchical clustering** for comparison.
- Label the clusters by comparing with real outcomes (if available).

---

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git

## ⚙️ Step 2: Install Dependencies

You can install the required Python packages using pip:

pip install pandas numpy matplotlib seaborn scikit-learn


## 🧪 Step 3: Run the Project

Run the notebook to follow the K-Means Clustering workflow:
 ```bash
jupyter notebook
```


## 📸 Screenshots

🔍 PCA Visualization of Clusters
This plot shows how the clusters formed using K-Means appear in reduced 2D space using PCA.

![Image](https://github.com/user-attachments/assets/d1d9ae9c-a384-436a-b2f0-2997edded7db)

🧠 Elbow Method - Finding the Optimal Number of Clusters
This graph helps identify the optimal number of clusters by showing the inertia value for different values of K.

![Image](https://github.com/user-attachments/assets/a346507e-46c2-4447-8f9d-1628182a48de)



