# 🧬 Data Science Methods Evaluation: Assumptions in Diverse Datasets

![Let's Get Started](https://media1.tenor.com/m/r3XdvPsAV3kAAAAd/despicable-me-minions.gif)

## Project Plan – Submission for Thursday, April 10

### 📚 Course Information

This project is part of the **Data Science in Bio** course offered at the **University of Texas at San Antonio (UTSA)** in **Spring 2025**.  
- **Department:** Computer Science  
- **Instructor:** Dr. Jianhua Ruan  

---

### 🧬 DSinBIO Project – Evaluating ExcelFormer on Biological Datasets

This project explores whether **ExcelFormer**, a deep learning model, can outperform traditional machine learning models in predicting binary disease outcomes such as **distant metastasis in breast cancer** using real-world gene expression datasets.

---

---

![Microscope](https://img.icons8.com/color/96/000000/microscope.png)

### 👥 Team Composition

- **Nadia (Fatemeh Sadat) Masoumi**

## 📁 Datasets

We use four datasets representing both **microarray** and **scRNA-seq** gene expression profiles:

| Dataset   | Type               | Patients | Genes |
|-----------|--------------------|----------|-------|
| **ACES**      | Microarray         | 1616     | 12,750 |
| **METABRIC**  | Microarray         | 1884     | 20,182 |
| **NKI**       | Microarray         | 295      | 11,658 |
| **TCGA**      | scRNA-seq          | 5580     | 13,446 (protein-coding) |

All datasets are **labeled with binary outcomes** indicating metastasis status within 5 years.

---

## 🤖 Models to be Compared

### Deep Learning Models
- `ExcelFormer`
- `MLP` (Multilayer Perceptron)

### Traditional ML Models
- `Random Forest`
- `Support Vector Machine`
- `Gradient Boosting`
- `Logistic Regression`

---

## 📊 Evaluation Metrics

Each model will be evaluated using:

- **Accuracy**
- **Precision**
- **Recall**
- **F1-score**
- **AUC (Area Under the Curve)**

---

## 🧪 Methodology

1. Preprocess and normalize each dataset.
2. Apply **stratified splitting** to preserve class distributions in train/test sets.
3. Handle **class imbalance** using:
   - `class_weight='balanced'`
   - `SMOTE`
   - `SMOTE + Tomek Links`
   - `Borderline-SMOTE`
4. Train all models on each dataset and evaluate with the listed metrics.
5. Compare results across datasets and identify:
   - Where ExcelFormer excels.
   - When traditional models are preferable.
6. Analyze results in the context of:
   - Sample size
   - Feature dimensionality
   - Class balance
   - Model complexity

---

## 🔍 Outcomes Expected

- Determine the robustness of ExcelFormer across small and large gene expression datasets.
- Understand the model's generalizability across microarray and scRNA-seq data.
- Provide guidance for researchers choosing between deep and classical ML models in bioinformatics.

---



_This README will evolve throughout the project as we finalize our method(s), datasets, and results._

