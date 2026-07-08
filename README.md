# 📊 THPT2026-KMeans-DataMining

> **Data Mining and K-Means Clustering of the 2026 Vietnamese High School Graduation Examination Dataset**

---

## 📖 Overview

This project applies **Data Mining** techniques to analyze the **2026 Vietnamese High School Graduation Examination** dataset containing more than **1 million candidate records**.

The primary objective is to discover hidden patterns in examination results through **unsupervised learning**, using the **K-Means clustering algorithm**.

The project includes data preprocessing, feature engineering, clustering, dimensionality reduction, visualization, and cluster analysis.

---

## ⚠️ Disclaimer

This repository is published for **academic research, educational demonstration, and portfolio purposes only**.

The source code is provided for learning and reference.

**Unauthorized copying, modification, redistribution, or commercial use of this project is strictly prohibited without prior written permission from the author.**

---

# 🎯 Objectives

The project aims to:

- Clean and preprocess raw examination data
- Handle missing values
- Generate additional analytical features
- Calculate multiple university admission combinations
- Normalize numerical features
- Determine the optimal number of clusters
- Cluster candidates using K-Means
- Visualize clustering results using Incremental PCA
- Analyze characteristics of each cluster
- Export clustering reports

---

# 📂 Dataset

The dataset contains over **1,000,000 Vietnamese candidates** participating in the **2026 High School Graduation Examination**.

The dataset includes:

- Candidate ID
- Mathematics
- Literature
- Foreign Language
- Physics
- Chemistry
- Biology
- History
- Geography
- Civic Education
- Informatics
- Technology
- Province
- Examination Subjects

Additional features are generated during preprocessing.

---

# ⚙️ Data Preprocessing

The preprocessing workflow consists of:

- Removing unnecessary columns
- Handling missing values
- Data type conversion
- Feature engineering
- Score normalization
- Admission combination calculation

Generated features include:

- Average Score
- Total Score
- Number of Subjects
- Maximum Score
- Minimum Score
- Number of Scores ≥ 8
- Number of Scores ≥ 9
- Number of Passing Subjects
- Best Admission Combination
- Maximum Admission Combination Score

---

# 🎓 University Admission Combinations

The project automatically calculates more than **30 admission combinations**, including:

- A00
- A01
- A02
- B00
- C00
- C03
- D01
- D07
- D14
- D15
- ...

For every candidate, the system determines:

- Best admission combination
- Maximum admission score

---

# 🤖 Machine Learning Pipeline

```text
Raw Examination Dataset
            │
            ▼
Data Cleaning
            │
            ▼
Feature Engineering
            │
            ▼
Feature Scaling
            │
            ▼
Elbow Method
            │
            ▼
K-Means Clustering
            │
            ▼
Incremental PCA
            │
            ▼
Cluster Analysis
            │
            ▼
Export Results
```

---

# 📊 Features Used for Clustering

The K-Means algorithm uses the following engineered numerical features:

| Feature |
|----------|
| AVG_SCORE |
| TOTAL_SCORE |
| NUM_SUBJECT |
| MAX_SCORE |
| MIN_SCORE |
| NUM_SCORE_8 |
| NUM_SCORE_9 |
| NUM_SCORE_PASS |
| MAX_COMB_SCORE |

---

# 🧠 Algorithms

## K-Means Clustering

K-Means is the primary clustering algorithm used to group candidates with similar examination characteristics.

Advantages:

- Fast
- Scalable
- Suitable for large datasets
- Easy to interpret

---

## Elbow Method

Used to determine the optimal number of clusters.

Selected value:

```
K = 5
```

---

## Incremental PCA

Because the dataset contains over **1 million candidates**, **Incremental PCA** is used instead of traditional PCA.

Benefits:

- Lower memory usage
- Faster processing on large datasets
- Efficient visualization

---

# 📈 Cluster Analysis

Each cluster represents candidates with similar academic performance.

The project analyzes:

- Cluster size
- Average score
- Total score
- Best admission combination
- Foreign language selection
- Academic performance characteristics

---

# 📦 Output Files

After execution, the project generates:

```text
KetQua_PhanCum_THPT2026.xlsx

Cluster_Center.xlsx

PCA_Result.csv

IncrementalPCA_KMeans.png

kmeans_model.pkl

standard_scaler.pkl
```

---

# 🛠 Technologies

- Python 3.12
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- OpenPyXL
- Joblib
- Jupyter Notebook

---

# 📁 Project Structure

```text
THPT2026-KMeans-DataMining
│
├── data
│   └── DiemThi_THPTQG2026.csv
│
├── notebooks
│   └── DataMining_THPT2026.ipynb
│
├── outputs
│   ├── KetQua_PhanCum_THPT2026.xlsx
│   ├── Cluster_Center.xlsx
│   ├── PCA_Result.csv
│   └── IncrementalPCA_KMeans.png
│
├── models
│   ├── kmeans_model.pkl
│   └── standard_scaler.pkl
│
├── requirements.txt
│
│
└── README.md
```

---

# 🚀 Installation

Clone the repository

```bash
git clone https://github.com/your-username/THPT2026-KMeans-DataMining.git
```

Go to the project directory

```bash
cd THPT2026-KMeans-DataMining
```

Install dependencies

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook

```bash
jupyter notebook
```

---

# 📈 Future Improvements

Potential future work includes:

- DBSCAN Clustering
- Hierarchical Clustering
- Gaussian Mixture Models (GMM)
- Candidate Recommendation System
- Admission Score Prediction
- Interactive Dashboard
- Web-based Application

---

# 👨‍💻 Author

**Le Hoang Duy Minh - Diminn**

**Undergraduate Student in Data Science and Artificial Intelligence**

Ho Chi Minh City University of Transport (UTH)

Vietnam

---

# 📬 Contact

For questions, suggestions, or collaboration, please contact the author via GitHub.

---

# 📚 Citation

If this project contributes to your research or academic work, please cite the repository instead of copying the source code.

Author:

**Le Hoang Duy Minh**

Project:

**THPT2026-KMeans-DataMining**

Year:

**2026**

---

# 🙏 Acknowledgements

This project was developed as an academic Data Mining project using publicly available examination data.

Special thanks to the open-source Python community and the following libraries:

- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- OpenPyXL
- Joblib

---

# 📄 Copyright

Copyright © 2026 Diminn

All rights reserved.

This repository is provided for educational and reference purposes only.

No permission is granted to copy, modify, redistribute, publish, or use this project, in whole or in part, without prior written permission from the author.
