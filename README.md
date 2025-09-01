# Pattern Classification of Stock Price Movement  

This project applies unsupervised learning techniques to classify patterns in the FTSE 100 stock index from 2020–2024. By clustering stocks based on behavioural similarities, the study explores hidden market structures, sectoral patterns, and investment insights.  

---

## 📌 Objectives  
- Detect and classify meaningful stock price movement patterns.
- Determine optimal number of clusters. 
- Compare clustering algorithms for interpretability and stability.  
- Assess the role of data normalization in clustering outcomes.
- Translate clustering results into actionable portfolio insights.  

---

## 📊 Dataset  
- Source: [Yahoo Finance](https://finance.yahoo.com/)  
- Period: January 2020 – December 2024  
- Constituents: 94 FTSE 100 stocks (after filtering incomplete data).  
- Transformation: Mid-prices converted into percentage differences.  

---

## ⚙️ Methodology  
1. **Preprocessing**  
   - Raw vs normalized datasets (Z-score, Min–Max, Log, Robust, Decimal scaling).  

2. **Clustering Algorithms**  
   - K-Means  
   - Gaussian Mixture Models (GMM)  
   - Agglomerative Hierarchical Clustering  
   - BIRCH  
   - DBSCAN  

3. **Evaluation Metrics**  
   - Silhouette Score  
   - Davies–Bouldin Index  
   - Calinski–Harabasz Index
   - Cluster plots
   - UMAP & t-SNE visualizations  

---

## 📈 Results  
- **Optimal clusters**: k = 5 (balanced structure).  
- **Best-performing algorithms**: Agglomerative & BIRCH.  
- **Raw dataset** retained financial meaning better than normalized.  
- **Investment insights**: Uptrend clusters gave best Sharpe ratios; downtrend clusters showed negative returns.  

---

## 📂 Repository Structure  


- data/                       # Contains raw and processed FTSE 100 stock data

- notebooks/                   # Jupyter notebooks for clustering experiments
   - clustering_4_raw.ipynb
   - clustering_5_raw.ipynb
   - clustering_7_raw.ipynb
   - clustering_10_raw.ipynb
   - clustering_5_robust_norm.ipynb
   - clustering_5_zscore_norm.ipynb
   - clustering_5_decimal_norm.ipynb
   - data_normalisations.ipynb

- README.md 
