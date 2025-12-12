# 🧬 Cancer Classification using Hybrid Deep Learning and Genetic Algorithms

Cancer classification is challenging due to strong molecular heterogeneity across tumor types.  
This project proposes a **hybrid framework** that combines **Genetic Algorithms (GA)** for gene subset selection with **deep learning models** to achieve accurate and interpretable cancer classification.

---

## 🔍 Project Highlights

- Genetic Algorithms for optimal gene subset selection  
- TabNet and SAINT models for binary and multiclass cancer classification  
- Gradient-based interpretability to identify biologically meaningful gene biomarkers  
- High predictive performance with strong biological relevance  

**Results:**
- **98.7% accuracy** on binary cancer classification  
- **95.6% accuracy** on multiclass (33 tumor types) classification  
- Successful recovery of known oncogenes such as *BRCA1*, *TP53*, and *KRAS*

---

## 📊 Dataset

**Source:** UCSC Xena – TCGA Pan-Cancer  
**Samples:** 10,459  
**Genes:** 17,950  
**Classes:** 33 tumor types  

### Preprocessing Steps

- Exon-to-gene collapsing  
- Median imputation for missing values  
- Low-variance gene filtering  
- Z-score normalization  
- Metadata mapping using the GDC API  

---

## 🧠 Models Used

### Deep Learning Models

- **TabNet**  
  Interpretable attention-based deep learning model designed for tabular data.

- **SAINT**  
  Transformer-based architecture with dual (row and column) attention and contrastive pretraining.

Both models were trained using **Adam / AdamW optimizers**, cosine learning rate scheduling, and early stopping.

---

## 🧪 Feature Selection

### Genetic Algorithm (GA)

Genetic Algorithms were used to select compact and informative gene subsets, reducing dimensionality while preserving discriminative biological signals.

---

## 🔬 Model Interpretability

### Gradient-Based Attribution

Gradient attribution and Integrated Gradients were applied to uncover biologically meaningful gene biomarkers.

**Key genes identified include:**
- *BRCA1*, *ESR1*, *PGR* — Breast cancer  
- *TP53*, *KRAS*, *EGFR* — Lung and colon cancers  
- *APC*, *SMAD4* — Colorectal cancer  

---

## 🎯 Applications

- Molecular cancer subtype classification  
- Biomarker discovery  
- Precision oncology research  
- Interpretable deep learning in genomics  

---

## ⚠️ Disclaimer

This project is intended for research purposes only and should not be used for clinical decision-making without expert validation.
