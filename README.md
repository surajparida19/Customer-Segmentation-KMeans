# 🛍️ Customer Segmentation using K-Means

[![Python](https://img.shields.io/badge/Python-3.9-blue)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML%20Library-orange)](https://scikit-learn.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-red)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-green)](https://seaborn.pydata.org/)

---

**Task-3 | Data Analysis & Data Science using Python**

This project performs **customer segmentation** using **K-Means clustering**. The aim is to group customers based on purchasing behavior (Age, Annual Income, Spending Score) so businesses can implement targeted marketing strategies and resource allocation.

---

## 🎯 Objective
Segment customers using clustering techniques to:
- Identify high-value and budget-conscious customers
- Design targeted marketing campaigns
- Improve retention through tailored offers
- Support strategic allocation of resources

---

## 📂 Dataset
**File:** `customer_data.csv`  
**Columns:**
- `CustomerID` — Unique identifier
- `Age` — Customer age
- `Annual Income` — Annual income (currency)
- `Spending Score` — Score based on customer spending behavior

---

## 🛠️ Libraries & Tools
- Python (3.9+)
- Pandas, NumPy
- Scikit-Learn (StandardScaler, KMeans, PCA)
- Matplotlib, Seaborn
- Jupyter Notebook

---

## 🧩 Project Workflow

### 1. Load & Inspect
- Load dataset with `pandas.read_csv()`
- Inspect shape, dtypes, missing values, duplicates, summary statistics

### 2. Data Preprocessing
- Encode categorical variables if present
- Standardize features using `StandardScaler` (important for clustering)

### 3. Optimal Cluster Selection
- Elbow Method (WCSS vs k) to find elbow point
- Optionally use Silhouette Score to validate k

### 4. Model Training
- Apply K-Means with chosen `k` (k = 5 from Elbow Method)
- Assign cluster labels to each customer and append as `Cluster` column

### 5. Visualization
- Elbow curve for k selection
- PCA (2D) scatter plot colored by cluster
- Pair plots to examine feature distributions per cluster
- Visualize cluster centroids for interpretation

### 6. Cluster Profiling
- Compute cluster-wise mean statistics
- Interpret each cluster (e.g., “High income — high spender”, “Young — moderate spender”)

---

## 📊 Deliverables
1. **Clustered dataset** with `Cluster` column  
2. **Visualizations**
   - Elbow plot (WCSS vs k)
   - PCA 2D scatter plot
   - Pair plots and centroid visuals
3. **Recommendations / Business Insights**
   - Which segments to prioritize for premium offers
   - Candidates for loyalty programs
   - Tailored promotions per age/income group

---

## ⚙️ Project Structure




---

## 💡 Key Findings (example)
- **5 distinct clusters** identified (based on Elbow)
- Cluster examples:
  - High Income — High Spending → target with premium offers & loyalty
  - Low Income — Low Spending → promote value bundles
  - Young Moderate Income — High Spending → lifestyle & upsell campaigns
- Actionable recommendations included in notebook

---

## 🚀 Future Enhancements
- Compare with DBSCAN and Hierarchical Clustering
- Validate clusters with Silhouette and Davies-Bouldin scores
- Build interactive dashboard (Streamlit / Power BI)
- Integrate more features (frequency, recency, monetary values)

---

## 📁 Files Included
- `customer_segmentation.ipynb` — main notebook with code and visualizations  
- `customer_data.csv` — dataset used for analysis  
- `plots/` — generated PNG plots (Elbow, PCA, pairplots)  
- `requirements.txt` — project dependencies

---

## 👤 Author
**Suraj Parida**  
Email: surajparida9191@gmail.com
