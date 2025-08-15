🛍️ Customer Segmentation using K-Means Clustering

📌 Overview
This project implements **K-Means clustering** to segment mall customers into meaningful groups based on their purchasing behavior and demographics.  
The segmentation can be used for **targeted marketing**, **customer relationship management**, and **business decision-making**.

📂 Dataset
- **File Name:** `Mall_Customers.csv`
- **Rows:** 200
- **Columns:** 5  
- **Features:**
  - `CustomerID` – Unique customer ID *(excluded from clustering)*
  - `Gender` – Customer gender *(optional in clustering)*
  - `Age` – Age of the customer
  - `Annual Income (k$)` – Annual income in thousands of dollars
  - `Spending Score (1-100)` – Spending score assigned by the mall

Dataset source: [Mall Customers Dataset – Kaggle] (https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

🔍 Methodology
1. **Data Loading & Exploration**
   - Imported CSV, inspected info, checked missing values
   - Visualized feature relationships using pair plots

2. **Feature Selection & Scaling**
   - Selected features: `Annual Income (k$)` & `Spending Score (1-100)`
   - Standardized values using `StandardScaler`

3. **Optimal K Selection**
   - Applied **Elbow Method** to visualize inertia vs. K
   - Calculated **Silhouette Scores** for cluster quality
   - Automatically selected the best K

4. **Model Training**
   - Trained **KMeans** with the optimal K
   - Saved model and scaler for reuse

5. **Cluster Analysis**
   - Calculated cluster centers (in original scale)
   - Interpreted customer segments

6. **Visualization**
   - Scatter plot of clusters with centroids
   - PCA visualization for multi-dimensional features

7. **Output Storage**
   - Saved clustered dataset (`Mall_Customers_Clustered.csv`)
   - Exported plots and model files

📊 Results
- **Optimal K:** Selected via silhouette score
- **Key Insights:**
  - High Income + High Spending → Premium customers
  - Low Income + High Spending → Budget-conscious but active buyers
  - Moderate Income + Low Spending → Low-engagement customers
- **Silhouette Score:** Shows good cluster separation

🛠️ Tech Stack
- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Joblib
- **Environment:** Jupyter Notebook

📅 Completed On August 15, 2025

🙌 Acknowledgment: 
This project is part of my AI/ML Internship to gain hands-on experience with classification algorithms using real-world datasets.

Author:
Shashank Chauhan 
Email: cshashank899@gmail.com.com GitHub: 
https://github.com/Shashank911
