# 📊 Student Data Preprocessing

A simple Data Science project that demonstrates the preprocessing stage before building a Machine Learning model. This project focuses on cleaning and transforming student data using Python.

---

## 📖 Project Overview

Data preprocessing is an essential step in data analysis and machine learning. In this project, the dataset is transformed through several preprocessing techniques, including:

- Data Loading
- Data Encoding
- Feature Scaling
- Feature Engineering
- Correlation Analysis
- Data Visualization

The goal is to prepare the dataset so it can be used efficiently for further analysis and predictive modeling.

---

## 🗂 Dataset Features

| Feature | Description |
|---------|-------------|
| ID | Student ID |
| Usia | Student Age |
| JamBelajar | Study Hours |
| Kehadiran | Attendance Percentage |
| Tugas | Assignment Score |
| NilaiUjian | Exam Score |
| Ekstrakurikuler | Participation in Extracurricular Activities |
| StatusEkonomi | Economic Status |
| Lulus | Graduation Status |

---

## ⚙️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Google Colab

---

## 🚀 Preprocessing Pipeline

✔ Read CSV Dataset

✔ Encode Categorical Features

✔ Normalize Numerical Features

✔ Create New Features

✔ Correlation Analysis

✔ Heatmap Visualization

---

## 💻 Code Example

### Encoding Categorical Data

```python
df["Ekstrakurikuler"] = df["Ekstrakurikuler"].map({
    "Tidak": 0,
    "Ya": 1
})

df["StatusEkonomi"] = df["StatusEkonomi"].map({
    "Rendah": 0,
    "Menengah": 1,
    "Tinggi": 2
})
```

### Feature Engineering

```python
df["RataNilai"] = (
    df["Tugas"] + df["NilaiUjian"]
) / 2

df["Produktivitas"] = (
    df["JamBelajar"] * df["Kehadiran"]
)
```

---

## 📈 Output

The preprocessing process produces:

- Encoded dataset
- Normalized numerical features
- New engineered features
- Correlation matrix
- Heatmap visualization

---

## 📁 Repository Structure

```
Student-Data-Preprocessing/
│── dataset.csv
│── Data_Sains_Project13.ipynb
│── README.md
│── LICENSE
│── .gitignore
└── images/
    └── heatmap.png
```

---

## 🎯 Learning Outcomes

Through this project, I learned how to:

- Transform categorical data into numerical values.
- Normalize numerical features using MinMaxScaler.
- Create meaningful features from existing data.
- Analyze relationships between variables using correlation.
- Visualize preprocessing results with heatmaps.

---

⭐ If you find this project useful, feel free to explore the repository and learn from the preprocessing workflow.
