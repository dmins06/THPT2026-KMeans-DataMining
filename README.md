# 📊 THPT2026-KMeans-DataMining

> Data Mining, Feature Engineering, and K-Means Clustering of the 2026 Vietnamese High School Graduation Examination Dataset.

![Python](https://img.shields.io/badge/Python-3.12-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.x-orange)
![Scikit--Learn](https://img.shields.io/badge/Scikit--Learn-1.7-green)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

---

## 📖 Overview

This project applies **Data Mining** techniques to analyze the **2026 Vietnamese High School Graduation Examination** dataset containing more than **1 million student records**.

The project focuses on discovering hidden patterns in examination results through **unsupervised learning**, specifically using the **K-Means clustering algorithm**.

Instead of predicting admission scores, this project aims to identify different groups of students based on their academic performance and examination characteristics.

---

## 🎯 Objectives

- Clean and preprocess raw examination data
- Perform feature engineering
- Calculate multiple university admission combinations
- Standardize numerical features
- Determine the optimal number of clusters using the Elbow Method
- Cluster students using K-Means
- Visualize clusters using Incremental PCA
- Analyze characteristics of each cluster
- Export clustering results for further analysis

---

## 📂 Dataset

The dataset contains over **1,000,000** examination records collected from the 2026 Vietnamese High School Graduation Examination.

Example attributes include:

- Candidate ID
- Mathematics
- Literature
- English
- Physics
- Chemistry
- Biology
- History
- Geography
- Civic Education
- Informatics
- Technology
- Foreign Languages (N1, N2, N3...)
- Province
- Examination Block

Additional features were generated during preprocessing.

---

## ⚙️ Data Preprocessing

The preprocessing pipeline includes:

- Removing unnecessary columns
- Handling missing values
- Converting data types
- Calculating total scores
- Calculating average scores
- Counting subjects taken
- Counting subjects with scores ≥ 8
- Counting subjects with scores ≥ 9
- Calculating the highest admission combination
- Determining the strongest admission block
- Feature normalization using StandardScaler

---

## 🎓 Admission Combinations

The project automatically computes more than **30 university admission combinations**, including:

- A00
- A01
- A02
- B00
- C00
- D01
- D07
- D14
- D15
- C03
- ...

For every candidate, the project determines:

- Highest admission combination
- Maximum admission score

---

## 🤖 Machine Learning Pipeline

```
Raw Dataset
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

## 📊 Features Used for Clustering

The K-Means model was trained using engineered numerical features:

- AVG_SCORE
- TOTAL_SCORE
- NUM_SUBJECT
- MAX_SCORE
- MIN_SCORE
- NUM_SCORE_8
- NUM_SCORE_9
- NUM_SCORE_PASS
- MAX_COMB_SCORE

---

## 🧠 Algorithms

### K-Means

The primary clustering algorithm used in this project.

Advantages:

- Fast
- Scalable
- Suitable for large datasets
- Easy to interpret

---

### Elbow Method

Used to determine the optimal number of clusters.

The optimal value selected:

```
K = 5
```

---

### Incremental PCA

Since the dataset contains more than one million records, **Incremental PCA** was used instead of standard PCA for visualization.

Benefits:

- Lower memory usage
- Suitable for large datasets
- Similar results to traditional PCA

---

## 📈 Cluster Analysis

Each cluster represents a group of students with similar examination performance.

Typical analysis includes:

- Average score
- Total score
- Strongest admission combination
- Preferred foreign language
- Cluster size
- Academic performance level

---

## 📦 Output Files

After execution, the project generates:

```
KetQua_PhanCum_THPT2026.xlsx

Cluster_Center.xlsx

PCA_Result.csv

IncrementalPCA_KMeans.png

kmeans_model.pkl

standard_scaler.pkl
```

---

## 🛠️ Technologies

- Python 3.12
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- OpenPyXL
- Joblib
- Jupyter Notebook

---

## 📁 Project Structure

```
THPT2026-KMeans-DataMining/

│
├── data/
│   └── DiemThi_THPTQG2026.csv
│
├── notebooks/
│   └── DataMining_THPT2026.ipynb
│
├── outputs/
│   ├── PCA_Result.csv
│   ├── Cluster_Center.xlsx
│   ├── KetQua_PhanCum_THPT2026.xlsx
│   └── IncrementalPCA_KMeans.png
│
├── models/
│   ├── kmeans_model.pkl
│   └── standard_scaler.pkl
│
├── requirements.txt
│
└── README.md
```

---

## 🚀 Installation

Clone the repository

```bash
git clone https://github.com/yourusername/THPT2026-KMeans-DataMining.git
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the notebook

```bash
jupyter notebook
```

---

## 📊 Future Improvements

Possible extensions include:

- DBSCAN clustering
- Hierarchical Clustering
- Gaussian Mixture Models
- Admission score prediction
- University recommendation system
- Interactive dashboard
- Web deployment

---

## 📄 License

This project is released under the MIT License.

---

## 👨‍💻 Author

**Minh Le Hoang Duy**

Information Systems Student

University of Transport Ho Chi Minh City

Vietnam

---

## ⭐ Acknowledgements

Special thanks to the Vietnamese High School Graduation Examination dataset and the open-source Python ecosystem, including Pandas, Scikit-learn, NumPy, and Matplotlib, for enabling large-scale educational data analysis.
