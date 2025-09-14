# Temporal Clustering of Firms by Analyst Coverage

![Python](https://img.shields.io/badge/python-3.10+-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Course](https://img.shields.io/badge/course-The%20Art%20of%20Analyzing%20Big%20Data-orange)

Final project for the course **The Art of Analyzing Big Data** (Ben-Gurion University, 2025).

---

## 📄 Project Report
I **highly recommend** reading the PDF for the full details, results, and discussion:  
👉 [Temporal_Clustering_of_Firms_by_Analyst_Coverage.pdf](./Temporal_Clustering_of_Firms_by_Analyst_Coverage.pdf)

---

## Overview
This project explores how to cluster firms based on **shared financial analyst coverage** and how these clusters evolve over time.  
We construct **firm–firm similarity networks**, embed them with **Node2Vec**, and apply clustering methods to uncover dynamic structures in financial markets.

The analysis focuses on:
- **Graph construction**: firm–analyst bipartite projection using sparse matrix algebra  
- **Embeddings**: Node2Vec with edge duplication to approximate weighted walks  
- **Clustering**: K-means with anchor-based incremental assignment across years  
- **Evaluation**: Cluster stability (tenure, switching rates), return predictability, case studies  

---

## Results (Highlights)
- Clusters show **long-term persistence**, with median tenure ≈ 3 years  
- Switching between clusters declined over time, stabilizing around 5% annually  
- Clusters capture **economic communities** (e.g., retailers, automakers, big tech hybrids)  
- Forward return analysis reveals heterogeneity across clusters, though forecasting remains challenging  

---

## Requirements
To reproduce the code (without data), install dependencies:

```bash
# Using pip
pip install -r requirements.txt
