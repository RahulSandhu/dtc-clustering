<div align="justify">

# Differentiated Thyroid Cancer Clustering Analysis

This repository contains a comprehensive unsupervised machine learning analysis
of differentiated thyroid cancer (DTC) patients. The project applies clustering
algorithms to identify distinct clinical phenotypes and their association with
disease recurrence, revealing four patient subgroups with markedly different
risk profiles through quantitative analysis, feature importance evaluation, and
statistical validation.

## 🚀 Setup

1. **Clone the repository**

```bash
   git clone https://github.com/yourusername/dtc-clustering
   cd dtc-clustering
```

2. **Create and activate a virtual environment**

```bash
   python3 -m venv .venv
   source .venv/bin/activate
```

3. **Install dependencies**

```bash
   pip install -r requirements.txt
```

## 📊 Dataset

The project analyzes a cohort of **383 differentiated thyroid cancer patients**
with comprehensive clinical, pathological, and treatment response data. Key
features include:

- **Demographics**: Age, gender
- **Clinical characteristics**: Smoking history, disease focality, lymph node
  involvement (adenopathy)
- **Risk stratification**: ATA (American Thyroid Association) risk categories
- **Pathology**: Disease stage
- **Treatment outcomes**: Response to therapy
- **Follow-up**: Recurrence status

The analysis uses **K-means clustering** with optimal cluster selection via the
elbow method and silhouette analysis to identify natural patient subgroups.

## 🔬 Results

Our clustering analysis identified **four distinct patient phenotypes** with
different recurrence patterns:

- **Cluster 0 (n=69, 18.0%)**: Young patients (median age 33) with
  intermediate-risk features and poor treatment response. Recurrence rate:
  **65.2%**

- **Cluster 1 (n=88, 23.0%)**: Middle-aged patients (median age 51) with
  low-risk disease and favorable outcomes. Recurrence rate: **9.1%**

- **Cluster 2 (n=57, 14.9%)**: Older patients (median age 62) with multiple
  adverse features including male predominance, heavy smoking, and advanced
  stage. Recurrence rate: **82.5%** (highest risk)

- **Cluster 3 (n=169, 44.1%)**: Youngest patients (median age 30) with optimal
  prognosis and excellent treatment response. Recurrence rate: **4.7%** (lowest
  risk)

Key findings revealed that risk stratification (26.8%), response to therapy
(21.6%), and adenopathy (14.9%) were the most discriminative features. Pairwise
statistical comparisons showed significant differences between clusters, with
C0-C3 and C2-C3 demonstrating the strongest divergence.

## 🎓 Acknowledgements

- [UCI Machine Learning
  Repository](https://archive.ics.uci.edu/dataset/915/differentiated+thyroid+cancer+recurrence)
  — Differentiated Thyroid Cancer Recurrence dataset
- Developed as part of the Machine Learning course in the Master in Health Data
  Science at Universitat Rovira i Virgili (URV)

</div>
